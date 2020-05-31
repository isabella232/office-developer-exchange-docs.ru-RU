---
title: Создание агента транспорта RoutingAgent для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f0e745f-9289-4f31-8877-926692a8c133
description: Узнайте, как создать настраиваемый агент транспорта RoutingAgent для использования с Exchange 2013.
ms.openlocfilehash: d07f68494acd26940a4837bbbfc7a0505114bd20
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761299"
---
# <a name="create-a-routingagent-transport-agent-for-exchange-2013"></a><span data-ttu-id="00754-103">Создание агента транспорта RoutingAgent для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="00754-103">Create a RoutingAgent transport agent for Exchange 2013</span></span>

<span data-ttu-id="00754-104">Узнайте, как создать настраиваемый агент транспорта RoutingAgent для использования с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="00754-104">Find out how to create a custom RoutingAgent transport agent to use with Exchange 2013.</span></span>
  
<span data-ttu-id="00754-105">**Применимо к:** Exchange Server 2013</span><span class="sxs-lookup"><span data-stu-id="00754-105">**Applies to:** Exchange Server 2013</span></span>
  
<span data-ttu-id="00754-106">Связанные фрагменты кода и примеры приложений:</span><span class="sxs-lookup"><span data-stu-id="00754-106">Related code snippets and sample apps:</span></span>

- [<span data-ttu-id="00754-107">Exchange 2013: создание агента транспорта журналов пропускной способности</span><span class="sxs-lookup"><span data-stu-id="00754-107">Exchange 2013: Build a bandwidth logging transport agent</span></span>](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa)
  
<span data-ttu-id="00754-108">Классы [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) и [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) являются базовыми классами для агентов транспорта, которые предназначены для запуска в службе транспорта на сервере почтовых ящиков Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="00754-108">The [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) and [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) classes are the base classes for transport agents that are designed to run on the transport service on an Exchange Server 2013 Mailbox server.</span></span> <span data-ttu-id="00754-109">Класс [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) предоставляет события, перечисленные в следующей таблице, для которых вы можете реализовать обработчики в агенте транспорта RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="00754-109">The [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) class provides the events listed in the following table for which you might implement handlers in your RoutingAgent transport agent.</span></span> 
  
<span data-ttu-id="00754-110">**Таблица 1. События класса RoutingAgent**</span><span class="sxs-lookup"><span data-stu-id="00754-110">**Table 1. RoutingAgent class events**</span></span>

|<span data-ttu-id="00754-111">**Event**</span><span class="sxs-lookup"><span data-stu-id="00754-111">**Event**</span></span>|<span data-ttu-id="00754-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00754-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00754-113">онкатегоризедмессаже</span><span class="sxs-lookup"><span data-stu-id="00754-113">OnCategorizedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnCategorizedMessage.aspx) <br/> |<span data-ttu-id="00754-114">Происходит, когда сервер выполняет преобразование контента, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="00754-114">Occurs after the server performs content conversion, if it is required.</span></span>  <br/> |
|[<span data-ttu-id="00754-115">OnResolvedMessage</span><span class="sxs-lookup"><span data-stu-id="00754-115">OnResolvedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnResolvedMessage.aspx) <br/> |<span data-ttu-id="00754-116">Возникает после того, как все получатели сообщения были разрешены и до того, как будет определена маршрутизация.</span><span class="sxs-lookup"><span data-stu-id="00754-116">Occurs after all the recipients of the message have been resolved and before routing is determined.</span></span>  <br/> |
|[<span data-ttu-id="00754-117">онраутедмессаже</span><span class="sxs-lookup"><span data-stu-id="00754-117">OnRoutedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) <br/> |<span data-ttu-id="00754-118">Возникает после того, как сервер направляет сообщение на следующий прыжок и выполняет преобразование контента, если это необходимо.</span><span class="sxs-lookup"><span data-stu-id="00754-118">Occurs after the server routes the message to the next hop and performs content conversion, if required.</span></span> <span data-ttu-id="00754-119">Сервер может использовать больше ресурсов для обработки каждого сообщения в событии [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) по сравнению с событием [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , так как сервер выполняет все необходимое преобразование контента и определяет следующий прыжок в маршруте для сообщения перед выполнением кода в обработчике событий [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) .</span><span class="sxs-lookup"><span data-stu-id="00754-119">The server might use more resources to process each message in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event than the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event because the server will perform any necessary content conversion and determine the next hop in the route for the message before it executes the code in the [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx) event handler.</span></span>  <br/> |
|[<span data-ttu-id="00754-120">онсубмиттедмессаже</span><span class="sxs-lookup"><span data-stu-id="00754-120">OnSubmittedMessage</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) <br/> |<span data-ttu-id="00754-121">Возникает после того, как сообщение отправится из очереди.</span><span class="sxs-lookup"><span data-stu-id="00754-121">Occurs after the message is taken off the submit queue.</span></span> <span data-ttu-id="00754-122">Используйте событие [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) , если агент транспорта RoutingAgent не нуждается в преобразовании контента, разрешенных получателях или данных маршрутизации.</span><span class="sxs-lookup"><span data-stu-id="00754-122">Use the [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) event if your RoutingAgent transport agent does not require content conversion, resolved recipients, or routing data.</span></span>  <br/> |
   
## <a name="creating-a-custom-routingagent-transport-agent"></a><span data-ttu-id="00754-123">Создание настраиваемого агента транспорта RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="00754-123">Creating a custom RoutingAgent transport agent</span></span>

<span data-ttu-id="00754-124">В следующей процедуре описано, как создать настраиваемый агент транспорта RoutingAgent.</span><span class="sxs-lookup"><span data-stu-id="00754-124">The following procedure describes how to create a custom RoutingAgent transport agent.</span></span> 
  
### <a name="to-create-the-transport-agent"></a><span data-ttu-id="00754-125">Создание агента транспорта</span><span class="sxs-lookup"><span data-stu-id="00754-125">To create the transport agent</span></span>

1. <span data-ttu-id="00754-126">Добавьте ссылки на пространства имен.</span><span class="sxs-lookup"><span data-stu-id="00754-126">Add references to the namespaces.</span></span>
    
   ```cs
      using Microsoft.Exchange.Data.Mime;
      using Microsoft.Exchange.Data.Transport;
      using Microsoft.Exchange.Data.Transport.Routing;
  
   ```

   <span data-ttu-id="00754-127">Эти пространства имен можно найти на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="00754-127">You can find these namespaces on your Exchange server.</span></span> <span data-ttu-id="00754-128">Добавив ссылку на эти пространства имен, вы получите доступ к элементам [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) , а также к другим классам, используемым в [Exchange 2013: Создание примера агента транспорта журналов пропускной способности](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) .</span><span class="sxs-lookup"><span data-stu-id="00754-128">By adding a reference to these namespaces, you will have access to the [RoutingAgent](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx) members as well as other classes used in the [Exchange 2013: Build a bandwidth logging transport agent](http://code.msdn.microsoft.com/Exchange/Exchange-2013-Build-a-d61a4aaa) sample.</span></span> 
    
2. <span data-ttu-id="00754-129">Реализуйте производный класс для класса [раутингажентфактори](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) .</span><span class="sxs-lookup"><span data-stu-id="00754-129">Implement the derived class for the [RoutingAgentFactory](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx) class.</span></span> 
    
   ```cs
      public class BandwidthLoggerFactory : RoutingAgentFactory
      {
          public override RoutingAgent CreateAgent(SmtpServer server)
          {
              return new BandwidthLogger(server);
          }
      }
  
   ```

   <span data-ttu-id="00754-130">В этом коде создается экземпляр производного класса и переопределяется метод **креатеажент** для создания экземпляра нового настраиваемого агента.</span><span class="sxs-lookup"><span data-stu-id="00754-130">This code will instantiate the derived class and override the **CreateAgent** method to create an instance of your new custom agent.</span></span> <span data-ttu-id="00754-131">Дополнительные методы, такие как **Close**, также могут быть переопределены в этом классе для выполнения пользовательского кода.</span><span class="sxs-lookup"><span data-stu-id="00754-131">Additional methods, such as **Close**, can also be overridden in this class to execute custom code.</span></span> 
    
3. <span data-ttu-id="00754-132">Определите свой агент.</span><span class="sxs-lookup"><span data-stu-id="00754-132">Define your agent.</span></span>
    
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

   <span data-ttu-id="00754-133">Определив класс агента, вы можете добавить пользовательские функции.</span><span class="sxs-lookup"><span data-stu-id="00754-133">After you define your agent class, you can add you custom functionality.</span></span> <span data-ttu-id="00754-134">В этом примере два события [онсубмиттедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) и [онраутедмессаже](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)перенаправлены в обработчики пользовательских событий.</span><span class="sxs-lookup"><span data-stu-id="00754-134">In this example, the two events [OnSubmittedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnSubmittedMessage.aspx) and [OnRoutedMessage](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.OnRoutedMessage.aspx)are redirected to your custom event handlers.</span></span> 
    
## <a name="see-also"></a><span data-ttu-id="00754-135">См. также</span><span class="sxs-lookup"><span data-stu-id="00754-135">See also</span></span>

- [<span data-ttu-id="00754-136">Основные понятия, связанные с агентами транспорта в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="00754-136">Transport agent concepts in Exchange 2013</span></span>](transport-agent-concepts-in-exchange-2013.md)    
- [<span data-ttu-id="00754-137">Справочник по агентам транспорта для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="00754-137">Transport agent reference for Exchange 2013</span></span>](transport-agent-reference-for-exchange-2013.md)    
- [<span data-ttu-id="00754-138">раутингажентфактори</span><span class="sxs-lookup"><span data-stu-id="00754-138">RoutingAgentFactory</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgentFactory.aspx)    
- [<span data-ttu-id="00754-139">RoutingAgent</span><span class="sxs-lookup"><span data-stu-id="00754-139">RoutingAgent</span></span>](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Transport.Routing.RoutingAgent.aspx)
    

