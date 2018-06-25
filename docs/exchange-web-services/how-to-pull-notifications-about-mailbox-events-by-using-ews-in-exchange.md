---
title: По запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: eb25cbd1-2244-4c3f-a71a-5ee20f81c41f
description: Узнайте, как использовать управляемый API EWS или веб-служб Exchange для подписки на уведомления репликации по запросу и получить события.
ms.openlocfilehash: 6a04aaf0102c149691a30c2bd2f499e03265bce8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761101"
---
# <a name="pull-notifications-about-mailbox-events-by-using-ews-in-exchange"></a>По запросу уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange

Узнайте, как использовать управляемый API EWS или веб-служб Exchange для подписки на уведомления репликации по запросу и получить события.
  
ВЕБ-службах Exchange для предоставления клиентам запроса (или репликации по запросу) уведомления об изменениях в почтовый ящик с сервера на клиент использует уведомления по запросу.
  
Если подписки на уведомления по запросу с помощью управляемых API EWS, можно [подписаться на и получение уведомлений репликации по запросу](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullewsma) с помощью метода [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . Затем вы получите событий с сервера с помощью метода [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) . 
  
Подписаться на уведомления по запросу с помощью веб-служб Exchange, [Создать подписку](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_cepullews) с помощью [операции подписки на](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx)синтаксический анализ ответа и [Получение уведомлений](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_getpull) с помощью [операции GetEvents](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx).
  
После получения уведомления из элементов, которые были изменены или созданы на сервере, его можно [синхронизировать изменения](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps).
  
## <a name="subscribe-to-and-get-pull-notifications-by-using-the-ews-managed-api"></a>Подпишитесь на и получать уведомления по запросу с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_cepullewsma"> </a>

В следующем примере кода показано, как использовать метод [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) для подписки на уведомления репликации по запросу для всех событий в папке "Входящие". Затем в примере используется метод [GetEvents](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pullsubscription.getevents%28v=exchg.80%29.aspx) для получения событий на сервере. В этом примере мы предполагаем, что допустимой привязки [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) этой **службы** . 
  
```cs
// Subscribe to pull notifications in the Inbox.
PullSubscription subscription = service.SubscribeToPullNotifications( 
    new FolderId[] { WellKnownFolderName.Inbox }, 30, null, 
    EventType.NewMail, EventType.Created, EventType.Deleted,
    EventType.Modified, EventType.Moved, EventType.Copied, EventType.FreeBusyChanged); 
 
// Call GetEvents to retrieve events from the server. 
GetEventsResults events = subscription.GetEvents(); 
```

После появления события с сервера можно [синхронизировать эти изменения на сервере](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). Используйте один из методов отказа от подписки, указанного в [как отписаться на уведомления?](notification-subscriptions-mailbox-events-and-ews-in-exchange.md#bk_notifunsubscribe) окончания подписки с сервером, когда подписка больше не требуется. 
  
## <a name="subscribe-to-pull-notifications-by-using-ews"></a>Подписаться на уведомления по запросу с помощью веб-служб Exchange
<a name="bk_cepullews"> </a>

В следующем примере показано запрос XML для отправки на сервер для подписки на все [EventTypes](http://msdn.microsoft.com/library/29ded9e5-f191-4aa3-bc3e-500de2fc8818%28Office.15%29.aspx) в папке "Входящие" с помощью [подписки на операции](http://msdn.microsoft.com/library/f17c3d08-c79e-41f1-ba31-6e41e7aafd87%28Office.15%29.aspx). Это также XML-запрос, который отправляет управляемый API EWS при присоединении к запросу уведомлений с помощью метода [SubscribeToPullNotifications](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.subscribetopullnotifications%28v=exchg.80%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <PullSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
      <DistinguishedFolderId Id="inbox" />
    </FolderIds>
    <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
            <EventType>NewMailEvent</EventType>
            <EventType>CreatedEvent</EventType>
            <EventType>DeletedEvent</EventType>
            <EventType>ModifiedEvent</EventType>
            <EventType>MovedEvent</EventType>
            <EventType>CopiedEvent</EventType>
            <EventType>FreeBusyChangedEvent</EventType>
    </EventTypes>
    <Timeout xmlns="http://schemas.microsoft.com/exchange/services/2006/types">30</Timeout>
  </PullSubscriptionRequest>
</Subscribe>
```

В следующем примере XML показано [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) сообщение, которое отправляется с сервера клиенту в ответ на запрос **подписки на** операции. Включение NoError значение для элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) означает, что успешно создана подписка. Элемент [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) однозначно определяет подписки уведомлений по запросу на сервере. Элемент [водяного знака](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) представляет закладку в очереди событий почтового ящика. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<SubscribeResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                   xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <SubscribeResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <SubscriptionId>d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
      <Watermark>AAAAAGUhAAAAAAAAAQ==</Watermark>
    </SubscribeResponseMessage>
  </ResponseMessages>
</SubscribeResponse>
```

После создания подписки, можно получить с помощью **SubscriptionId** , который возвращается в сообщении **SubscribeResponse** события. 
  
## <a name="get-pull-notifications-by-using-ews"></a>Получать уведомления по запросу с помощью веб-служб Exchange
<a name="bk_getpull"> </a>

В следующем примере XML показано сообщение запроса [GetEvents операции](http://msdn.microsoft.com/library/f268efe5-9a1a-41a2-b6a6-51fcde7720a1%28Office.15%29.aspx) , передаче от клиента к серверу для получения уведомлений для [SubscriptionId](http://msdn.microsoft.com/library/77c0abab-69e8-428e-8c20-22258e4ef71b%28Office.15%29.aspx) , который возвращается в сообщении [SubscribeResponse](http://msdn.microsoft.com/library/fd87e9b7-c231-44fa-9f5b-19ae96cda5cc%28Office.15%29.aspx) . Для первого запроса **GetEvents** используйте [водяного знака](http://msdn.microsoft.com/library/e1545046-94f9-4ac7-af1c-ea81dfb6822c%28Office.15%29.aspx) , возвращаемого в ответе **подписаться** . Для последующих запросов **GetEvents** используйте последний **водяного знака** , который был возвращен в предыдущем **GetEvents** запроса. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEvents xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
  <Watermark xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">AAAAAGUhAAAAAAAAAQ==</Watermark>
</GetEvents>
```

В следующем примере XML показано **GetEvents** ответное сообщение, которое отправляется с сервера. Каждый отклик **GetEvents** включены сведения о одно или несколько событий. Для каждого события возвращается **водяного знака** . Последний **водяной знак** должен быть сохранен и используется в следующем запросе **GetEvents** . Если события не хранилище были выполнены с момента последнего запроса **GetEvents** , возвращается состояние события. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<GetEventsResponseType xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <GetEventsResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <Notification>
        <SubscriptionId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">d581ab79-a2ec-4653-9c8e-564d7cfc1d8c</SubscriptionId>
        <PreviousWatermark xmlns="http://schemas.microsoft.com/exchange/services/2006/types">AAAAAGUhAAAAAAAAAQ==</PreviousWatermark>
        <MoreEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/types">false</MoreEvents>
        <NewMailEvent xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

После получения события с сервера, [синхронизировать изменения клиенту](how-to-pull-notifications-about-mailbox-events-by-using-ews-in-exchange.md#bk_nextsteps). С помощью [операции отказа от подписки](http://msdn.microsoft.com/library/994a9d2b-1501-4804-90f0-12bd914496ec%28Office.15%29.aspx) окончания подписки с сервером, когда подписка больше не требуется. 
  
## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_nextsteps"> </a>

После время получения уведомления, можно [синхронизацию иерархии папок](how-to-synchronize-folders-by-using-ews-in-exchange.md) или [Синхронизация содержимого папки, изменены](how-to-synchronize-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также


- [Подписки на уведомления, события почтовых ящиков и службы EWS в Exchange](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)
    
- [Поток уведомлений о событиях почтовых ящиков с помощью веб-служб Exchange в Exchange](how-to-stream-notifications-about-mailbox-events-by-using-ews-in-exchange.md)
    
- [Поддержка сходства между группой подписок и сервера почтовых ящиков в Exchange](how-to-maintain-affinity-between-group-of-subscriptions-and-mailbox-server.md)
    
- [Обработка ошибок, связанных с уведомлений в веб-служб Exchange в Exchange](handling-notification-related-errors-in-ews-in-exchange.md)
    
- [Синхронизация почтового ящика и веб-службах Exchange](mailbox-synchronization-and-ews-in-exchange.md)
    

