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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462376"
---
# <a name="creating-transport-agents-for-exchange-2013"></a><span data-ttu-id="129f1-103">Создание агентов транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-103">Creating transport agents for Exchange 2013</span></span>

<span data-ttu-id="129f1-104">Сведения о том, как создавать настраиваемые агенты транспорта для Exchange 2013, а также требования к системе для создания настраиваемого агента.</span><span class="sxs-lookup"><span data-stu-id="129f1-104">Find information about how to create custom transport agents for Exchange 2013, and the system requirements for creating a custom agent.</span></span>
  
<span data-ttu-id="129f1-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="129f1-106">Exchange Server 2013 включает несколько агентов транспорта, которые можно использовать для обработки сообщений.</span><span class="sxs-lookup"><span data-stu-id="129f1-106">Exchange Server 2013 includes several transport agents that you can use to process messages.</span></span> <span data-ttu-id="129f1-107">С помощью сборок, поставляемых с Exchange, вы можете создавать собственные агенты для выполнения определенных задач в соответствии с потребностями Организации.</span><span class="sxs-lookup"><span data-stu-id="129f1-107">By using the assemblies that come with Exchange, you can create your own custom agents to perform specific tasks according to the needs of your organization.</span></span> <span data-ttu-id="129f1-108">Например, вы можете использовать агент транспорта SmtpReceiveAgent для перехвата сообщений, полученных с помощью протокола SMTP, и обработки сообщения для преобразования формата текста, содержащего предварительно отформатированный текст.</span><span class="sxs-lookup"><span data-stu-id="129f1-108">For example, you can use an SmtpReceiveAgent transport agent to intercept messages that are received via the SMTP protocol and process the message to convert the format of the body to contain preformatted text.</span></span> <span data-ttu-id="129f1-109">Вы можете использовать агент транспорта RoutingAgent для записи сообщений, которые проходят через сервер, по маршруту на другой сервер.</span><span class="sxs-lookup"><span data-stu-id="129f1-109">You can use a RoutingAgent transport agent to log the messages that pass through the server on route to another server.</span></span> <span data-ttu-id="129f1-110">Кроме того, вы можете создавать более сложные функции, использующие более одного типа агентов.</span><span class="sxs-lookup"><span data-stu-id="129f1-110">You can also create more complex features that make use of more than one type of agent.</span></span> <span data-ttu-id="129f1-111">Например, для создания антивирусного агента можно реализовать SmtpReceiveAgent и агент RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="129f1-111">For example, to create an antivirus agent, you can implement an SmtpReceiveAgent and a RoutingAgent agent.</span></span> <span data-ttu-id="129f1-112">Если в вашей сети есть компонент, который не поддерживает протокол SMTP, можно использовать агент транспорта DeliveryAgent для обработки связи между сервером Exchange и внешним компонентом.</span><span class="sxs-lookup"><span data-stu-id="129f1-112">If you have a component on your network that does not support the SMTP protocol, you can use a DeliveryAgent transport agent to handle the communication between your Exchange server and your external component.</span></span> 
  
<span data-ttu-id="129f1-113">В этой статье приводятся сведения о необходимых условиях и задачах, связанных с созданием собственного агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="129f1-113">This article provides information about the prerequisites for and tasks involved in creating your own transport agent.</span></span> <span data-ttu-id="129f1-114">Сведения о создании определенных агентов транспорта можно найти [в статье Create a RoutingAgent Transport Transport Agent for exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create a SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), и [Создайте агент транспорта DeliveryAgent для Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="129f1-114">For information about creating specific transport agents, see [Create a RoutingAgent transport agent for Exchange 2013](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md), [Create an SmtpReceiveAgent transport agent for Exchange 2013](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md), and [Create a DeliveryAgent transport agent for Exchange 2013](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md).</span></span>
  
## <a name="prerequisites-for-creating-a-transport-agent"></a><span data-ttu-id="129f1-115">Необходимые условия для создания агента транспорта</span><span class="sxs-lookup"><span data-stu-id="129f1-115">Prerequisites for creating a transport agent</span></span>
<span data-ttu-id="129f1-116"><a name="bk_prerequisites"> </a></span><span class="sxs-lookup"><span data-stu-id="129f1-116"><a name="bk_prerequisites"> </a></span></span>

<span data-ttu-id="129f1-117">Ниже приведены необходимые условия, необходимые для реализации агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="129f1-117">The following are the prerequisites that you need in order to implement a transport agent:</span></span>
  
- <span data-ttu-id="129f1-118">Компьютер под управлением Exchange 2013, на котором запущена служба транспорта переднего плана на сервере клиентского доступа или пограничном транспортном сервере или на транспортной службе на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="129f1-118">A computer running Exchange 2013 that is running the Front End Transport service on a Client Access or Edge Transport server, or the Transport service on a Mailbox server.</span></span> <span data-ttu-id="129f1-119">Сведения об архитектуре ролей сервера в Exchange 2013 приведены в статье [Основные понятия агента транспорта в exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span><span class="sxs-lookup"><span data-stu-id="129f1-119">For information about the server role architecture in Exchange 2013, see [Transport agent concepts in Exchange 2013](transport-agent-concepts-in-exchange-2013.md).</span></span>
    
- <span data-ttu-id="129f1-120">Следующие сборки для классов агентов транспорта:</span><span class="sxs-lookup"><span data-stu-id="129f1-120">The following assemblies for the transport agent classes:</span></span>
    
  - <span data-ttu-id="129f1-121">Microsoft. Exchange. Data. dll</span><span class="sxs-lookup"><span data-stu-id="129f1-121">Microsoft.Exchange.Data.dll</span></span>
    
  - <span data-ttu-id="129f1-122">Microsoft. Exchange. Data. Common. dll</span><span class="sxs-lookup"><span data-stu-id="129f1-122">Microsoft.Exchange.Data.Common.dll</span></span>
    
  - <span data-ttu-id="129f1-123">Microsoft. Exchange. Transport. dll</span><span class="sxs-lookup"><span data-stu-id="129f1-123">Microsoft.Exchange.Transport.dll</span></span>
    
- <span data-ttu-id="129f1-124">Платформа .NET Framework 4,5</span><span class="sxs-lookup"><span data-stu-id="129f1-124">The .NET Framework 4.5</span></span>
    
<span data-ttu-id="129f1-125">Кроме того, рекомендуется установить Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="129f1-125">We also recommend that you install Visual Studio 2012.</span></span> <span data-ttu-id="129f1-126">Вы можете реализовать агенты транспорта с помощью Visual Basic .NET или C#.</span><span class="sxs-lookup"><span data-stu-id="129f1-126">You can implement transport agents by using either Visual Basic .NET or C#.</span></span>
  
## <a name="referencing-the-assemblies"></a><span data-ttu-id="129f1-127">Создание ссылок на сборки</span><span class="sxs-lookup"><span data-stu-id="129f1-127">Referencing the assemblies</span></span>
<span data-ttu-id="129f1-128"><a name="bk_ReferenceAssemblies"> </a></span><span class="sxs-lookup"><span data-stu-id="129f1-128"><a name="bk_ReferenceAssemblies"> </a></span></span>

<span data-ttu-id="129f1-129">Exchange 2013 предоставляет библиотеку классов, поддерживающих расширение поведения транспорта Exchange.</span><span class="sxs-lookup"><span data-stu-id="129f1-129">Exchange 2013 provides a library of classes that support the extension of Exchange transport behavior.</span></span> <span data-ttu-id="129f1-130">Для этих классов требуется .NET Framework 4,5.</span><span class="sxs-lookup"><span data-stu-id="129f1-130">These classes require the .NET Framework 4.5.</span></span> <span data-ttu-id="129f1-131">Вы можете реализовать агенты транспорта на основе этих классов с помощью Visual Studio 2012.</span><span class="sxs-lookup"><span data-stu-id="129f1-131">You can implement transport agents based on these classes by using Visual Studio 2012.</span></span>
  
<span data-ttu-id="129f1-132">Установщик Exchange 2013 устанавливает сборки, используемые для разработки агента транспорта, и регистрирует их в глобальном кэше сборок (GAC).</span><span class="sxs-lookup"><span data-stu-id="129f1-132">The Exchange 2013 installer installs assemblies that are used for transport agent development and registers them in the global assembly cache (GAC).</span></span> <span data-ttu-id="129f1-133">Чтобы начать реализацию агента транспорта, создайте ссылку на сборку Microsoft. Exchange. Data. Transport в проекте библиотеки классов.</span><span class="sxs-lookup"><span data-stu-id="129f1-133">To begin implementing a transport agent, create a reference to the Microsoft.Exchange.Data.Transport assembly in a class library project.</span></span>
  
## <a name="implementing-a-transport-agent"></a><span data-ttu-id="129f1-134">Реализация агента транспорта</span><span class="sxs-lookup"><span data-stu-id="129f1-134">Implementing a transport agent</span></span>
<span data-ttu-id="129f1-135"><a name="bk_implementationExample"> </a></span><span class="sxs-lookup"><span data-stu-id="129f1-135"><a name="bk_implementationExample"> </a></span></span>

<span data-ttu-id="129f1-136">В следующем примере показана минимальная реализация классов, производных от классов [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) и [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) .</span><span class="sxs-lookup"><span data-stu-id="129f1-136">The following example shows a minimal implementation of classes that derive from the [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) and [SmtpReceiveAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgent.aspx) classes.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="129f1-137">Если для одного события установлено и зарегистрировано несколько агентов транспорта, будут вызываться все агенты, даже если один агент удаляет всех получателей из почтового элемента.</span><span class="sxs-lookup"><span data-stu-id="129f1-137">If multiple transport agents are installed and registered for the same event, all agents will be invoked, even if one agent removes all the recipients from a mail item.</span></span> <span data-ttu-id="129f1-138">> чтобы избежать необработанных ошибок или непредсказуемого поведения, агент транспорта должен обрабатывать случаи, в которых количество получателей почтового элемента равно нулю.</span><span class="sxs-lookup"><span data-stu-id="129f1-138">> To avoid unhandled errors or unpredictable behavior, your transport agent should handle cases in which the recipient count on a mail item is equal to zero.</span></span> 
  
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

## <a name="installing-and-enabling-an-agent"></a><span data-ttu-id="129f1-139">Установка и включение агента</span><span class="sxs-lookup"><span data-stu-id="129f1-139">Installing and enabling an agent</span></span>
<span data-ttu-id="129f1-140"><a name="bk_InstallEnable"> </a></span><span class="sxs-lookup"><span data-stu-id="129f1-140"><a name="bk_InstallEnable"> </a></span></span>

<span data-ttu-id="129f1-141">После компиляции агента в библиотеку DLL необходимо установить и включить агент на сервере Exchange Development Server.</span><span class="sxs-lookup"><span data-stu-id="129f1-141">After you compile your agent to a DLL, you must install and enable the agent on your development Exchange server.</span></span> <span data-ttu-id="129f1-142">В командной консоли Exchange с помощью командлета [Install – TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) установите агент, а командлет [Enable – TransportAgent —](https://technet.microsoft.com/library/bb124921.aspx) для включения агента.</span><span class="sxs-lookup"><span data-stu-id="129f1-142">In the Exchange Management Shell, use the [Install-TransportAgent](https://technet.microsoft.com/library/aa997998.aspx) cmdlet to install your agent, and the [Enable-TransportAgent](https://technet.microsoft.com/library/bb124921.aspx) cmdlet to enable your agent.</span></span> <span data-ttu-id="129f1-143">Сведения о том, как использовать командную консоль Exchange, можно найти в статье [Exchange Server PowerShell (Командная консоль Exchange)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span><span class="sxs-lookup"><span data-stu-id="129f1-143">For information about how to use the Exchange Management Shell, see [Exchange Server PowerShell (Exchange Management Shell)](https://docs.microsoft.com/powershell/exchange/exchange-server/exchange-management-shell?view=exchange-ps).</span></span>
  
> [!CAUTION]
> <span data-ttu-id="129f1-144">Агенты транспорта имеют полный доступ ко всем сообщениям электронной почты, которые они обнаруживают.</span><span class="sxs-lookup"><span data-stu-id="129f1-144">Transport agents have full access to all email messages that they encounter.</span></span> <span data-ttu-id="129f1-145">Exchange 2013 не ограничивает поведение агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="129f1-145">Exchange 2013 does not restrict the behavior of a transport agent.</span></span> <span data-ttu-id="129f1-146">Агенты транспорта, которые работают нестабильно или содержат изъяны безопасности, могут повлиять на стабильность и безопасность Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="129f1-146">Transport agents that are unstable or that contain security flaws might affect the stability and security of Exchange 2013.</span></span> <span data-ttu-id="129f1-147">Таким образом, следует устанавливать только те агенты транспорта, которые полностью доверенны и полностью протестированы.</span><span class="sxs-lookup"><span data-stu-id="129f1-147">Therefore, you should only install transport agents that you fully trust and that have been fully tested.</span></span> 
  
<span data-ttu-id="129f1-148">При использовании командлета **Install – TransportAgent** для установки агента консоль управления Exchange сохраняет блокировку сборки.</span><span class="sxs-lookup"><span data-stu-id="129f1-148">When you use the **Install-TransportAgent** cmdlet to install an agent, the Exchange Management Shell keeps a lock on the assembly.</span></span> <span data-ttu-id="129f1-149">Чтобы снять блокировку сборки, необходимо закрыть экземпляр командной консоли Exchange, который использовался для установки агента.</span><span class="sxs-lookup"><span data-stu-id="129f1-149">To release the lock on the assembly, you must close the instance of the Exchange Management Shell that you used to install the agent.</span></span> <span data-ttu-id="129f1-150">Вы не сможете обновить сборку, пока не освободите блокировку.</span><span class="sxs-lookup"><span data-stu-id="129f1-150">You will be unable to update the assembly until you release the lock.</span></span> 
  
<span data-ttu-id="129f1-151">В приведенном ниже примере показано, как использовать командную консоль Exchange для установки и включения агента с именем Мяжент с помощью класса, производного от [смтпрецеивеажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) с именем Мяжентс. мяжентфактори.</span><span class="sxs-lookup"><span data-stu-id="129f1-151">The following example shows how to use the Exchange Management Shell to install and enable an agent named MyAgent by using a class derived from [SmtpReceiveAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Smtp.SmtpReceiveAgentFactory.aspx) named MyAgents.MyAgentFactory.</span></span> 
  
 `Install-TransportAgent -Name "MyCustomAgent" -TransportAgentFactory "MyAgents.MyAgentFactory" -AssemblyPath "C:\myagents\MyAgent.dll"`
  
<span data-ttu-id="129f1-152">В этом примере имя агента Микустомажент на сервере, на котором установлен агент.</span><span class="sxs-lookup"><span data-stu-id="129f1-152">This example names the agent MyCustomAgent on the server on which the agent is installed.</span></span> <span data-ttu-id="129f1-153">В приведенном ниже примере показано, как включить агент с именем Микустомажент.</span><span class="sxs-lookup"><span data-stu-id="129f1-153">The following example shows how to enable the agent named MyCustomAgent.</span></span>
  
 `Enable-TransportAgent -Name "MyCustomAgent"`
  
<span data-ttu-id="129f1-154">Чтобы управлять агентом транспорта в транспортной службе переднего плана на сервере клиентского доступа, добавьте в команду следующее значение: `-TransportService FrontEnd` .</span><span class="sxs-lookup"><span data-stu-id="129f1-154">To manage a transport agent in the Front End Transport service on a Client Access server, add the following value to the command:  `-TransportService FrontEnd`.</span></span> <span data-ttu-id="129f1-155">Например, чтобы просмотреть агенты транспорта в службе транспорта переднего плана, выполните следующую команду.</span><span class="sxs-lookup"><span data-stu-id="129f1-155">For example, to view the transport agents in the Front End Transport service, run the following command.</span></span>
  
 `Get-TransportAgent -TransportService FrontEnd`
  
<span data-ttu-id="129f1-156">Дополнительные сведения об установке и управлении агентом, а так же об этом можно узнать в разделе [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="129f1-156">For more information about installing, enabling, and managing your agent, see [Manage Transport Agents](https://technet.microsoft.com/library/bb125175%28v=exchg.150%29.aspx).</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="129f1-157">В этой статье</span><span class="sxs-lookup"><span data-stu-id="129f1-157">In this section</span></span>
<span data-ttu-id="129f1-158"><a name="bk_inthissection"> </a></span><span class="sxs-lookup"><span data-stu-id="129f1-158"><a name="bk_inthissection"> </a></span></span>

- [<span data-ttu-id="129f1-159">Создание агента транспорта RoutingAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-159">Create a RoutingAgent transport agent for Exchange 2013</span></span>](how-to-create-a-routingagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="129f1-160">Создание агента транспорта SmtpReceiveAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-160">Create an SmtpReceiveAgent transport agent for Exchange 2013</span></span>](how-to-create-an-smtpreceiveagent-transport-agent-for-exchange-2013.md)
    
- [<span data-ttu-id="129f1-161">Создание агента транспорта DeliveryAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-161">Create a DeliveryAgent transport agent for Exchange 2013</span></span>](how-to-create-a-deliveryagent-transport-agent-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="129f1-162">См. также</span><span class="sxs-lookup"><span data-stu-id="129f1-162">See also</span></span>

- [<span data-ttu-id="129f1-163">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-163">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)   
- [<span data-ttu-id="129f1-164">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="129f1-164">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)
    

