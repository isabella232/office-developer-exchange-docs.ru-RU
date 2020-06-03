---
title: Создание агентов транспорта для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d291ab78-7cdd-4dbe-a5f4-9dc8e9650a33
description: Сведения о том, как создавать настраиваемые агенты транспорта для Exchange 2013, а также требования к системе для создания настраиваемого агента.
ms.openlocfilehash: cb1cd180817524fe29a100a48d90444c75a77510
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462376"
---
# <a name="creating-transport-agents-for-exchange-2013"></a>Создание агентов транспорта для Exchange 2013

Сведения о том, как создавать настраиваемые агенты транспорта для Exchange 2013, а также требования к системе для создания настраиваемого агента.
  
**Применимо к:** Exchange Server 2013
  
Exchange Server 2013 включает несколько агентов транспорта, которые можно использовать для обработки сообщений. С помощью сборок, поставляемых с Exchange, вы можете создавать собственные агенты для выполнения определенных задач в соответствии с потребностями Организации. Например, вы можете использовать агент транспорта SmtpReceiveAgent для перехвата сообщений, полученных с помощью протокола SMTP, и обработки сообщения для преобразования формата текста, содержащего предварительно отформатированный текст. Вы можете использовать агент транспорта RoutingAgent для записи сообщений, которые проходят через сервер, по маршруту на другой сервер. Кроме того, вы можете создавать более сложные функции, использующие более одного типа агентов. Например, для создания антивирусного агента можно реализовать SmtpReceiveAgent и агент RoutingAgent. Если в вашей сети есть компонент, который не поддерживает протокол SMTP, можно использовать агент транспорта DeliveryAgent для обработки связи между сервером Exchange и внешним компонентом. 
  
В этой статье приводятся сведения о необходимых условиях и задачах, связанных с созданием собственного агента транспорта. Сведения о создании определенных агентов транспорта можно найти [в статье Create a RoutingAgent Transport Transport Agent for exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create a SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), и [Создайте агент транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).
  
## <a name="prerequisites-for-creating-a-transport-agent"></a>Необходимые условия для создания агента транспорта
<a name="bk_prerequisites"> </a>

Ниже приведены необходимые условия, необходимые для реализации агента транспорта.
  
- Компьютер под управлением Exchange 2013, на котором запущена служба транспорта переднего плана на сервере клиентского доступа или пограничном транспортном сервере или на транспортной службе на сервере почтовых ящиков. Сведения об архитектуре ролей сервера в Exchange 2013 приведены в статье [Основные понятия агента транспорта в exchange 2013](transport-agent-concepts-in-exchange-2013.md).
    
- Следующие сборки для классов агентов транспорта:
    
  - Microsoft. Exchange. Data. dll
    
  - Microsoft. Exchange. Data. Common. dll
    
  - Microsoft. Exchange. Transport. dll
    
- Платформа .NET Framework 4,5
    
Кроме того, рекомендуется установить Visual Studio 2012. Вы можете реализовать агенты транспорта с помощью Visual Basic .NET или C#.
  
## <a name="referencing-the-assemblies"></a>Создание ссылок на сборки
<a name="bk_ReferenceAssemblies"> </a>

Exchange 2013 предоставляет библиотеку классов, поддерживающих расширение поведения транспорта Exchange. Для этих классов требуется .NET Framework 4,5. Вы можете реализовать агенты транспорта на основе этих классов с помощью Visual Studio 2012.
  
Установщик Exchange 2013 устанавливает сборки, используемые для разработки агента транспорта, и регистрирует их в глобальном кэше сборок (GAC). Чтобы начать реализацию агента транспорта, создайте ссылку на сборку Microsoft. Exchange. Data. Transport в проекте библиотеки классов.
  
## <a name="implementing-a-transport-agent"></a>Реализация агента транспорта
<a name="bk_implementationExample"> </a>

В следующем примере показана минимальная реализация классов, производных от классов [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) . 
  
> [!CAUTION]
> Если для одного события установлено и зарегистрировано несколько агентов транспорта, будут вызываться все агенты, даже если один агент удаляет всех получателей из почтового элемента. > чтобы избежать необработанных ошибок или непредсказуемого поведения, агент транспорта должен обрабатывать случаи, в которых количество получателей почтового элемента равно нулю. 
  
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

После компиляции агента в библиотеку DLL необходимо установить и включить агент на сервере Exchange Development Server. В командной консоли Exchange с помощью командлета [Install – TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) установите агент, а командлет [Enable – TransportAgent —](https://technet.microsoft.com/library/bb124921.aspx) для включения агента. Сведения о том, как использовать командную консоль Exchange, можно найти в статье [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).
  
> [!CAUTION]
> Агенты транспорта имеют полный доступ ко всем сообщениям электронной почты, которые они обнаруживают. Exchange 2013 не ограничивает поведение агента транспорта. Агенты транспорта, которые работают нестабильно или содержат изъяны безопасности, могут повлиять на стабильность и безопасность Exchange 2013. Таким образом, следует устанавливать только те агенты транспорта, которые полностью доверенны и полностью протестированы. 
  
При использовании командлета **Install – TransportAgent** для установки агента консоль управления Exchange сохраняет блокировку сборки. Чтобы снять блокировку сборки, необходимо закрыть экземпляр командной консоли Exchange, который использовался для установки агента. Вы не сможете обновить сборку, пока не освободите блокировку. 
  
В приведенном ниже примере показано, как использовать командную консоль Exchange для установки и включения агента с именем Мяжент с помощью класса, производного от [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) с именем Мяжентс. мяжентфактори. 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
В этом примере имя агента Микустомажент на сервере, на котором установлен агент. В приведенном ниже примере показано, как включить агент с именем Микустомажент.
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
Чтобы управлять агентом транспорта в транспортной службе переднего плана на сервере клиентского доступа, добавьте в команду следующее значение: `-TransportService FrontEnd` . Например, чтобы просмотреть агенты транспорта в службе транспорта переднего плана, выполните следующую команду.
  
 `Get-TransportAgent -TransportService FrontEnd`
  
Дополнительные сведения об установке и управлении агентом, а так же об этом можно узнать в разделе [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).
  
## <a name="in-this-section"></a>В этой статье
<a name="bk_inthissection"> </a>

- [Создание агента транспорта RoutingAgent для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [Создание агента транспорта SmtpReceiveAgent для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [Создание агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a>См. также

- [Основные понятия, связанные с агентами транспорта в Exchange 2013](transport-agent-concepts-in-exchange-2013.md)   
- [Справочник по агентам транспорта для Exchange 2013](transport-agent-reference-for-exchange-2013.md)
    

