---
title: Операция GetStreamingEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEvents
api_type:
- schema
ms.assetid: 8da95423-72bc-4034-90a8-162eedcd059b
description: Найдите сведения о веб-служб Exchange GetStreamingEvents операции.
ms.openlocfilehash: 0e93be7b14cb1ca6a2a9821b016f7bdc0e8d7772
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833673"
---
# <a name="getstreamingevents-operation"></a><span data-ttu-id="405df-103">Операция GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-103">GetStreamingEvents operation</span></span>

<span data-ttu-id="405df-104">Найдите сведения о **GetStreamingEvents** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="405df-104">Find information about the **GetStreamingEvents** EWS operation.</span></span> 
  
<span data-ttu-id="405df-105">Операция **GetStreamingEvents** используется потоковая передача клиенты подписки для запроса уведомлений с сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="405df-105">The **GetStreamingEvents** operation is used by streaming subscription clients to request notifications from the Client Access server.</span></span> <span data-ttu-id="405df-106">Ответ **GetStreamingEvents** возвращает массив элементов и события, которые происходили в почтовом ящике с момента последнего уведомления.</span><span class="sxs-lookup"><span data-stu-id="405df-106">The **GetStreamingEvents** response returns an array of items and events that have occurred in a mailbox since the last the notification.</span></span> 
  
## <a name="getstreamingevents-request-example"></a><span data-ttu-id="405df-107">Пример запроса GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-107">GetStreamingEvents request example</span></span>

### <a name="description"></a><span data-ttu-id="405df-108">Описание</span><span class="sxs-lookup"><span data-stu-id="405df-108">Description</span></span>

<span data-ttu-id="405df-109">В следующем примере операция **GetStreamingEvents** показано, как запросить событий и элементы, связанные с подпиской, который идентифицируется по идентификатору подписки.</span><span class="sxs-lookup"><span data-stu-id="405df-109">The following example of a **GetStreamingEvents** operation shows how to request the events and items that are associated with a subscription that is identified by the subscription identifier.</span></span> 
  
### <a name="code"></a><span data-ttu-id="405df-110">Программа</span><span class="sxs-lookup"><span data-stu-id="405df-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
  xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Body>
    <GetStreamingEvents xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</SubscriptionId>
      <ConnectionTimeout>30</ConnectionTimeout>
    </GetStreamingEvents>
  </soap:Body>
</soap:Envelope>
```

### <a name="getstreamingevents-request-elements"></a><span data-ttu-id="405df-111">Элементы запроса GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-111">GetStreamingEvents request elements</span></span>

<span data-ttu-id="405df-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="405df-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="405df-113">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-113">GetStreamingEvents</span></span>](getstreamingevents.md)
    
- [<span data-ttu-id="405df-114">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="405df-114">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
- [<span data-ttu-id="405df-115">ConnectionTimeout</span><span class="sxs-lookup"><span data-stu-id="405df-115">ConnectionTimeout</span></span>](connectiontimeout.md)
    
## <a name="successful-getstreamingevents-response-example"></a><span data-ttu-id="405df-116">Пример успешного ответа GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-116">Successful GetStreamingEvents response example</span></span>

### <a name="description"></a><span data-ttu-id="405df-117">Описание</span><span class="sxs-lookup"><span data-stu-id="405df-117">Description</span></span>

<span data-ttu-id="405df-118">В следующем примере ответа **GetStreamingEvents** показано уведомлений, отправленных в клиенте при получении нового сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="405df-118">The following example of a **GetStreamingEvents** response shows the notifications that are sent to the client when a new email message is received.</span></span> <span data-ttu-id="405df-119">Включает уведомления для следующих событий: CreatedEvent, NewMail и ModifiedEvent.</span><span class="sxs-lookup"><span data-stu-id="405df-119">It includes notifications for the following events: CreatedEvent, NewMail, and ModifiedEvent.</span></span> 
  
### <a name="code"></a><span data-ttu-id="405df-120">Программа</span><span class="sxs-lookup"><span data-stu-id="405df-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Header xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <ServerVersionInfo xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="7" Version="V2_4" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
</soap:Header>
<soap:Body xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <m:GetStreamingEventsResponse xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
    <m:ResponseMessages>
      <m:GetStreamingEventsResponseMessage ResponseClass="Success">
        <m:ResponseCode>NoError</m:ResponseCode>
        <m:Notifications>
          <m:Notification>
            <t:SubscriptionId>f6bc657d-dde1-4f94-952d-143b95d6483d</t:SubscriptionId>
            <t:CreatedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:CreatedEvent>
            <t:NewMailEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:ItemId Id="AAMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwBGAAAAAABSSWVKrmGUTJE+MVIvofglBwDZGACZQpSgSpyNkexYe2b7AAAAAAENAADZGACZQpSgSpyNkexYe2b7AAANGFYwAAA=" ChangeKey="CQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
            </t:NewMailEvent>
            <t:ModifiedEvent>
              <t:TimeStamp>2013-09-16T04:31:29Z</t:TimeStamp>
              <t:FolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgENAAAA" ChangeKey="AQAAAA==" />
              <t:ParentFolderId Id="AQMkADkzNjJjODUzLWZhMDMtNDVkMS05ZDdjLWVmMDlkYjQ1Zjc4MwAuAAADUkllSq5hlEyRPjFSL6H4JQEA2RgAmUKUoEqcjZHsWHtm+wAAAgEJAAAA" ChangeKey="AQAAAA==" />
              <t:UnreadCount>1</t:UnreadCount>
            </t:ModifiedEvent>
          </m:Notification>
        </m:Notifications>
      </m:GetStreamingEventsResponseMessage>
    </m:ResponseMessages>
  </m:GetStreamingEventsResponse>
</soap:Body>
```

### <a name="getstreamingevents-response-elements"></a><span data-ttu-id="405df-121">Элементы ответов GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-121">GetStreamingEvents response elements</span></span>

<span data-ttu-id="405df-122">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="405df-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="405df-123">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="405df-123">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
    
- [<span data-ttu-id="405df-124">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="405df-124">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="405df-125">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="405df-125">GetStreamingEventsResponseMessage</span></span>](getstreamingeventsresponsemessage.md)
    
- [<span data-ttu-id="405df-126">NotesFolderPermissionLevel</span><span class="sxs-lookup"><span data-stu-id="405df-126">NotesFolderPermissionLevel</span></span>](notesfolderpermissionlevel.md)
    
- [<span data-ttu-id="405df-127">Уведомление</span><span class="sxs-lookup"><span data-stu-id="405df-127">Notification</span></span>](notification-ex15websvcsotherref.md)
    
- [<span data-ttu-id="405df-128">SubscriptionId (GetStreamingEvents)</span><span class="sxs-lookup"><span data-stu-id="405df-128">SubscriptionId (GetStreamingEvents)</span></span>](subscriptionid-getstreamingevents.md)
    
<span data-ttu-id="405df-129">Чтобы найти другие параметры в сообщении ответа **GetStreamingEvents** операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="405df-129">To find other options for the response message of the **GetStreamingEvents** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="405df-130">Запустите на элементе [уведомлений](notification-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="405df-130">Start at the [Notification](notification-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="getstreamingevents-error-response-example"></a><span data-ttu-id="405df-131">Пример ответа об ошибке GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="405df-131">GetStreamingEvents error response example</span></span>

### <a name="description"></a><span data-ttu-id="405df-132">Описание</span><span class="sxs-lookup"><span data-stu-id="405df-132">Description</span></span>

<span data-ttu-id="405df-133">В следующем примере показано ошибочный ответ на запрос **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="405df-133">The following example shows an error response to a **GetStreamingEvents** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="405df-134">Программа</span><span class="sxs-lookup"><span data-stu-id="405df-134">Code</span></span>

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
    <GetStreamingEventsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetStreamingEventsResponseMessage ResponseClass="Error">
        <m:MessageText></m:MessageText>
        <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        <m:ResponseCode>ErrorInvalidSubscription</m:ResponseCode>
        <m:ConnectionStatus>Closed</m:ConnectionStatus>
      </m:ResponseMessages>
    </GetStreamingEventsResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="remarks"></a><span data-ttu-id="405df-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="405df-135">Remarks</span></span>

<span data-ttu-id="405df-136">При обработке запроса **GetStreamingEvents** , сервера клиентского доступа необходимо выполнить следующие действия:</span><span class="sxs-lookup"><span data-stu-id="405df-136">When processing a **GetStreamingEvents** request, the Client Access server performs the following steps:</span></span> 
  
1. <span data-ttu-id="405df-137">[SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) запроса подтверждения действительную подписку, размещенного на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="405df-137">The [SubscriptionId (GetStreamingEvents)](subscriptionid-getstreamingevents.md) of the request is confirmed to be a valid subscription that is hosted on the Client Access server.</span></span> <span data-ttu-id="405df-138">Если он не установлен, **GetStreamingEvents** завершается неудачно.</span><span class="sxs-lookup"><span data-stu-id="405df-138">If it is not, the **GetStreamingEvents** call fails.</span></span> 
    
2. <span data-ttu-id="405df-139">SMTP-адрес пользователя, прошедшего проверку подлинности для запроса проверяется на наличие прав олицетворения.</span><span class="sxs-lookup"><span data-stu-id="405df-139">The SMTP address of the authenticated user for the request is validated to have impersonation rights.</span></span> <span data-ttu-id="405df-140">Если нет, не удается выполнить запрос **GetStreamingEvents** .</span><span class="sxs-lookup"><span data-stu-id="405df-140">If they do not, the **GetStreamingEvents** request fails.</span></span> 
    
3. <span data-ttu-id="405df-141">Очередь подписки будет опрошен на наличие событий, ожидающих отправляются клиенту.</span><span class="sxs-lookup"><span data-stu-id="405df-141">The subscription queue is queried for events that are waiting to be sent to the client.</span></span> <span data-ttu-id="405df-142">Если очередь не является пустым, первые 50 события из очереди, которые извлекаются из очереди и кодируются в уведомление.</span><span class="sxs-lookup"><span data-stu-id="405df-142">If the queue is not empty, the first 50 events from the queue are pulled from the queue and encoded into a notification.</span></span>
    
4. <span data-ttu-id="405df-143">Если события не обнаружены в очереди, [StatusEvent](statusevent.md) создан и кодируются в ответ уведомлений.</span><span class="sxs-lookup"><span data-stu-id="405df-143">If no events are found in the queue, a [StatusEvent](statusevent.md) is generated and encoded into a notification response.</span></span> 
    
5. <span data-ttu-id="405df-144">Уведомление ответ возвращается клиенту.</span><span class="sxs-lookup"><span data-stu-id="405df-144">The notification response is returned to the client.</span></span>
    
6. <span data-ttu-id="405df-145">События, включенные в уведомлении, удаляются из очереди подписки, водяной знак последнего локального сервера клиентского доступа для подписки на задано значение водяной знак последнего события, который возвращается.</span><span class="sxs-lookup"><span data-stu-id="405df-145">The events that are included in the notification are removed from the subscription queue and the Client Access server-local last watermark for the subscription is set to the watermark of the last event that is returned.</span></span>
    
7. <span data-ttu-id="405df-146">Сброс таймера времени ожидания для подписки.</span><span class="sxs-lookup"><span data-stu-id="405df-146">The timeout timer for the subscription is reset.</span></span>
    
## <a name="see-also"></a><span data-ttu-id="405df-147">См. также</span><span class="sxs-lookup"><span data-stu-id="405df-147">See also</span></span>



[<span data-ttu-id="405df-148">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="405df-148">Subscribe operation</span></span>](subscribe-operation.md)
  
[<span data-ttu-id="405df-149">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="405df-149">Unsubscribe operation</span></span>](unsubscribe-operation.md)

