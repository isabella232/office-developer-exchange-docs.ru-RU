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
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>Уведомления по запросу о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API EWS или EWS, чтобы подписаться на уведомления и получать события.
  
Службы EWS в Exchange используют Уведомления опрашивающей репликации, чтобы позволить клиентам запрашивать (или получать) уведомления об изменениях в почтовом ящике с сервера клиенту.
  
При подписке на уведомления по запросу с помощью управляемого API EWS вы [можете подписаться на уведомления и получать](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) их с помощью метода [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . Затем вы получаете события с сервера с помощью метода [Events](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) . 
  
Чтобы подписаться на уведомления по запросу с помощью EWS, [создайте подписку](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) с помощью [операции Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx), проанализируйте ответ, а затем [получите уведомления](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) с помощью [операции](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx)GetResponse.
  
После того как клиент получит уведомления об элементах, которые были изменены или созданы на сервере, он сможет [синхронизировать изменения](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Подписаться на уведомления и получать уведомления по запросу с помощью управляемого API EWS
<a name="bk_cepullewsma"> </a>

В приведенном ниже примере кода показано, как использовать метод [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) , чтобы подписаться на уведомления для всех событий в папке "Входящие". Затем в примере используется метод [Events](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) для получения событий с сервера. В этом примере предполагается, что **Служба** является допустимой привязкой [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) . 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

После получения события с сервера вы можете [синхронизировать эти изменения с сервером](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Используйте один из методов unsubscribe, указанных в разделе [как отменить подписку на уведомления?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) , чтобы завершить подписку на сервер, если подписка больше не нужна. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Подпишитесь на уведомления по запросу с помощью EWS
<a name="bk_cepullews"> </a>

В следующем примере показан XML-запрос, который отправляется на сервер для подписки на все [евенттипес](https://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) в папке "Входящие" с помощью [операции Subscribe](https://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Это также запрос XML, который управляемый API EWS отправляет при подписке на уведомления по запросу с помощью метода [subscribetopullnotificationshttp](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . 
  
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

В следующем примере XML-кода показано сообщение [субскрибереспонсе](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) , которое отправляется от сервера клиенту в ответ на запрос операции **Subscribe** . Включение значения ошибки для элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) означает, что подписка была успешно создана. Элемент [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) однозначно идентифицирует подписку на уведомления по запросу на сервере. Элемент [водяного знака](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) представляет закладку в очереди событий почтового ящика. 
  
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

После создания подписки можно получить события, используя значение **SubscriptionId** , которое возвращается в сообщении **субскрибереспонсе** . 
  
## <a name="get-pull-notifications-by-using-ews"></a>Получение уведомлений по запросу с помощью EWS
<a name="bk_getpull"> </a>

В следующем примере XML-кода показаны сообщение о запросе [операции с событиями](https://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) , которое отправляется с клиента на сервер для получения уведомлений для [SubscriptionId](https://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) , возвращаемых в сообщении [субскрибереспонсе](https://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . Для первого запроса на получение **событий** используйте [водяной знак](https://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) , возвращенный в ответе **Subscribe** . Для последующих запросов к **событиям** используйте последний **водяной знак** , который был возвращен в предыдущих запросах **Events** . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

В следующем примере XML-кода показаны ответные сообщения о **событиях** , отправляемые сервером клиенту. Каждый ответ на **события** содержит сведения о одном или нескольких событиях. Для каждого события возвращается **водяной знак** . Последний **водяной знак** должен быть сохранен и использован в последующих запросах на **событие** . Если с момента последнего запроса на получение **событий** не было событий хранилища, возвращается событие Status. 
  
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

После получения события с сервера [синхронизируйте изменения, внесенные в клиент](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Используйте [операцию unsubscribe](https://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) , чтобы завершить подписку на сервер, если подписка больше не нужна. 
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_nextsteps"> </a>

После получения уведомлений можно [синхронизировать иерархию папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [синхронизировать содержимое измененной папки](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Потоковая передача уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Поддержание сходства между группой подписок и сервером почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Обработка ошибок, связанных с уведомлениями, в EWS в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

