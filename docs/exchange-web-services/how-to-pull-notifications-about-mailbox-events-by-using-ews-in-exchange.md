---
title: Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Узнайте, как использовать управляемый API EWS или EWS, чтобы подписаться на уведомления и получать события.
ms.openlocfilehash: 3d77c0d4efb8fc853eea64ff2429af5c3dbead27
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456750"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a><span data-ttu-id="a712b-103">Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-103">Pull notifications about mailbox events by using EWS in Exchange</span></span>

<span data-ttu-id="a712b-104">Узнайте, как использовать управляемый API EWS или EWS, чтобы подписаться на уведомления и получать события.</span><span class="sxs-lookup"><span data-stu-id="a712b-104">Find out how to use the EWS Managed API or EWS to subscribe to pull notifications and get events.</span></span>
  
<span data-ttu-id="a712b-105">Службы EWS в Exchange используют Уведомления опрашивающей репликации, чтобы позволить клиентам запрашивать (или получать) уведомления об изменениях в почтовом ящике с сервера клиенту.</span><span class="sxs-lookup"><span data-stu-id="a712b-105">EWS in Exchange uses pull notifications to enable clients to request (or pull) notifications about changes to the mailbox from the server to the client.</span></span>
  
<span data-ttu-id="a712b-106">При подписке на уведомления по запросу с помощью управляемого API EWS вы [можете подписаться на уведомления и получать](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) их с помощью метода [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a712b-106">If you're subscribing to pull notifications by using the EWS Managed API, you [subscribe to and get pull notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="a712b-107">Затем вы получаете события с сервера с помощью метода [Events](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a712b-107">You then get events from the server by using the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="a712b-108">Чтобы подписаться на уведомления по запросу с помощью EWS, [создайте подписку](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) с помощью [операции Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), проанализируйте ответ, а затем [получите уведомления](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) с помощью [операции](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)GetResponse.</span><span class="sxs-lookup"><span data-stu-id="a712b-108">To subscribe to pull notifications by using EWS, you [create a subscription](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), parse the response, and then [get the notifications](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) by using the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="a712b-109">После того как клиент получит уведомления об элементах, которые были изменены или созданы на сервере, он сможет [синхронизировать изменения](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a712b-109">After the client receives notifications of items that are changed or created on the server, it can then [synchronize the changes](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span>
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a><span data-ttu-id="a712b-110">Подписаться на уведомления и получать уведомления по запросу с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="a712b-110">Subscribe to and get pull notifications by using the EWS Managed API</span></span>
<span data-ttu-id="a712b-111"><a name="bk_cepullewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="a712b-111"><a name="bk_cepullewsma"> </a></span></span>

<span data-ttu-id="a712b-112">В приведенном ниже примере кода показано, как использовать метод [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) , чтобы подписаться на уведомления для всех событий в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="a712b-112">The following code example shows how to use the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method to subscribe to pull notifications for all events in the Inbox folder.</span></span> <span data-ttu-id="a712b-113">Затем в примере используется метод [Events](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) для получения событий с сервера.</span><span class="sxs-lookup"><span data-stu-id="a712b-113">The example then uses the [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) method to retrieve events from the server.</span></span> <span data-ttu-id="a712b-114">В этом примере предполагается, что **Служба** является допустимой привязкой [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a712b-114">In this example, we assume that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) binding.</span></span> 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

<span data-ttu-id="a712b-115">После получения события с сервера вы можете [синхронизировать эти изменения с сервером](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span><span class="sxs-lookup"><span data-stu-id="a712b-115">After you receive an event from the server, you can [synchronize those changes with the server](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).</span></span> <span data-ttu-id="a712b-116">Используйте один из методов unsubscribe, указанных в разделе [как отменить подписку на уведомления?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) , чтобы завершить подписку на сервер, если подписка больше не нужна.</span><span class="sxs-lookup"><span data-stu-id="a712b-116">Use one of the unsubscribe methods specified in [How do I unsubscribe to notifications?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a><span data-ttu-id="a712b-117">Подпишитесь на уведомления по запросу с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="a712b-117">Subscribe to pull notifications by using EWS</span></span>
<span data-ttu-id="a712b-118"><a name="bk_cepullews"> </a></span><span class="sxs-lookup"><span data-stu-id="a712b-118"><a name="bk_cepullews"> </a></span></span>

<span data-ttu-id="a712b-119">В следующем примере показан XML-запрос, который отправляется на сервер для подписки на все [евенттипес](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) в папке "Входящие" с помощью [операции Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="a712b-119">The following example shows the XML request to send to the server to subscribe to all [EventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) in the Inbox folder by using the [Subscribe operation](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx).</span></span> <span data-ttu-id="a712b-120">Это также запрос XML, который управляемый API EWS отправляет при подписке на уведомления по запросу с помощью метода [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a712b-120">This is also the XML request that the EWS Managed API sends when subscribing to pull notifications by using the [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="https://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

<span data-ttu-id="a712b-121">В следующем примере XML-кода показано сообщение [субскрибереспонсе](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции **Subscribe** .</span><span class="sxs-lookup"><span data-stu-id="a712b-121">The following XML example shows the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message that is sent from the server to the client in response to the **Subscribe** operation request.</span></span> <span data-ttu-id="a712b-122">Включение значения ошибки для элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) означает, что подписка была успешно создана.</span><span class="sxs-lookup"><span data-stu-id="a712b-122">The inclusion of the NoError value for the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element means that the subscription was created successfully.</span></span> <span data-ttu-id="a712b-123">Элемент [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) однозначно идентифицирует подписку на уведомления по запросу на сервере.</span><span class="sxs-lookup"><span data-stu-id="a712b-123">The [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) element uniquely identifies the pull notification subscription on the server.</span></span> <span data-ttu-id="a712b-124">Элемент [водяного знака](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) представляет закладку в очереди событий почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a712b-124">The [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) element represents a bookmark in the mailbox event queue.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

<span data-ttu-id="a712b-125">После создания подписки можно получить события, используя значение **SubscriptionId** , которое возвращается в сообщении **субскрибереспонсе** .</span><span class="sxs-lookup"><span data-stu-id="a712b-125">After creating the subscription, you can now get events by using the **SubscriptionId** that is returned in the **SubscribeResponse** message.</span></span> 
  
## <a name="get-pull-notifications-by-using-ews"></a><span data-ttu-id="a712b-126">Получение уведомлений по запросу с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="a712b-126">Get pull notifications by using EWS</span></span>
<span data-ttu-id="a712b-127"><a name="bk_getpull"> </a></span><span class="sxs-lookup"><span data-stu-id="a712b-127"><a name="bk_getpull"> </a></span></span>

<span data-ttu-id="a712b-128">В следующем примере XML-кода показаны сообщение о запросе [операции с событиями](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) , которое отправляется с клиента на сервер для получения уведомлений для [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) , возвращаемых в сообщении [субскрибереспонсе](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="a712b-128">The following XML example shows the [GetEvents operation](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) request message that is sent from the client to the server to get notifications for the [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) that is returned in the [SubscribeResponse](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) message.</span></span> <span data-ttu-id="a712b-129">Для первого запроса на получение **событий** используйте [водяной знак](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) , возвращенный в ответе **Subscribe** .</span><span class="sxs-lookup"><span data-stu-id="a712b-129">For the first **GetEvents** request, use the [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) returned in the **Subscribe** response.</span></span> <span data-ttu-id="a712b-130">Для последующих запросов к **событиям** используйте последний **водяной знак** , который был возвращен в предыдущих запросах **Events** .</span><span class="sxs-lookup"><span data-stu-id="a712b-130">For subsequent **GetEvents** requests, use the last **Watermark** that was returned in the previous **GetEvents** request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

<span data-ttu-id="a712b-131">В следующем примере XML-кода показаны ответные сообщения о **событиях** , отправляемые сервером клиенту.</span><span class="sxs-lookup"><span data-stu-id="a712b-131">The following XML example shows the **GetEvents** response message that is sent from the server to the client.</span></span> <span data-ttu-id="a712b-132">Каждый ответ на **события** содержит сведения о одном или нескольких событиях.</span><span class="sxs-lookup"><span data-stu-id="a712b-132">Each **GetEvents** response includes information about one or more events.</span></span> <span data-ttu-id="a712b-133">Для каждого события возвращается **водяной знак** .</span><span class="sxs-lookup"><span data-stu-id="a712b-133">A **Watermark** is returned for each event.</span></span> <span data-ttu-id="a712b-134">Последний **водяной знак** должен быть сохранен и использован в последующих запросах на **событие** .</span><span class="sxs-lookup"><span data-stu-id="a712b-134">The last **Watermark** must be saved and used in the next **GetEvents** request.</span></span> <span data-ttu-id="a712b-135">Если с момента последнего запроса на получение **событий** не было событий хранилища, возвращается событие Status.</span><span class="sxs-lookup"><span data-stu-id="a712b-135">If no store events have occurred since the last **GetEvents** request, a status event is returned.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="https://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Watermark>AAAAAHMhAAAAAAAAAQ==</Watermark>
          <TimeStamp>2013-09-15T21:37:01Z</TimeStamp>
          <ItemId Id="AAAtA=" ChangeKey="CQAAAA==" />
          <ParentFolderId Id="AQAtAEFkbWA==" ChangeKey="AQAAAA==" />
        </NewMailEvent>
      </Notification>
    </GetEventsResponseMessage>
  </ResponseMessages>
</GetEventsResponse>
```

После получения события с сервера [синхронизируйте изменения, внесенные в клиент](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). <span data-ttu-id="a712b-137">Используйте [операцию unsubscribe](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) , чтобы завершить подписку на сервер, если подписка больше не нужна.</span><span class="sxs-lookup"><span data-stu-id="a712b-137">Use the [Unsubscribe operation](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) to end the subscription with the server when the subscription is no longer needed.</span></span> 
  
## <a name="next-steps"></a><span data-ttu-id="a712b-138">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a712b-138">Next steps</span></span>
<span data-ttu-id="a712b-139"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="a712b-139"><a name="bk_nextsteps"> </a></span></span>

<span data-ttu-id="a712b-140">После получения уведомлений можно [синхронизировать иерархию папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [синхронизировать содержимое измененной папки](how-to-synchronize-items-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a712b-140">After you're received notifications, you can [sync the folder hierarchy](how-to-synchronize-folders-by-using-ews-in-exchange.md) or [sync the contents of the folder that changed](how-to-synchronize-items-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a712b-141">См. также</span><span class="sxs-lookup"><span data-stu-id="a712b-141">See also</span></span>


- [<span data-ttu-id="a712b-142">Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-142">Notification subscriptions, mailbox events, and EWS in Exchange</span></span>](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [<span data-ttu-id="a712b-143">Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-143">Stream notifications about mailbox events by using EWS in Exchange</span></span>](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="a712b-144">Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-144">Maintain affinity between a group of subscriptions and the Mailbox server in Exchange</span></span>](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [<span data-ttu-id="a712b-145">Обработка ошибок, связанных с уведомлениями, в EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-145">Handling notification-related errors in EWS in Exchange</span></span>](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [<span data-ttu-id="a712b-146">Синхронизация почтового ящика и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="a712b-146">Mailbox synchronization and EWS in Exchange</span></span>](mailbox-synchronization-and-ews-in-exchange.md)
    

