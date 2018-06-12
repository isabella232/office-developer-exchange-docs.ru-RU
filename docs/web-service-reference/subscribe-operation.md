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
description: Операция подписки на используется подписываться клиентских приложений в извещающей или опрашивающей уведомления. Важно необходимо учитывать, что структура сообщения запросов и ответов отличается в зависимости от типа уведомления о событии.
ms.openlocfilehash: f6cacab80c8ca2e505ab63a162a161fcf5de8585
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835619"
---
# <a name="subscribe-operation"></a><span data-ttu-id="c56a6-104">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="c56a6-104">Subscribe operation</span></span>

<span data-ttu-id="c56a6-105">Операция подписки на используется подписываться клиентских приложений в извещающей или опрашивающей уведомления.</span><span class="sxs-lookup"><span data-stu-id="c56a6-105">The Subscribe operation is used to subscribe client applications to either push or pull notifications.</span></span> <span data-ttu-id="c56a6-106">Важно необходимо учитывать, что структура сообщения запросов и ответов отличается в зависимости от типа уведомления о событии.</span><span class="sxs-lookup"><span data-stu-id="c56a6-106">It is important to be aware that the structure of the request messages and responses is different depending on the type of event notification.</span></span> 
  
## <a name="pull-subscription-subscribe-request-example"></a><span data-ttu-id="c56a6-107">Пример запроса подписки подписка репликации по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-107">Pull Subscription Subscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="c56a6-108">Описание</span><span class="sxs-lookup"><span data-stu-id="c56a6-108">Description</span></span>

<span data-ttu-id="c56a6-109">В следующем примере кода показано, как подписываться на подписку на уведомления о события репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="c56a6-109">The following code example shows how to subscribe to a pull event notification subscription.</span></span> <span data-ttu-id="c56a6-110">Подписка информирует клиентское приложение при добавлении новых сообщений в папке "Входящие" и, если элемент удален из папки «Входящие».</span><span class="sxs-lookup"><span data-stu-id="c56a6-110">The subscription informs the client application if new mail is added to the Inbox and if an item is deleted from the Inbox.</span></span> <span data-ttu-id="c56a6-111">Подписка будет времени ожидания, если клиент запрашивает сведения о событиях в течение 10 минут.</span><span class="sxs-lookup"><span data-stu-id="c56a6-111">The subscription will time out if the client does not request information about events within ten minutes.</span></span> <span data-ttu-id="c56a6-112">Если срок действия подписки, новой подписки должно быть установлено для продолжения для запроса уведомления.</span><span class="sxs-lookup"><span data-stu-id="c56a6-112">If the subscription expires, a new subscription must be established to continue to request notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="c56a6-113">Программа</span><span class="sxs-lookup"><span data-stu-id="c56a6-113">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-request-elements"></a><span data-ttu-id="c56a6-114">Элементы запроса подписка подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-114">Pull Subscription Subscribe Request Elements</span></span>

<span data-ttu-id="c56a6-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c56a6-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c56a6-116">Подписка</span><span class="sxs-lookup"><span data-stu-id="c56a6-116">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="c56a6-117">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c56a6-117">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
    
- [<span data-ttu-id="c56a6-118">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c56a6-118">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c56a6-119">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c56a6-119">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c56a6-120">EventTypes</span><span class="sxs-lookup"><span data-stu-id="c56a6-120">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="c56a6-121">EventType</span><span class="sxs-lookup"><span data-stu-id="c56a6-121">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="c56a6-122">Timeout</span><span class="sxs-lookup"><span data-stu-id="c56a6-122">Timeout</span></span>](timeout.md)
    
<span data-ttu-id="c56a6-123">Чтобы найти другие параметры для запроса подписки на операции, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="c56a6-123">To find other options for the request message of the Subscribe operation, explore the schema hierarchy.</span></span> <span data-ttu-id="c56a6-124">Запустите в элементе [PullSubscriptionRequest](pullsubscriptionrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="c56a6-124">Start at the [PullSubscriptionRequest](pullsubscriptionrequest.md) element.</span></span> 
  
## <a name="successful-pull-subscription-subscribe-response-example"></a><span data-ttu-id="c56a6-125">Успешные подписка по запросу подписки пример ответа</span><span class="sxs-lookup"><span data-stu-id="c56a6-125">Successful Pull Subscription Subscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="c56a6-126">Описание</span><span class="sxs-lookup"><span data-stu-id="c56a6-126">Description</span></span>

<span data-ttu-id="c56a6-127">В следующем примере показано ответа подписки успешной репликации по запросу.</span><span class="sxs-lookup"><span data-stu-id="c56a6-127">The following example shows a successful pull subscription response.</span></span> <span data-ttu-id="c56a6-128">Ответ содержит идентификатор подписки и водяной знак, который используется для получения массива событий, связанных с подпиской.</span><span class="sxs-lookup"><span data-stu-id="c56a6-128">The response contains the subscription identifier and watermark that is used to get the array of events that are associated with a subscription.</span></span> <span data-ttu-id="c56a6-129">Идентификатор подписки также используется для отмены подписки клиента.</span><span class="sxs-lookup"><span data-stu-id="c56a6-129">The subscription identifier is also used to unsubscribe a client from a subscription.</span></span>
  
### <a name="code"></a><span data-ttu-id="c56a6-130">Программа</span><span class="sxs-lookup"><span data-stu-id="c56a6-130">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-subscribe-response-elements"></a><span data-ttu-id="c56a6-131">Подписка подписки элементы ответа по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-131">Pull Subscription Subscribe response elements</span></span>

<span data-ttu-id="c56a6-132">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c56a6-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c56a6-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c56a6-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c56a6-134">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c56a6-134">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c56a6-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c56a6-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c56a6-136">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c56a6-136">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c56a6-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c56a6-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c56a6-138">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c56a6-138">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="c56a6-139">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="c56a6-139">Watermark</span></span>](watermark.md)
    
## <a name="pull-subscription-subscribe-error-response-example"></a><span data-ttu-id="c56a6-140">Пример ответа об ошибке подписка подписка по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-140">Pull Subscription Subscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="c56a6-141">Описание</span><span class="sxs-lookup"><span data-stu-id="c56a6-141">Description</span></span>

<span data-ttu-id="c56a6-142">В следующем примере показано ответ на запрос подписки на ошибки.</span><span class="sxs-lookup"><span data-stu-id="c56a6-142">The following example shows an error response to a Subscribe request.</span></span> <span data-ttu-id="c56a6-143">Ошибки, возникающие при при попытке подписаться на уведомления с помощью делегата клиента.</span><span class="sxs-lookup"><span data-stu-id="c56a6-143">The error is caused by an attempt to subscribe to notifications by using delegate access.</span></span>
  
### <a name="code"></a><span data-ttu-id="c56a6-144">Программа</span><span class="sxs-lookup"><span data-stu-id="c56a6-144">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="pull-subscription-error-response-elements"></a><span data-ttu-id="c56a6-145">Элементы ответа об ошибке подписка по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-145">Pull Subscription Error response elements</span></span>

<span data-ttu-id="c56a6-146">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c56a6-146">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="c56a6-147">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c56a6-147">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c56a6-148">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c56a6-148">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c56a6-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c56a6-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c56a6-150">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c56a6-150">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c56a6-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="c56a6-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="c56a6-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c56a6-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c56a6-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c56a6-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="push-subscription-request-example"></a><span data-ttu-id="c56a6-154">Пример запроса Push подписки</span><span class="sxs-lookup"><span data-stu-id="c56a6-154">Push Subscription request example</span></span>

### <a name="description"></a><span data-ttu-id="c56a6-155">Описание</span><span class="sxs-lookup"><span data-stu-id="c56a6-155">Description</span></span>

<span data-ttu-id="c56a6-156">В следующем примере кода показано, как подписываться на события уведомления принудительной подписки.</span><span class="sxs-lookup"><span data-stu-id="c56a6-156">The following code example shows how to subscribe to a push event notification subscription.</span></span> <span data-ttu-id="c56a6-157">Запрос определяет папки для отслеживания, типы событий для отслеживания, частота уведомления о состоянии и URL-адрес клиента веб-службы, который прослушивает push-уведомлений.</span><span class="sxs-lookup"><span data-stu-id="c56a6-157">The request identifies the folders to monitor, the types of events to monitor, the frequency of status notifications, and the URL of the client Web service that listens for the push notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="c56a6-158">Программа</span><span class="sxs-lookup"><span data-stu-id="c56a6-158">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Subscribe xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <PushSubscriptionRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <FolderIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <DistinguishedFolderId Id="inbox" />
        </FolderIds>
        <EventTypes xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <EventType>NewMailEvent</EventType>
          <EventType>CopiedEvent</EventType>
          <EventType>CreatedEvent</EventType>
          <EventType>DeletedEvent</EventType>
          <EventType>ModifiedEvent</EventType>
          <EventType>MovedEvent</EventType>
        </EventTypes>
        <StatusFrequency xmlns="http://schemas.microsoft.com/exchange/services/2006/types">1</StatusFrequency>
        <URL xmlns="http://schemas.microsoft.com/exchange/services/2006/types">http://clientWebService/Service.asmx</URL>
      </PushSubscriptionRequest>
    </Subscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="c56a6-159">Комментарии</span><span class="sxs-lookup"><span data-stu-id="c56a6-159">Comments</span></span>

<span data-ttu-id="c56a6-160">Клиент Web службы необходимо настроить перед push-уведомлений подписка запрос отправляется; в противном случае первого уведомления не будут отправляться допустимый конечную точку и push-уведомлений завершится с ошибкой.</span><span class="sxs-lookup"><span data-stu-id="c56a6-160">The client Web service must be set up before the push notification subscribe request is sent; otherwise, the first notification will not be sent to a valid endpoint and the push notification will fail.</span></span> <span data-ttu-id="c56a6-161">Для получения дополнительных сведений см [Push-уведомлений пример приложения](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="c56a6-161">For more information, see [Push Notification Sample Application](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx).</span></span>
  
<span data-ttu-id="c56a6-162">Новые [SubscriptionId (GetEvents)](subscriptionid-getevents.md) создается, когда вы повторная.</span><span class="sxs-lookup"><span data-stu-id="c56a6-162">A new [SubscriptionId (GetEvents)](subscriptionid-getevents.md) is created when you resubscribe.</span></span> <span data-ttu-id="c56a6-163">Используйте водяного знака предыдущей подписки для повторная в точке, где заканчивается предыдущей подписки.</span><span class="sxs-lookup"><span data-stu-id="c56a6-163">Use the watermark of a previous subscription to resubscribe at the point where the previous subscription ended.</span></span> 
  
### <a name="push-subscription-request-elements"></a><span data-ttu-id="c56a6-164">Push-элементы запрос подписки</span><span class="sxs-lookup"><span data-stu-id="c56a6-164">Push Subscription Request Elements</span></span>

<span data-ttu-id="c56a6-165">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c56a6-165">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c56a6-166">Подписка</span><span class="sxs-lookup"><span data-stu-id="c56a6-166">Subscribe</span></span>](subscribe.md)
    
- [<span data-ttu-id="c56a6-167">PushSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="c56a6-167">PushSubscriptionRequest</span></span>](pushsubscriptionrequest.md)
    
- [<span data-ttu-id="c56a6-168">FolderIds</span><span class="sxs-lookup"><span data-stu-id="c56a6-168">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="c56a6-169">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c56a6-169">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="c56a6-170">EventTypes</span><span class="sxs-lookup"><span data-stu-id="c56a6-170">EventTypes</span></span>](eventtypes.md)
    
- [<span data-ttu-id="c56a6-171">EventType</span><span class="sxs-lookup"><span data-stu-id="c56a6-171">EventType</span></span>](eventtype.md)
    
- [<span data-ttu-id="c56a6-172">StatusFrequency</span><span class="sxs-lookup"><span data-stu-id="c56a6-172">StatusFrequency</span></span>](statusfrequency.md)
    
- [<span data-ttu-id="c56a6-173">URL-адрес</span><span class="sxs-lookup"><span data-stu-id="c56a6-173">Url </span></span>](url-ex15websvcsotherref.md)
    
## <a name="successful-push-subscription-response-example"></a><span data-ttu-id="c56a6-174">Пример ответа успешной Push-подписки</span><span class="sxs-lookup"><span data-stu-id="c56a6-174">Successful Push Subscription response example</span></span>

### <a name="description"></a><span data-ttu-id="c56a6-175">Описание</span><span class="sxs-lookup"><span data-stu-id="c56a6-175">Description</span></span>

<span data-ttu-id="c56a6-176">В следующем примере показано ответа подписки успешно выполненных push.</span><span class="sxs-lookup"><span data-stu-id="c56a6-176">The following example shows a successful push subscription response.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c56a6-177">Программа</span><span class="sxs-lookup"><span data-stu-id="c56a6-177">Code</span></span>

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
    <SubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="push-subscription-response-elements"></a><span data-ttu-id="c56a6-178">Push-элементы ответа подписки</span><span class="sxs-lookup"><span data-stu-id="c56a6-178">Push Subscription response elements</span></span>

<span data-ttu-id="c56a6-179">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c56a6-179">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c56a6-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c56a6-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c56a6-181">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="c56a6-181">SubscribeResponse</span></span>](subscriberesponse.md)
    
- [<span data-ttu-id="c56a6-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c56a6-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="c56a6-183">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c56a6-183">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
    
- [<span data-ttu-id="c56a6-184">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c56a6-184">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="c56a6-185">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="c56a6-185">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
- [<span data-ttu-id="c56a6-186">Водяной знак</span><span class="sxs-lookup"><span data-stu-id="c56a6-186">Watermark</span></span>](watermark.md)
    
## <a name="see-also"></a><span data-ttu-id="c56a6-187">См. также</span><span class="sxs-lookup"><span data-stu-id="c56a6-187">See also</span></span>



[<span data-ttu-id="c56a6-188">Отписаться операции</span><span class="sxs-lookup"><span data-stu-id="c56a6-188">Unsubscribe operation</span></span>](unsubscribe-operation.md)
  
[<span data-ttu-id="c56a6-189">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="c56a6-189">GetEvents operation</span></span>](getevents-operation.md)


[<span data-ttu-id="c56a6-190">С помощью подписки по запросу</span><span class="sxs-lookup"><span data-stu-id="c56a6-190">Using Pull Subscriptions</span></span>](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)
  
[<span data-ttu-id="c56a6-191">Пример приложения для push-уведомлений</span><span class="sxs-lookup"><span data-stu-id="c56a6-191">Push Notification Sample Application</span></span>](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

