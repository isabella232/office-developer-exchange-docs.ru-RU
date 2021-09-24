---
title: Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Узнайте, как использовать управляемый API или EWS EWS для подписки на получение уведомлений и получения событий.
ms.openlocfilehash: eb694eddd16567e42ccc43b2854f0432c54dc6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513103"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API или EWS EWS для подписки на получение уведомлений и получения событий.
  
EWS в Exchange для того, чтобы клиенты могли запрашивать (или тянуть) уведомления об изменениях в почтовом ящике с сервера на клиента.
  
Если вы подписываете подписку на получение уведомлений с помощью управляемого API EWS, вы подписываете и получаете уведомления о тяге с помощью метода [SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) Затем события получаются с сервера с помощью [метода GetEvents.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) 
  
Чтобы подписаться на получение уведомлений [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) с помощью EWS, вы создаете подписку [](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) с помощью операции [Подписка,](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)разберите ответ, а затем получите уведомления с помощью [операции GetEvents](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
После получения клиентом уведомлений об изменениях или создания элементов на сервере он может [синхронизировать изменения.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps)
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Подписка на уведомления о вытягии и получение их с помощью управляемого API EWS
<a name="bk_cepullewsma"> </a>

В следующем примере кода показано, как использовать метод [SubscribeToPullNotifications](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) для подписки на получение уведомлений для всех событий в папке "Входящие". В этом примере метод [GetEvents](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) используется для получения событий с сервера. В этом примере предполагается, что **служба является** допустимой привязкой [ExchangeService.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

После получения события с сервера можно синхронизировать [эти изменения с сервером.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) Используйте один из методов отписки, указанных в "Как отписаться от [уведомлений?",](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) чтобы прекратить подписку на сервер, когда подписка больше не требуется. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Подписка на получение уведомлений с помощью EWS
<a name="bk_cepullews"> </a>

В следующем примере показан XML-запрос на отправку на сервер для подписки на все [eventTypes](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) в папке "Входящие" с помощью операции [Подписка.](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx) Это также XML-запрос, который управляемый API EWS отправляет при подписке на получение уведомлений с помощью метода [SubscribeToPullNotifications.](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) 
  
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

В следующем примере XML показано сообщение [SubscribeResponse,](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) которое отправляется с сервера клиенту в ответ на запрос **операции Subscribe.** Включение значения NoError для элемента [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) означает, что подписка была создана успешно. Элемент [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) однозначно определяет подписку на уведомление о тяге на сервере. Элемент [Watermark](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) представляет закладки в очереди событий почтового ящика. 
  
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

После создания подписки вы можете получать события с помощью **SubscriptionId,** возвращаемого в сообщении **SubscribeResponse.** 
  
## <a name="get-pull-notifications-by-using-ews"></a>Получать уведомления о вытягии с помощью EWS
<a name="bk_getpull"> </a>

В следующем примере XML показано сообщение запроса на операцию [GetEvents,](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) которое отправляется от клиента на сервер для получения уведомлений о [подписке,](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) возвращаемой в сообщении [SubscribeResponse.](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) Для первого **запроса GetEvents** используйте [водяной знак,](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) возвращенный в **ответе Подписка.** Для **последующих запросов GetEvents** используйте последний **водяной** знак, возвращенный в предыдущем запросе **GetEvents.** 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

В следующем примере XML показано сообщение **ответа GetEvents,** которое отправляется с сервера клиенту. Каждый **ответ GetEvents** содержит сведения об одном или более событиях. Для **каждого события** возвращается водяной знак. Последний **водяной знак** необходимо сохранить и использовать в следующем запросе **GetEvents.** Если после последнего запроса **GetEvents** события магазина не происходили, событие состояния возвращается. 
  
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

После получения события с сервера [синхронизуй изменения с клиентом.](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps) Используйте операцию [Отписки,](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) чтобы прекратить подписку на сервере, когда подписка больше не требуется. 
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_nextsteps"> </a>

После получать уведомления можно синхронизировать иерархию папок или синхронизировать содержимое [измененной папки.](how-to-synchronize-items-by-using-ews-in-exchange.md) [](how-to-synchronize-folders-by-using-ews-in-exchange.md)
  
## <a name="see-also"></a>См. также


- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

