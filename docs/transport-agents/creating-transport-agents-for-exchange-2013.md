---
title: Создание агенты транспорта для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Сведения о создании настраиваемых транспортных агентов для Exchange 2013 и требования к системе для создания пользовательских агентов.
ms.openlocfilehash: 6146e37c44441bed1d30d08f71ede255dba26440
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761293"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Создание агенты транспорта для Exchange 2013

Сведения о создании настраиваемых транспортных агентов для Exchange 2013 и требования к системе для создания пользовательских агентов.
  
**Применимо к:** Exchange Server 2013
  
Exchange Server 2013 включает в себя ряд агенты транспорта, которые можно использовать для обработки сообщений. С помощью сборки, входящие в состав Exchange, можно создавать свои собственные пользовательские агенты для выполнения определенных задач в соответствии с потребностями организации. Например можно использовать агент транспорта SmtpReceiveAgent для перехвата сообщений, которые получены с помощью протокола SMTP и процесс преобразования формата форматированного текста в теле сообщения. Агент транспорта RoutingAgent можно использовать для записи в журнал сообщений, проходящих через сервер на маршрут на другой сервер. Также можно создавать более сложные функции, которые позволяют использовать более одного типа агента. Например для создания антивирусного агента, можно реализовать SmtpReceiveAgent и RoutingAgent агента. Если компонент локальной сети, не поддерживает протокол SMTP, можно использовать агента транспорта DeliveryAgent для связи между сервером Exchange server и внешним компонентом. 
  
В этой статье описаны необходимые условия для и задачи, выполняемые при создании собственного агента транспорта. Сведения о создании агенты транспорта конкретных см [RoutingAgent агента транспорта для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Создание SmtpReceiveAgent агента транспорта для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), [Создать агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Необходимые условия для создания агента транспорта
<a name="bk_prerequisites"> </a>

Ниже приведены компоненты, необходимые для реализации агента транспорта.
  
- Компьютер под управлением Exchange 2013, на котором работает служба транспорта переднего плана на сервере клиентского доступа или пограничный транспортный или транспортной службы на сервере почтовых ящиков. Сведения об архитектуре роли сервера в Exchange 2013 видеть [транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Следующие сборки для классов агента транспорта:
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- .NET Framework 4.5
    
Мы также рекомендуем вам установить Visual Studio 2012. Агенты транспорта можно реализовать с помощью Visual Basic .NET или C#.
  
## <a name="referencing-the-assemblies"></a>Создание ссылок на сборки
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 предоставляет библиотеку классов, которые поддерживают расширение поведения транспорта Exchange. Эти классы требуют .NET Framework 4.5. Вы можете реализовать агенты транспорта на основе этих классов с помощью Visual Studio 2012.
  
Программа установки Exchange 2013 устанавливает сборках, которые используются для разработки агента транспорта и регистрирует их в глобальный кэш сборок (GAC). Чтобы приступить к реализации агента транспорта, создайте ссылку на сборку Microsoft.Exchange.Data.Transport в проекте библиотеки классов.
  
## <a name="implementing-a-transport-agent"></a>Реализация агента транспорта
<a name="bk_implementationExample"> </a>

Следующий пример показывает минимальная реализация классы, производные от классов [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Если несколько агенты транспорта установлена и зарегистрирована для одного события, все агенты будет вызываться, даже если один агент удаляет всех получателей из почтового элемента. > Во избежание необработанных ошибок или непредсказуемое поведение, агента транспорта должен обрабатывать случаи, в которых число получателей для почтового элемента равно нулю. 
  
```cs
using System;
using System.Collections.Generic;
using System.Text;
using Microsoft.Exchange.Data.Transport;
using Microsoft.Exchange.Data.Transport.Smtp;
namespace MyAgents
{
    public sealed class MyAgentFactory : SmtpReceiveAgentFactory
    {
        public override SmtpReceiveAgent CreateAgent(SmtpServer server)
        {
            return new MyAgent();
        }
    }
    public class MyAgent : SmtpReceiveAgent
    {
        public MyAgent()
        {
            this.OnEndOfData += new EndOfDataEventHandler(MyEndOfDataHandler);
        }
        private void MyEndOfDataHandler (ReceiveMessageEventSource source, EndOfDataEventArgs e)
        {
            // The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject += " - this text appended by MyAgent";
        }
    }
}
```

```vb
Imports System
Imports System.Collections.Generic
Imports System.Text
Imports Microsoft.Exchange.Data.Transport
Imports Microsoft.Exchange.Data.Transport.Smtp
Namespace MyAgents
    NotInheritable Class MyAgentFactory
        Inherits SmtpReceiveAgentFactory
        Public Overrides Function CreateAgent(ByVal server as SmtpServer) As SmtpReceiveAgent
            Return New MyAgent
        End Function
    End Class
    Public Class MyAgent
        Inherits SmtpReceiveAgent
        Private Sub MyEndOfDataHandler(ByVal source As ReceiveMessageEventSource, ByVal e As EndOfDataEventArgs) Handles Me.OnEndOfData
            ' The following line appends text to the subject of the message that caused the event.
            e.MailItem.Message.Subject &amp;= e.MailItem.Message.Subject + " - this text appended by MyAgent"
        End Sub
    End Class
End Namespace
```

## <a name="installing-and-enabling-an-agent"></a>Установка и включение агента
<a name="bk_InstallEnable"> </a>

После компиляции агент для библиотеки DLL необходимо установить и настроить агент на сервере Exchange разработки. В командной консоли Exchange используйте командлет [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) для установки агента и командлет [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) для включения агента. Сведения о том, как использовать консоль управления Exchange можно [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Агенты транспорта имеют полный доступ ко всем сообщениям электронной почты, которые они возникать. Exchange 2013 не ограничивает поведение агента транспорта. Агенты транспорта, которые нестабильных или, которые содержат недостатков безопасности могут отрицательно повлиять на надежность и безопасность Exchange 2013. Таким образом следует устанавливать только агенты транспорта, которые полного доверия и, полностью проверялись. 
  
При использовании командлета **Install-TransportAgent** для установки агента управления Exchange сохраняет блокировки на сборку. Чтобы снять блокировку сборки, необходимо закрыть экземпляр Командная консоль Exchange, который используется для установки агента. Нельзя обновить ее до снятия блокировки. 
  
Следующем примере показано, как использовать консоль управления Exchange для установки и активации агента с именем MyAgent с помощью класса, производного от [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) с именем MyAgents.MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
В этом примере имя агента MyCustomAgent на сервере, на котором установлен агент. Следующий пример демонстрирует включение агента с именем MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Для управления агента транспорта в транспортной службе на сервере клиентского доступа, добавьте следующий параметр к команде: `-TransportService FrontEnd`. Например чтобы просмотреть агенты транспорта в транспортной службе, выполните следующую команду.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Дополнительные сведения об установке Включение и управление агента, видеть [Управление агенты транспорта](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>В этом разделе
<a name="bk_inthissection"> </a>

- [Создание агента транспорта RoutingAgent для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Создание агента транспорта SmtpReceiveAgent для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Создание агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>См. также

- [Транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Справочник по агента транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

