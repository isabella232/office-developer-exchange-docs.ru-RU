---
title: Операция по отмене подписки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: Операция unsubscribe используется для завершения подписки на уведомления по запросу. Используйте эту операцию вместо времени ожидания подписки. Эта операция допустима только для уведомлений о опрашивающей репликации.
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468028"
---
# <a name="unsubscribe-operation"></a><span data-ttu-id="46886-105">Операция по отмене подписки</span><span class="sxs-lookup"><span data-stu-id="46886-105">Unsubscribe operation</span></span>

<span data-ttu-id="46886-106">Операция unsubscribe используется для завершения подписки на уведомления по запросу.</span><span class="sxs-lookup"><span data-stu-id="46886-106">The Unsubscribe operation is used to end a pull notification subscription.</span></span> <span data-ttu-id="46886-107">Используйте эту операцию вместо времени ожидания подписки.</span><span class="sxs-lookup"><span data-stu-id="46886-107">Use this operation rather than letting a subscription timeout.</span></span> <span data-ttu-id="46886-108">Эта операция допустима только для уведомлений о опрашивающей репликации.</span><span class="sxs-lookup"><span data-stu-id="46886-108">This operation is only valid for pull notifications.</span></span>
  
## <a name="unsubscribe-request-example"></a><span data-ttu-id="46886-109">Пример запроса unsubscribe</span><span class="sxs-lookup"><span data-stu-id="46886-109">Unsubscribe request example</span></span>

### <a name="description"></a><span data-ttu-id="46886-110">Description</span><span class="sxs-lookup"><span data-stu-id="46886-110">Description</span></span>

<span data-ttu-id="46886-111">В следующем примере показано SOAP-сообщение SOAP, отправляемое для отмены подписки клиента из службы уведомлений.</span><span class="sxs-lookup"><span data-stu-id="46886-111">The following example shows the SOAP XML message that is sent to unsubscribe a client from the Notification service.</span></span>
  
### <a name="code"></a><span data-ttu-id="46886-112">Код</span><span class="sxs-lookup"><span data-stu-id="46886-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a><span data-ttu-id="46886-113">Элементы запроса отменять подписку</span><span class="sxs-lookup"><span data-stu-id="46886-113">Unsubscribe request elements</span></span>

<span data-ttu-id="46886-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46886-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="46886-115">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="46886-115">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="46886-116">SubscriptionId (Events)</span><span class="sxs-lookup"><span data-stu-id="46886-116">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a><span data-ttu-id="46886-117">Пример успешного отклика отмены подписки</span><span class="sxs-lookup"><span data-stu-id="46886-117">Successful Unsubscribe response example</span></span>

### <a name="description"></a><span data-ttu-id="46886-118">Description</span><span class="sxs-lookup"><span data-stu-id="46886-118">Description</span></span>

<span data-ttu-id="46886-119">В следующем примере показан успешный ответ на запрос отказа от подписки.</span><span class="sxs-lookup"><span data-stu-id="46886-119">The following example shows a successful response to an Unsubscribe request.</span></span>
  
### <a name="code"></a><span data-ttu-id="46886-120">Код</span><span class="sxs-lookup"><span data-stu-id="46886-120">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a><span data-ttu-id="46886-121">Элементы отклика для отмены подписки</span><span class="sxs-lookup"><span data-stu-id="46886-121">Unsubscribe response elements</span></span>

<span data-ttu-id="46886-122">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46886-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="46886-123">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="46886-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46886-124">Отмена подписки</span><span class="sxs-lookup"><span data-stu-id="46886-124">Unsubscribe</span></span>](unsubscribe.md)
    
- [<span data-ttu-id="46886-125">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="46886-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46886-126">унсубскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="46886-126">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="46886-127">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="46886-127">ResponseCode</span></span>](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a><span data-ttu-id="46886-128">Пример отклика об отмене подписки</span><span class="sxs-lookup"><span data-stu-id="46886-128">Unsubscribe Error response example</span></span>

### <a name="description"></a><span data-ttu-id="46886-129">Description</span><span class="sxs-lookup"><span data-stu-id="46886-129">Description</span></span>

<span data-ttu-id="46886-130">Следующий пример ответа об отказе от подписки возникает в ответ на попытку отменить подписку с помощью идентификатора подписки, который не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="46886-130">The following example of an Unsubscribe error response occurs in response to an attempt to unsubscribe by using a subscription identifier that cannot be located in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="46886-131">Код</span><span class="sxs-lookup"><span data-stu-id="46886-131">Code</span></span>

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
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a><span data-ttu-id="46886-132">Элементы отклика на сообщение об ошибке отклика</span><span class="sxs-lookup"><span data-stu-id="46886-132">Unsubscribe Error response elements</span></span>

<span data-ttu-id="46886-133">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="46886-133">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="46886-134">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="46886-134">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="46886-135">унсубскрибереспонсе</span><span class="sxs-lookup"><span data-stu-id="46886-135">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
    
- [<span data-ttu-id="46886-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="46886-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="46886-137">унсубскрибереспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="46886-137">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
    
- [<span data-ttu-id="46886-138">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="46886-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="46886-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="46886-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="46886-140">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="46886-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="46886-141">См. также</span><span class="sxs-lookup"><span data-stu-id="46886-141">See also</span></span>

- [<span data-ttu-id="46886-142">Операции подписки</span><span class="sxs-lookup"><span data-stu-id="46886-142">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="46886-143">Операция GetEvents</span><span class="sxs-lookup"><span data-stu-id="46886-143">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="46886-144">Использование подписок по запросу</span><span class="sxs-lookup"><span data-stu-id="46886-144">Using Pull Subscriptions</span></span>](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

