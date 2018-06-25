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
description: Операция GetEvents используется клиентами подписки пула для запроса уведомлений с сервера клиентского доступа. Ответ GetEvents операция возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления.
ms.openlocfilehash: 1a23a9d570a4554e54becb7927f25dff89888c74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762763"
---
# <a name="getevents-operation"></a><span data-ttu-id="f2f24-104">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-104">GetEvents operation</span></span>

<span data-ttu-id="f2f24-105">Операция **GetEvents** используется клиентами подписки пула для запроса уведомлений с сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f2f24-105">The **GetEvents** operation is used by pull subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="f2f24-106">Ответ **GetEvents** операция возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="f2f24-106">The **GetEvents** operation response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="f2f24-107">Операция **DeleteUserConfiguration** , будет вызвано событие перемещения по системе события уведомления.</span><span class="sxs-lookup"><span data-stu-id="f2f24-107">The **DeleteUserConfiguration** operation will trigger a move event for the event notification system.</span></span> <span data-ttu-id="f2f24-108">Объект конфигурации пользователя перемещается в корзину.</span><span class="sxs-lookup"><span data-stu-id="f2f24-108">The user configuration object will be moved to the dumpster.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f2f24-109">Замечания</span><span class="sxs-lookup"><span data-stu-id="f2f24-109">Remarks</span></span>

<span data-ttu-id="f2f24-110">Изменения элементов календаря может привести к созданию несколько событий.</span><span class="sxs-lookup"><span data-stu-id="f2f24-110">Changes to Calendar items may result in the generation of multiple events.</span></span> <span data-ttu-id="f2f24-111">Эти события основаны на результатах временные элементов, создаются в почтовом ящике изменяемый как часть обычных операций календаря или оба элементов хранения данных о доступности.</span><span class="sxs-lookup"><span data-stu-id="f2f24-111">These events are the result of temporary items being created in the mailbox, free/busy data storage items being changed as part of the normal Calendar operations, or both.</span></span> <span data-ttu-id="f2f24-112">События для элемента класса «IPM. SchedulePlus.FreeBusy.BinaryData» должны пропускаться клиентов веб-служб.</span><span class="sxs-lookup"><span data-stu-id="f2f24-112">Events for item class "IPM.SchedulePlus.FreeBusy.BinaryData" should be ignored by Web service clients.</span></span> <span data-ttu-id="f2f24-113">Эти временные элементы удаляются после их создания; Таким образом при попытке извлечь эти элементы ошибка будут возвращены, о том, что элемент не найден.</span><span class="sxs-lookup"><span data-stu-id="f2f24-113">These temporary items are deleted after they are created; therefore, if an attempt is made to retrieve these items, an error will be returned that states that the item was not found.</span></span>
  
## <a name="getevents-request-example"></a><span data-ttu-id="f2f24-114">Пример запроса GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-114">GetEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="f2f24-115">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f24-115">Description</span></span>

<span data-ttu-id="f2f24-116">Следующем примере показано, как запросить событий и элементы, связанные с подпиской, который идентифицируется средством идентификатор подписки и водяного знака.</span><span class="sxs-lookup"><span data-stu-id="f2f24-116">The following example shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier and watermark.</span></span>
  
### <a name="code"></a><span data-ttu-id="f2f24-117">Программа</span><span class="sxs-lookup"><span data-stu-id="f2f24-117">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <Watermark>AAAAAMAGAAAAAAAAAQ==</Watermark>
    </GetEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getevents-request-elements"></a><span data-ttu-id="f2f24-118">Элементы запроса GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-118">GetEvents Request Elements</span></span>

<span data-ttu-id="f2f24-119">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f2f24-119">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="f2f24-120">GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-120">GetEvents</span></span>](getevents.md)
    
- [<span data-ttu-id="f2f24-121">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="f2f24-121">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="f2f24-122">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="f2f24-122">Watermark</span></span>](watermark.md)
    
## <a name="successful-getevents-response-example"></a><span data-ttu-id="f2f24-123">Пример успешного ответа GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-123">Successful GetEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="f2f24-124">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f24-124">Description</span></span>

<span data-ttu-id="f2f24-125">В следующем примере ответа показано уведомление об существование двух новых почтовых сообщений с момента последнего уведомления запрос был отправлен на сервер.</span><span class="sxs-lookup"><span data-stu-id="f2f24-125">The following example of a response shows a notification of the existence of two new mail messages since the last notification request was sent to the server.</span></span>
  
### <a name="code"></a><span data-ttu-id="f2f24-126">Программа</span><span class="sxs-lookup"><span data-stu-id="f2f24-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="f2f24-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="f2f24-127">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="f2f24-128">Идентификаторы элементов и папок URL-были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="f2f24-128">The item and folder identifiers have been shortened to preserve readability.</span></span> 
  
### <a name="getevents-response-elements"></a><span data-ttu-id="f2f24-129">Элементы GetEvents ответа</span><span class="sxs-lookup"><span data-stu-id="f2f24-129">GetEvents response elements</span></span>

<span data-ttu-id="f2f24-130">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="f2f24-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="f2f24-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f2f24-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="f2f24-132">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="f2f24-132">GetEventsResponse</span></span>](geteventsresponse.md)
    
- [<span data-ttu-id="f2f24-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f2f24-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="f2f24-134">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f2f24-134">GetEventsResponseMessage</span></span>](geteventsresponsemessage.md)
    
- [<span data-ttu-id="f2f24-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f2f24-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f2f24-136">Уведомление</span><span class="sxs-lookup"><span data-stu-id="f2f24-136">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="f2f24-137">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="f2f24-137">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="f2f24-138">PreviousWatermark</span><span class="sxs-lookup"><span data-stu-id="f2f24-138">PreviousWatermark</span></span>](previouswatermark.md)
    
- [<span data-ttu-id="f2f24-139">MoreEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-139">MoreEvents</span></span>](moreevents.md)
    
- [<span data-ttu-id="f2f24-140">NewMailEvent</span><span class="sxs-lookup"><span data-stu-id="f2f24-140">NewMailEvent</span></span>](newmailevent.md)
    
- [<span data-ttu-id="f2f24-141">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="f2f24-141">Watermark</span></span>](watermark.md)
    
- [<span data-ttu-id="f2f24-142">Метка времени</span><span class="sxs-lookup"><span data-stu-id="f2f24-142">TimeStamp</span></span>](timestamp.md)
    
- [<span data-ttu-id="f2f24-143">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="f2f24-143">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="f2f24-144">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="f2f24-144">ParentFolderId</span></span>](parentfolderid.md)
    
<span data-ttu-id="f2f24-145">Чтобы найти другие параметры в сообщении ответа **GetEvents** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="f2f24-145">To find other options for the response message of the **GetEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="f2f24-146">Запустите на элементе [уведомлений](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="f2f24-146">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getevents-error-response-example"></a><span data-ttu-id="f2f24-147">Пример ответа об ошибке GetEvents</span><span class="sxs-lookup"><span data-stu-id="f2f24-147">GetEvents Error response example</span></span>

### <a name="description"></a><span data-ttu-id="f2f24-148">Описание</span><span class="sxs-lookup"><span data-stu-id="f2f24-148">Description</span></span>

<span data-ttu-id="f2f24-149">В следующем примере показано возврату ошибки **GetEvents** запрос.</span><span class="sxs-lookup"><span data-stu-id="f2f24-149">The following example shows an error response to a **GetEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="f2f24-150">Программа</span><span class="sxs-lookup"><span data-stu-id="f2f24-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
                 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="remarks"></a><span data-ttu-id="f2f24-151">Замечания</span><span class="sxs-lookup"><span data-stu-id="f2f24-151">Remarks</span></span>

<span data-ttu-id="f2f24-152">При обработке запроса **GetEvents** сервера клиентского доступа необходимо выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="f2f24-152">When processing a **GetEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="f2f24-153">SubscriptionID запрос подтверждения действительную подписку, размещенного на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f2f24-153">The SubscriptionID of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="f2f24-154">Если он не установлен, **GetEvents** завершается неудачно.</span><span class="sxs-lookup"><span data-stu-id="f2f24-154">If it is not, the **GetEvents** call fails.</span></span> 
    
2. <span data-ttu-id="f2f24-155">SMTP-адрес пользователя, прошедшего проверку подлинности для запроса сравнивается с SMTP-адрес пользователя, создавшего подписку.</span><span class="sxs-lookup"><span data-stu-id="f2f24-155">The SMTP address of the authenticated user for the request is compared to the SMTP address of the user who created the subscription.</span></span> <span data-ttu-id="f2f24-156">Если они не совпадают, происходит сбой запроса **GetEvents** .</span><span class="sxs-lookup"><span data-stu-id="f2f24-156">If they do not match, the **GetEvents** request fails.</span></span> 
    
3. <span data-ttu-id="f2f24-157">Очередь подписки будет опрошен на наличие событий, ожидающих отправляются клиенту.</span><span class="sxs-lookup"><span data-stu-id="f2f24-157">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="f2f24-158">Если очередь не является пустым, первые 50 события из очереди, которые извлекаются из очереди и кодируются в уведомление.</span><span class="sxs-lookup"><span data-stu-id="f2f24-158">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="f2f24-159">Если события не обнаружены в очереди, StatusEvent создан и кодируются в ответ уведомлений.</span><span class="sxs-lookup"><span data-stu-id="f2f24-159">If no events are found in the queue, a StatusEvent is generated and encoded into a notification response.</span></span>
    
5. <span data-ttu-id="f2f24-160">Уведомление ответ возвращается клиенту.</span><span class="sxs-lookup"><span data-stu-id="f2f24-160">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="f2f24-161">События, включенные в уведомлении, удаляются из очереди подписки, клиентского доступа сервера локальной последний водяной знак для подписки на задано значение водяной знак последнего события, который возвращается.</span><span class="sxs-lookup"><span data-stu-id="f2f24-161">The events that are included in the notification are removed from the subscription queue and the Client Access server local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="f2f24-162">Сброс таймера времени ожидания для подписки.</span><span class="sxs-lookup"><span data-stu-id="f2f24-162">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="f2f24-163">См. также</span><span class="sxs-lookup"><span data-stu-id="f2f24-163">See also</span></span>



[<span data-ttu-id="f2f24-164">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="f2f24-164">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="f2f24-165">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="f2f24-165">Unsubscribe operation</span></span>](unsubscribe-operation.md)


[<span data-ttu-id="f2f24-166">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="f2f24-166">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

