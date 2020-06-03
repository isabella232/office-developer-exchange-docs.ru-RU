---
title: Операции подписки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subscribe
api_type:
- schema
ms.assetid: f17c3d08-c79e-41f1-ba31-6e41e7aafd87
description: Операция Subscribe используется для подписки клиентских приложений на Push-или опрашивающие уведомления. Важно знать, что структура сообщений запросов и ответов различается в зависимости от типа уведомления о событии.
ms.openlocfilehash: c40e0e434f698c6535ff5d03fd4d45a453959dd6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467048"
---
# <a name="subscribe-operation"></a><span data-ttu-id="30d15-104">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="30d15-104">Subscribe operation</span></span>

<span data-ttu-id="30d15-105">Операция Subscribe используется для подписки клиентских приложений на Push-или опрашивающие уведомления.</span><span class="sxs-lookup"><span data-stu-id="30d15-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="30d15-106">Важно знать, что структура сообщений запросов и ответов различается в зависимости от типа уведомления о событии.</span><span class="sxs-lookup"><span data-stu-id="30d15-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="30d15-107">Пример запроса на получение подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="30d15-108">Description</span><span class="sxs-lookup"><span data-stu-id="30d15-108">Description</span></span>

<span data-ttu-id="30d15-109">В приведенном ниже примере кода показано, как подписаться на подписку на уведомления о событиях опрашивающей репликации.</span><span class="sxs-lookup"><span data-stu-id="30d15-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="30d15-110">Подписка информирует клиентское приложение о добавлении новой почты в папку "Входящие" и удалении элемента из папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="30d15-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="30d15-111">Если клиент не запрашивает сведения о событиях в течение десяти минут, произойдет время ожидания подписки.</span><span class="sxs-lookup"><span data-stu-id="30d15-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="30d15-112">Если срок действия подписки истечет, необходимо установить новую подписку, чтобы продолжить запрашивать уведомления.</span><span class="sxs-lookup"><span data-stu-id="30d15-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="30d15-113">Код</span><span class="sxs-lookup"><span data-stu-id="30d15-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <PullSubscriptionRequest>
        <t:FolderIds>
          <t:DistinguishedFolderId Id="inbox"/>
        </t:FolderIds>
        <t:EventTypes>
          <t:EventType>NewMailEvent</t:EventType>
          <t:EventType>DeletedEvent</t:EventType>
        </t:EventTypes>
        <t:Timeout>10</t:Timeout>
      </PullSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="30d15-114">Элементы запроса подписки по запросу на получение подписки</span><span class="sxs-lookup"><span data-stu-id="30d15-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="30d15-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30d15-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="30d15-116">Подписаться</span><span class="sxs-lookup"><span data-stu-id="30d15-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="30d15-117">пуллсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="30d15-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="30d15-118">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="30d15-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="30d15-119">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="30d15-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="30d15-120">евенттипес</span><span class="sxs-lookup"><span data-stu-id="30d15-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="30d15-121">EventType</span><span class="sxs-lookup"><span data-stu-id="30d15-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="30d15-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="30d15-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="30d15-123">Чтобы найти другие варианты сообщения запроса операции Subscribe, изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="30d15-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="30d15-124">Начните с элемента [пуллсубскриптионрекуест](pullsubscriptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="30d15-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="30d15-125">Пример успешных откликов подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="30d15-126">Description</span><span class="sxs-lookup"><span data-stu-id="30d15-126">Description</span></span>

<span data-ttu-id="30d15-127">В следующем примере показан успешный ответ на подписку по запросу.</span><span class="sxs-lookup"><span data-stu-id="30d15-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="30d15-128">Ответ содержит идентификатор и водяной знак подписки, которые используются для получения массива событий, связанных с подпиской.</span><span class="sxs-lookup"><span data-stu-id="30d15-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="30d15-129">Идентификатор подписки также используется для отказа от подписки клиента из подписки.</span><span class="sxs-lookup"><span data-stu-id="30d15-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="30d15-130">Код</span><span class="sxs-lookup"><span data-stu-id="30d15-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:SubscriptionId>39ea5d0f-f062-455e-a1e9-89c0304390f4</m:SubscriptionId>
          <m:Watermark>AAAAAHgGAAAAAAAAAQ==</m:Watermark>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="30d15-131">Элементы ответа на подписку по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="30d15-132">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30d15-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="30d15-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="30d15-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30d15-134">субскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="30d15-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="30d15-135">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="30d15-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30d15-136">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="30d15-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="30d15-137">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="30d15-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30d15-138">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="30d15-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="30d15-139">Watermark</span><span class="sxs-lookup"><span data-stu-id="30d15-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="30d15-140">Пример ответа на сообщение об ошибке подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="30d15-141">Description</span><span class="sxs-lookup"><span data-stu-id="30d15-141">Description</span></span>

<span data-ttu-id="30d15-142">В приведенном ниже примере показан ответ об ошибке запроса на подписку.</span><span class="sxs-lookup"><span data-stu-id="30d15-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="30d15-143">Ошибка вызвана попыткой подписаться на уведомления с помощью делегированного доступа.</span><span class="sxs-lookup"><span data-stu-id="30d15-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="30d15-144">Код</span><span class="sxs-lookup"><span data-stu-id="30d15-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>Subscriptions are not supported for delegate user access.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionDelegateAccessNotSupported</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SubscribeResponseMessage>
      </m:ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="30d15-145">Элементы ответа об ошибке подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="30d15-146">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30d15-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="30d15-147">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="30d15-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30d15-148">субскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="30d15-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="30d15-149">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="30d15-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30d15-150">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="30d15-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="30d15-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="30d15-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="30d15-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="30d15-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30d15-153">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="30d15-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="30d15-154">Пример запроса на принудительную подписку</span><span class="sxs-lookup"><span data-stu-id="30d15-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="30d15-155">Description</span><span class="sxs-lookup"><span data-stu-id="30d15-155">Description</span></span>

<span data-ttu-id="30d15-156">В следующем примере кода показано, как подписаться на подписку на push-уведомления о событиях.</span><span class="sxs-lookup"><span data-stu-id="30d15-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="30d15-157">Запрос определяет папки для мониторинга, типы событий для отслеживания, частоту уведомлений о состоянии и URL-адрес веб-службы клиента, которая прослушивает push-уведомления.</span><span class="sxs-lookup"><span data-stu-id="30d15-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="30d15-158">Код</span><span class="sxs-lookup"><span data-stu-id="30d15-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="https://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="https://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="30d15-159">Комментарии</span><span class="sxs-lookup"><span data-stu-id="30d15-159">Comments</span></span>

<span data-ttu-id="30d15-160">Клиентская веб-служба должна быть настроена перед отправкой запроса на подписку с Push-уведомлениями; в противном случае первое уведомление не будет отправлено в действительную конечную точку, а push-уведомление завершится с ошибками.</span><span class="sxs-lookup"><span data-stu-id="30d15-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="30d15-161">Для получения дополнительных сведений обратитесь к разделу [пример приложения push-уведомлений](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="30d15-161">For more information, see [Push Notification Sample Application](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="30d15-162">При повторной подписку создается новый идентификатор [SubscriptionId (Events)](subscriptionid-getevents.md) .</span><span class="sxs-lookup"><span data-stu-id="30d15-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="30d15-163">Использование водяного знака предыдущей подписки для повторной подписки на момент окончания предыдущей подписки.</span><span class="sxs-lookup"><span data-stu-id="30d15-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="30d15-164">Элементы запроса на принудительную подписку</span><span class="sxs-lookup"><span data-stu-id="30d15-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="30d15-165">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30d15-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="30d15-166">Подписаться</span><span class="sxs-lookup"><span data-stu-id="30d15-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="30d15-167">пушсубскриптионрекуест</span><span class="sxs-lookup"><span data-stu-id="30d15-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="30d15-168">фолдеридс</span><span class="sxs-lookup"><span data-stu-id="30d15-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="30d15-169">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="30d15-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="30d15-170">евенттипес</span><span class="sxs-lookup"><span data-stu-id="30d15-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="30d15-171">EventType</span><span class="sxs-lookup"><span data-stu-id="30d15-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="30d15-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="30d15-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="30d15-173">Адрес</span><span class="sxs-lookup"><span data-stu-id="30d15-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="30d15-174">Пример успешной принудительной подписки</span><span class="sxs-lookup"><span data-stu-id="30d15-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="30d15-175">Description</span><span class="sxs-lookup"><span data-stu-id="30d15-175">Description</span></span>

<span data-ttu-id="30d15-176">В следующем примере показан успешный ответ на принудительную подписку.</span><span class="sxs-lookup"><span data-stu-id="30d15-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="30d15-177">Код</span><span class="sxs-lookup"><span data-stu-id="30d15-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessages>
        <SubscribeResponseMessage ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <SubscriptionId>83826921-afdf-48be-b469-628cc02b5f49</SubscriptionId>
          <Watermark>AQAAAOpvG0LURVdOhQkPOWZLPcI8EgAAAAAAAAE=</Watermark>
        </SubscribeResponseMessage>
      </ResponseMessages>
    </SubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="push-subscription-response-elements"></a><span data-ttu-id="30d15-178">Элементы ответа на принудительную подписку</span><span class="sxs-lookup"><span data-stu-id="30d15-178">Push Subscription response elements</span></span>

<span data-ttu-id="30d15-179">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="30d15-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="30d15-180">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="30d15-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="30d15-181">субскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="30d15-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="30d15-182">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="30d15-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="30d15-183">субскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="30d15-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="30d15-184">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="30d15-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="30d15-185">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="30d15-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="30d15-186">Watermark</span><span class="sxs-lookup"><span data-stu-id="30d15-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="30d15-187">См. также</span><span class="sxs-lookup"><span data-stu-id="30d15-187">See also</span></span>



[<span data-ttu-id="30d15-188">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="30d15-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="30d15-189">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="30d15-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="30d15-190">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="30d15-190">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="30d15-191">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="30d15-191">Push Notification Sample Application</span></span>](https://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

