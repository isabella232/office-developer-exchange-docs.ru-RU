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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761293"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="f6cf2-103">Создание агенты транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="f6cf2-104">Сведения о создании настраиваемых транспортных агентов для Exchange 2013 и требования к системе для создания пользовательских агентов.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="f6cf2-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="f6cf2-106">Exchange Server 2013 включает в себя ряд агенты транспорта, которые можно использовать для обработки сообщений.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="f6cf2-107">С помощью сборки, входящие в состав Exchange, можно создавать свои собственные пользовательские агенты для выполнения определенных задач в соответствии с потребностями организации.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="f6cf2-108">Например можно использовать агент транспорта SmtpReceiveAgent для перехвата сообщений, которые получены с помощью протокола SMTP и процесс преобразования формата форматированного текста в теле сообщения.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="f6cf2-109">Агент транспорта RoutingAgent можно использовать для записи в журнал сообщений, проходящих через сервер на маршрут на другой сервер.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="f6cf2-110">Также можно создавать более сложные функции, которые позволяют использовать более одного типа агента.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="f6cf2-111">Например для создания антивирусного агента, можно реализовать SmtpReceiveAgent и RoutingAgent агента.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="f6cf2-112">Если компонент локальной сети, не поддерживает протокол SMTP, можно использовать агента транспорта DeliveryAgent для связи между сервером Exchange server и внешним компонентом.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="f6cf2-113">В этой статье описаны необходимые условия для и задачи, выполняемые при создании собственного агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="f6cf2-114">Сведения о создании агенты транспорта конкретных см [RoutingAgent агента транспорта для Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Создание SmtpReceiveAgent агента транспорта для Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), [Создать агента транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="f6cf2-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="f6cf2-115">Необходимые условия для создания агента транспорта</span><span class="sxs-lookup"><span data-stu-id="f6cf2-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="f6cf2-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="f6cf2-116"></span></span>

<span data-ttu-id="f6cf2-117">Ниже приведены компоненты, необходимые для реализации агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="f6cf2-118">Компьютер под управлением Exchange 2013, на котором работает служба транспорта переднего плана на сервере клиентского доступа или пограничный транспортный или транспортной службы на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="f6cf2-119">Сведения об архитектуре роли сервера в Exchange 2013 видеть [транспорта концепции агентов в Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="f6cf2-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="f6cf2-120">Следующие сборки для классов агента транспорта:</span><span class="sxs-lookup"><span data-stu-id="f6cf2-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="f6cf2-121">Microsoft.Exchange.Data.dll</span><span class="sxs-lookup"><span data-stu-id="f6cf2-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="f6cf2-122">Microsoft.Exchange.Data.Common.dll</span><span class="sxs-lookup"><span data-stu-id="f6cf2-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="f6cf2-123">Microsoft.Exchange.Transport.dll</span><span class="sxs-lookup"><span data-stu-id="f6cf2-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="f6cf2-124">.NET Framework 4.5</span><span class="sxs-lookup"><span data-stu-id="f6cf2-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="f6cf2-125">Мы также рекомендуем вам установить Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="f6cf2-126">Агенты транспорта можно реализовать с помощью Visual Basic .NET или C#.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="f6cf2-127">Создание ссылок на сборки</span><span class="sxs-lookup"><span data-stu-id="f6cf2-127">Referencing the assemblies</span></span>
<span data-ttu-id="f6cf2-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="f6cf2-128"></span></span>

<span data-ttu-id="f6cf2-129">Exchange 2013 предоставляет библиотеку классов, которые поддерживают расширение поведения транспорта Exchange.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="f6cf2-130">Эти классы требуют .NET Framework 4.5.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="f6cf2-131">Вы можете реализовать агенты транспорта на основе этих классов с помощью Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="f6cf2-132">Программа установки Exchange 2013 устанавливает сборках, которые используются для разработки агента транспорта и регистрирует их в глобальный кэш сборок (GAC).</span><span class="sxs-lookup"><span data-stu-id="f6cf2-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="f6cf2-133">Чтобы приступить к реализации агента транспорта, создайте ссылку на сборку Microsoft.Exchange.Data.Transport в проекте библиотеки классов.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="f6cf2-134">Реализация агента транспорта</span><span class="sxs-lookup"><span data-stu-id="f6cf2-134">Implementing a transport agent</span></span>
<span data-ttu-id="f6cf2-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="f6cf2-135"></span></span>

<span data-ttu-id="f6cf2-136">Следующий пример показывает минимальная реализация классы, производные от классов [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f6cf2-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="f6cf2-137">Если несколько агенты транспорта установлена и зарегистрирована для одного события, все агенты будет вызываться, даже если один агент удаляет всех получателей из почтового элемента.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="f6cf2-138">> Во избежание необработанных ошибок или непредсказуемое поведение, агента транспорта должен обрабатывать случаи, в которых число получателей для почтового элемента равно нулю.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
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

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="f6cf2-139">Установка и включение агента</span><span class="sxs-lookup"><span data-stu-id="f6cf2-139">Installing and enabling an agent</span></span>
<span data-ttu-id="f6cf2-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="f6cf2-140"></span></span>

<span data-ttu-id="f6cf2-141">После компиляции агент для библиотеки DLL необходимо установить и настроить агент на сервере Exchange разработки.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="f6cf2-142">В командной консоли Exchange используйте командлет [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) для установки агента и командлет [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) для включения агента.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-142">In the Exchange Management Shell, use the [Install-TransportAgent](http://technet.microsoft.com/en-us/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](http://technet.microsoft.com/en-us/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="f6cf2-143">Сведения о том, как использовать консоль управления Exchange можно [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="f6cf2-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/en-us/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="f6cf2-144">Агенты транспорта имеют полный доступ ко всем сообщениям электронной почты, которые они возникать.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="f6cf2-145">Exchange 2013 не ограничивает поведение агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="f6cf2-146">Агенты транспорта, которые нестабильных или, которые содержат недостатков безопасности могут отрицательно повлиять на надежность и безопасность Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="f6cf2-147">Таким образом следует устанавливать только агенты транспорта, которые полного доверия и, полностью проверялись.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="f6cf2-148">При использовании командлета **Install-TransportAgent** для установки агента управления Exchange сохраняет блокировки на сборку.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="f6cf2-149">Чтобы снять блокировку сборки, необходимо закрыть экземпляр Командная консоль Exchange, который используется для установки агента.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="f6cf2-150">Нельзя обновить ее до снятия блокировки.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="f6cf2-151">Следующем примере показано, как использовать консоль управления Exchange для установки и активации агента с именем MyAgent с помощью класса, производного от [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) с именем MyAgents.MyAgentFactory.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="f6cf2-152">В этом примере имя агента MyCustomAgent на сервере, на котором установлен агент.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="f6cf2-153">Следующий пример демонстрирует включение агента с именем MyCustomAgent.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="f6cf2-154">Для управления агента транспорта в транспортной службе на сервере клиентского доступа, добавьте следующий параметр к команде: `-TransportService FrontEnd`.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="f6cf2-155">Например чтобы просмотреть агенты транспорта в транспортной службе, выполните следующую команду.</span><span class="sxs-lookup"><span data-stu-id="f6cf2-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="f6cf2-156">Дополнительные сведения об установке Включение и управление агента, видеть [Управление агенты транспорта](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="f6cf2-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](http://technet.microsoft.com/en-us/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="f6cf2-157">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="f6cf2-157">In this section</span></span>
<span data-ttu-id="f6cf2-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="f6cf2-158"></span></span>

- [<span data-ttu-id="f6cf2-159">Создание агента транспорта RoutingAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="f6cf2-160">Создание агента транспорта SmtpReceiveAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="f6cf2-161">Создание агента транспорта DeliveryAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="f6cf2-162">См. также</span><span class="sxs-lookup"><span data-stu-id="f6cf2-162">See also</span></span>

- [<span data-ttu-id="f6cf2-163">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="f6cf2-164">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="f6cf2-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

