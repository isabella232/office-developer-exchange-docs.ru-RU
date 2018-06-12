---
title: Создание агента транспорта RoutingAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Узнайте, как создать настраиваемые агента транспорта RoutingAgent для использования с Exchange 2013.
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761299"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="70b5b-103">Создание агента транспорта RoutingAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="70b5b-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="70b5b-104">Узнайте, как создать настраиваемые агента транспорта RoutingAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="70b5b-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="70b5b-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="70b5b-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="70b5b-106">Связанные фрагменты кода и примеры приложений:</span><span class="sxs-lookup"><span data-stu-id="70b5b-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="70b5b-107">Exchange 2013: Создание агента транспорта пропускной способности ведения журнала</span><span class="sxs-lookup"><span data-stu-id="70b5b-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="70b5b-108">Классы, [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) и [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , базовые классы для агенты транспорта, которые предназначены для выполнения в службе транспорта на сервере почтовых ящиков Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="70b5b-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="70b5b-109">Класс [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) предоставляет события, указанные в следующей таблице, для которого может внедрить обработчики в вашей RoutingAgent агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="70b5b-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="70b5b-110">**В таблице 1. События класса RoutingAgent**</span><span class="sxs-lookup"><span data-stu-id="70b5b-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="70b5b-111">**Событие**</span><span class="sxs-lookup"><span data-stu-id="70b5b-111">**Event**</span></span>|<span data-ttu-id="70b5b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70b5b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70b5b-113">OnCategorizedMessage</span><span class="sxs-lookup"><span data-stu-id="70b5b-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="70b5b-114">Возникает после сервер выполняет преобразование содержимого, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="70b5b-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="70b5b-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="70b5b-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="70b5b-116">Возникает после устранения возможных всех получателей сообщения и перед маршрутизацией определяется.</span><span class="sxs-lookup"><span data-stu-id="70b5b-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="70b5b-117">OnRoutedMessage</span><span class="sxs-lookup"><span data-stu-id="70b5b-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="70b5b-118">Возникает после сервер перенаправляет сообщение до следующего прыжка и выполняет преобразование содержимого при необходимости.</span><span class="sxs-lookup"><span data-stu-id="70b5b-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="70b5b-119">Сервер может использовать дополнительные ресурсы для обработки каждого сообщения в событии [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) чем событие [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , так как сервер будет выполнять любые необходимые преобразования содержимого и определение следующего прыжка в маршрут для сообщения Перед выполнением кода в обработчик событий [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .</span><span class="sxs-lookup"><span data-stu-id="70b5b-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="70b5b-120">OnSubmittedMessage</span><span class="sxs-lookup"><span data-stu-id="70b5b-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="70b5b-121">Возникает после сообщения взят из очереди отправки.</span><span class="sxs-lookup"><span data-stu-id="70b5b-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="70b5b-122">Используйте событие [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , если агента транспорта RoutingAgent не требуется преобразования содержимого, разрешить получателей или маршрутизации данных.</span><span class="sxs-lookup"><span data-stu-id="70b5b-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="70b5b-123">Создание настраиваемых RoutingAgent агента транспорта</span><span class="sxs-lookup"><span data-stu-id="70b5b-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="70b5b-124">Следующая процедура описывается создание пользовательских RoutingAgent агента транспорта.</span><span class="sxs-lookup"><span data-stu-id="70b5b-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="70b5b-125">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="70b5b-125">To create the transport agent</span></span>

1. <span data-ttu-id="70b5b-126">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="70b5b-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="70b5b-127">Эти пространства имен можно найти на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="70b5b-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="70b5b-128">Добавление ссылки на следующие пространства имен, будет обеспечивает доступ к членам [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) также другие классы, используемые в [Exchange 2013: создание агента транспорта ведения журнала пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) образца.</span><span class="sxs-lookup"><span data-stu-id="70b5b-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="70b5b-129">Реализация производного класса для класса [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="70b5b-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="70b5b-130">Этот код будет создать экземпляр производного класса и переопределить метод **CreateAgent** для создания экземпляра настраиваемого агент.</span><span class="sxs-lookup"><span data-stu-id="70b5b-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="70b5b-131">Дополнительные методы, такие как **Закрытие**, можно также переопределить в этом классе для выполнения пользовательского кода.</span><span class="sxs-lookup"><span data-stu-id="70b5b-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="70b5b-132">Определение агента.</span><span class="sxs-lookup"><span data-stu-id="70b5b-132">Define your agent.</span></span>
    
   ```cs
      public class BandwidthLogger : RoutingAgent
      {
          // Your custom code goes here
          public BandwidthLogger(SmtpServer server)
          {
              Debug.WriteLine(logPrefix + "Agent constructor");
              this.server = server;
              this.OnSubmittedMessage += SubmittedMessage;
              this.OnRoutedMessage += RoutedMessage;
          }
      }
  
   ```

   <span data-ttu-id="70b5b-133">После определения класса агента вы можно добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="70b5b-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="70b5b-134">В этом примере два события [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)перенаправляются к настраиваемым обработчикам событий.</span><span class="sxs-lookup"><span data-stu-id="70b5b-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="70b5b-135">См. также</span><span class="sxs-lookup"><span data-stu-id="70b5b-135">See also</span></span>

- [<span data-ttu-id="70b5b-136">Транспорта концепции агентов в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="70b5b-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="70b5b-137">Справочник по агента транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="70b5b-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="70b5b-138">RoutingAgentFactory</span><span class="sxs-lookup"><span data-stu-id="70b5b-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="70b5b-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="70b5b-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

