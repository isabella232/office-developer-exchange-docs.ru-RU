---
title: Создание транспортных агентов Exchange 2013 г.
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Сведения о создании специальных транспортных агентов для Exchange 2013 г., а также системные требования к созданию настраиваемой агенту.
ms.openlocfilehash: ea5ae1fab85fde781cb365a21b7a40ccd52955b3
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520957"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Создание транспортных агентов Exchange 2013 г.

Сведения о создании специальных транспортных агентов для Exchange 2013 г., а также системные требования к созданию настраиваемой агенту.
  
**Применяется к:** Exchange Server 2013 г.
  
Exchange Server 2013 г. включает несколько транспортных агентов, которые можно использовать для обработки сообщений. Используя сборки, которые Exchange, можно создать собственные настраиваемые агенты для выполнения определенных задач в соответствии с потребностями организации. Например, транспортный агент SmtpReceiveAgent можно использовать для перехвата сообщений, полученных с помощью протокола SMTP, и обработки сообщения для преобразования формата тела в предварительно составленный текст. Транспортный агент RoutingAgent можно использовать для входа сообщений, которые передаются через сервер по маршруту на другой сервер. Вы также можете создать более сложные функции, которые используют несколько типов агентов. Например, для создания антивирусного агента можно реализовать SmtpReceiveAgent и агент RoutingAgent. Если в сети есть компонент, который не поддерживает протокол SMTP, можно использовать транспортный агент DeliveryAgent для обработки связи между Exchange сервером и внешним компонентом. 
  
В этой статье приводится информация о необходимых для создания собственного транспортного агента и задачах. Сведения о создании специальных транспортных агентов см. в статью Создание транспортного агента [RoutingAgent за Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)г., создание транспортного агента [SmtpReceiveAgent для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)г. и создание транспортного [агента DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)г.
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Необходимые условия для создания транспортного агента
<a name="bk_prerequisites"> </a>

Для реализации транспортного агента необходимо выполнить следующие условия:
  
- Компьютер, работающий Exchange 2013 г., который работает службой переднего транспорта на сервере клиентского доступа или на краевом транспортном сервере или транспортной службе на сервере почтовых ящиков. Сведения об архитектуре роли сервера в Exchange 2013 г. см. в Exchange [2013](transport-agent-concepts-in-exchange-2013.md)г. .
    
- Следующие сборки для классов транспортных агентов:
    
  - Microsoft.Exchange.Data.dll
    
  - Microsoft.Exchange.Data.Common.dll
    
  - Microsoft.Exchange.Transport.dll
    
- The платформа .NET Framework 4.5
    
Мы также рекомендуем установить Visual Studio 2012. Транспортные агенты можно реализовать с помощью Visual Basic .NET или C#.
  
## <a name="referencing-the-assemblies"></a>Ссылки на сборки
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 г. предоставляет библиотеку классов, которые поддерживают расширение Exchange транспорта. Для этих классов требуется платформа .NET Framework 4.5. На основе этих классов можно реализовать транспортные агенты с помощью Visual Studio 2012 г.
  
Установщик Exchange 2013 г. устанавливает сборки, используемые для разработки транспортных агентов, и регистрирует их в глобальном кэше сборки (GAC). Чтобы приступить к реализации транспортного агента, создайте ссылку на Microsoft. Exchange. Сборка Data.Transport в проекте библиотеки классов.
  
## <a name="implementing-a-transport-agent"></a>Реализация транспортного агента
<a name="bk_implementationExample"> </a>

В следующем примере показана минимальная реализация классов, вытекающих из классов [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent.](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) 
  
> [!CAUTION]
> Если для одного события установлено и зарегистрировано несколько транспортных агентов, все агенты будут вызываться, даже если один агент удаляет всех получателей из почтового элемента. >, чтобы избежать ненаблюдаемой ошибки или непредсказуемого поведения, транспортный агент должен обрабатывать случаи, в которых получатель рассчитывает на элемент почты равно нулю. 
  
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

После компиляции агента в DLL необходимо установить и включить его на сервере разработки Exchange. В Exchange для установки агента используйте команды [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) и средство [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) для установки агента. Сведения об использовании оболочки управления Exchange см. в Exchange Server [PowerShell (Exchange Management Shell).](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps)
  
> [!CAUTION]
> Агенты транспорта имеют полный доступ ко всем сообщениям электронной почты, которые они обнаруживают. Exchange 2013 г. не ограничивает поведение транспортного агента. Агенты транспорта, которые являются неустойчивыми или содержат недостатки безопасности, могут повлиять на стабильность и безопасность Exchange 2013 г. Поэтому следует установить только транспортные агенты, которые полностью доверяли и которые были полностью протестированы. 
  
При установке агента с помощью команды **Install-TransportAgent** Exchange управленческой оболочки сохраняется блокировка сборки. Чтобы освободить блокировку сборки, необходимо закрыть экземпляр Exchange, который использовался для установки агента. Вы не сможете обновить сборку, пока не отпустите блокировку. 
  
В следующем примере показано, как использовать оболочку управления Exchange для установки агента с именем MyAgent, используя класс, полученный из [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) с именем MyAgents.MyAgentFactory. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
В этом примере именуется агент MyCustomAgent на сервере, на котором установлен агент. В следующем примере показано, как включить агент с именем MyCustomAgent.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Чтобы управлять транспортным агентом в передней транспортной службе на сервере клиентского доступа, добавьте в команду следующее значение:  `-TransportService FrontEnd` . Например, чтобы просмотреть агенты транспорта в передней транспортной службе, запустите следующую команду.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Дополнительные сведения об установке, включив и управляя вашим агентом, см. в этой [информации.](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx)
  
## <a name="in-this-section"></a>В этом разделе:
<a name="bk_inthissection"> </a>

- [Создание транспортного агента RoutingAgent для Exchange 2013 г.](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Создание транспортного агента SmtpReceiveAgent для Exchange 2013 г.](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Создание транспортного агента DeliveryAgent для Exchange 2013 г.](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>См. также

- [Концепции транспортного агента в Exchange 2013 г.](transport-agent-concepts-in-exchange-2013.md)   
- [Ссылка агента транспорта на Exchange 2013 г.](transport-agent-reference-for-exchange-2013.md)
    

