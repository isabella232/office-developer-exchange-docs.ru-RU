---
title: Операция GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: f268efe5-9a1a-41a2-b6a6-51fcde7720a1
description: Операция Events используется клиентами подписки по запросу для запроса уведомлений с сервера клиентского доступа. Ответ операции Events возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления.
ms.openlocfilehash: 9258fd003c242911866aa7abbca5eba2b9582223
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462516"
---
# <a name="getevents-operation"></a><span data-ttu-id="131dd-104">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="131dd-104">GetEvents operation</span></span>

<span data-ttu-id="131dd-105">Операция **Events** используется клиентами подписки по запросу для запроса уведомлений с сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="131dd-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="131dd-106">Ответ операции **Events** возвращает массив элементов и событий, произошедших в почтовом ящике с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="131dd-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="131dd-107">Операция **DeleteUserConfiguration** инициирует событие Move для системы уведомления о событиях.</span><span class="sxs-lookup"><span data-stu-id="131dd-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="131dd-108">Объект конфигурации пользователя будет перемещен в корзину.</span><span class="sxs-lookup"><span data-stu-id="131dd-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="131dd-109">Примечания</span><span class="sxs-lookup"><span data-stu-id="131dd-109">Remarks</span></span>

<span data-ttu-id="131dd-110">Изменения элементов календаря могут привести к созданию нескольких событий.</span><span class="sxs-lookup"><span data-stu-id="131dd-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="131dd-111">Эти события являются результатом того, что временные элементы создаются в почтовом ящике, элементы хранения данных о занятости изменяются в рамках обычных операций календаря или и то, и другое.</span><span class="sxs-lookup"><span data-stu-id="131dd-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="131dd-112">События для класса элемента "IPM. Счедулеплус. FreeBusy. Бинаридата должен игнорироваться клиентами веб-служб.</span><span class="sxs-lookup"><span data-stu-id="131dd-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="131dd-113">Эти временные элементы удаляются после их создания; Таким образом, при попытке получить эти элементы возвращается ошибка, указывающая на то, что элемент не найден.</span><span class="sxs-lookup"><span data-stu-id="131dd-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="131dd-114">Пример запроса на получение событий</span><span class="sxs-lookup"><span data-stu-id="131dd-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="131dd-115">Description</span><span class="sxs-lookup"><span data-stu-id="131dd-115">Description</span></span>

<span data-ttu-id="131dd-116">В приведенном ниже примере показано, как запросить события и элементы, связанные с подпиской, которая определяется идентификатором подписки и водяным знаком.</span><span class="sxs-lookup"><span data-stu-id="131dd-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="131dd-117">Код</span><span class="sxs-lookup"><span data-stu-id="131dd-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="131dd-118">Элементы запроса Events</span><span class="sxs-lookup"><span data-stu-id="131dd-118">GetEvents Request Elements</span></span>

<span data-ttu-id="131dd-119">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="131dd-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="131dd-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="131dd-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="131dd-121">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="131dd-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="131dd-122">Watermark</span><span class="sxs-lookup"><span data-stu-id="131dd-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="131dd-123">Пример успешных откликов на события</span><span class="sxs-lookup"><span data-stu-id="131dd-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="131dd-124">Description</span><span class="sxs-lookup"><span data-stu-id="131dd-124">Description</span></span>

<span data-ttu-id="131dd-125">В приведенном ниже примере ответа показано уведомление о существовании двух новых почтовых сообщений с момента отправки последнего запроса уведомления на сервер.</span><span class="sxs-lookup"><span data-stu-id="131dd-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="131dd-126">Код</span><span class="sxs-lookup"><span data-stu-id="131dd-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:PreviousWatermark>AAAAAMAGAAAAAAAAAQ==</t:PreviousWatermark>
            <t:MoreEvents>false</t:MoreEvents>
            <t:NewMailEvent>
              <t:Watermark>AAAAAM4GAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T00:36:29Z</t:TimeStamp>
              <t:ItemId Id="AQApAHR" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:NewMailEvent>
              <t:Watermark>AAAAAOQGAAAAAAAAAQ==</t:Watermark>
              <t:TimeStamp>2006-08-22T01:00:50Z</t:TimeStamp>
              <t:ItemId Id="AQApAHRw" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQApAH" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
          </m:Notification>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="131dd-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="131dd-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="131dd-128">Идентификаторы элементов и папок были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="131dd-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="131dd-129">Элементы ответа на события</span><span class="sxs-lookup"><span data-stu-id="131dd-129">GetEvents response elements</span></span>

<span data-ttu-id="131dd-130">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="131dd-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="131dd-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="131dd-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="131dd-132">жетевентсреспонсе</span><span class="sxs-lookup"><span data-stu-id="131dd-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="131dd-133">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="131dd-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="131dd-134">жетевентсреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="131dd-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="131dd-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="131dd-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="131dd-136">Уведомление</span><span class="sxs-lookup"><span data-stu-id="131dd-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="131dd-137">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="131dd-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="131dd-138">превиаусватермарк</span><span class="sxs-lookup"><span data-stu-id="131dd-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="131dd-139">моривентс</span><span class="sxs-lookup"><span data-stu-id="131dd-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="131dd-140">невмаилевент</span><span class="sxs-lookup"><span data-stu-id="131dd-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="131dd-141">Watermark</span><span class="sxs-lookup"><span data-stu-id="131dd-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="131dd-142">Метка времени</span><span class="sxs-lookup"><span data-stu-id="131dd-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="131dd-143">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="131dd-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="131dd-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="131dd-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="131dd-145">Чтобы найти другие параметры ответного сообщения **для операции GetResponse** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="131dd-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="131dd-146">Начните с элемента [уведомления](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="131dd-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="131dd-147">Пример ответа на сообщение об ошибке при возникновении событий</span><span class="sxs-lookup"><span data-stu-id="131dd-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="131dd-148">Description</span><span class="sxs-lookup"><span data-stu-id="131dd-148">Description</span></span>

<span data-ttu-id="131dd-149">В приведенном ниже примере показан ответ об ошибке запроса на получение **событий** .</span><span class="sxs-lookup"><span data-stu-id="131dd-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="131dd-150">Код</span><span class="sxs-lookup"><span data-stu-id="131dd-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetEventsResponseMessage ResponseClass="Error">
          <m:MessageText>Access is denied. Only the subscription owner may access the subscription.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionAccessDenied</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetEventsResponseMessage>
      </m:ResponseMessages>
    </GetEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="131dd-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="131dd-151">Remarks</span></span>

<span data-ttu-id="131dd-152">При обработке запроса по **событиям** сервер клиентского доступа выполняет следующие действия:</span><span class="sxs-lookup"><span data-stu-id="131dd-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="131dd-153">Значение SubscriptionID для запроса подтверждено допустимой подпиской, размещенной на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="131dd-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="131dd-154">В противном случае произойдет сбой вызова метода **Events** .</span><span class="sxs-lookup"><span data-stu-id="131dd-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="131dd-155">SMTP-адрес пользователя, прошедшего проверку подлинности для запроса, сравнивается с SMTP-адресом пользователя, создавшего подписку.</span><span class="sxs-lookup"><span data-stu-id="131dd-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="131dd-156">Если они не совпадают, происходит сбой запроса **Events** .</span><span class="sxs-lookup"><span data-stu-id="131dd-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="131dd-157">Очередь подписки запрашивает события, ожидающие отправки клиенту.</span><span class="sxs-lookup"><span data-stu-id="131dd-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="131dd-158">Если очередь не пустая, первые 50 событий из очереди извлекаются из очереди и кодируются в уведомление.</span><span class="sxs-lookup"><span data-stu-id="131dd-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="131dd-159">Если в очереди не найдено ни одного события, создается Статусевент и кодируется в ответ на уведомление.</span><span class="sxs-lookup"><span data-stu-id="131dd-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="131dd-160">Ответ на уведомление возвращается клиенту.</span><span class="sxs-lookup"><span data-stu-id="131dd-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="131dd-161">События, включенные в уведомление, удаляются из очереди подписки, а последний водяной знак сервера клиентского доступа для подписки задается водяным знаком последнего возвращаемого события.</span><span class="sxs-lookup"><span data-stu-id="131dd-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="131dd-162">Таймер времени ожидания для подписки сбрасывается.</span><span class="sxs-lookup"><span data-stu-id="131dd-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="131dd-163">См. также</span><span class="sxs-lookup"><span data-stu-id="131dd-163">See also</span></span>



[<span data-ttu-id="131dd-164">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="131dd-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="131dd-165">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="131dd-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="131dd-166">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="131dd-166">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

