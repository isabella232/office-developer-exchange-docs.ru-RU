---
title: CreateItem (AcceptSharingInvitation)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 710c893a-3037-4f04-b336-aefedd36c406
description: Операции CreateItem используется для принятия приглашения на общий доступ к календарю другого пользователя или данных контактов.
ms.openlocfilehash: 993ef0402e624af69f632af5bdce4c02bd9d41f3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761886"
---
# <a name="createitem-acceptsharinginvitation"></a><span data-ttu-id="5efb7-103">CreateItem (AcceptSharingInvitation)</span><span class="sxs-lookup"><span data-stu-id="5efb7-103">CreateItem (AcceptSharingInvitation)</span></span>

<span data-ttu-id="5efb7-104">Операции **CreateItem** используется для принятия приглашения на общий доступ к календарю другого пользователя или данных контактов.</span><span class="sxs-lookup"><span data-stu-id="5efb7-104">The **CreateItem** operation is used to accept an invitation to share another user's calendar or contacts data.</span></span> 
  
## <a name="accept-sharing-invitation-request-example"></a><span data-ttu-id="5efb7-105">Принятие приглашения на общий доступ к пример запроса</span><span class="sxs-lookup"><span data-stu-id="5efb7-105">Accept Sharing Invitation request example</span></span>

### <a name="description"></a><span data-ttu-id="5efb7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5efb7-106">Description</span></span>

<span data-ttu-id="5efb7-107">В следующем примере показано, как для принятия приглашения на общий доступ.</span><span class="sxs-lookup"><span data-stu-id="5efb7-107">The following example shows how to accept a sharing invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="5efb7-108">Программа</span><span class="sxs-lookup"><span data-stu-id="5efb7-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Items xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <AcceptSharingInvitation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ" ChangeKey="CwAAABYAA" />
        </AcceptSharingInvitation>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5efb7-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="5efb7-109">Request elements</span></span>

<span data-ttu-id="5efb7-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5efb7-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5efb7-111">CreateItem</span><span class="sxs-lookup"><span data-stu-id="5efb7-111">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="5efb7-112">Элементы</span><span class="sxs-lookup"><span data-stu-id="5efb7-112">Items</span></span>](items.md)
    
- [<span data-ttu-id="5efb7-113">AcceptSharingInvitation</span><span class="sxs-lookup"><span data-stu-id="5efb7-113">AcceptSharingInvitation</span></span>](acceptsharinginvitation.md)
    
- [<span data-ttu-id="5efb7-114">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="5efb7-114">ReferenceItemId</span></span>](referenceitemid.md)
    
### <a name="comments"></a><span data-ttu-id="5efb7-115">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5efb7-115">Comments</span></span>

<span data-ttu-id="5efb7-116">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5efb7-116">The item identifier and change key have been shortened to preserve readability.</span></span>
  
## <a name="successful-accept-sharing-invitation-response-example"></a><span data-ttu-id="5efb7-117">Пример успешного ответа принять приглашение на общий доступ к</span><span class="sxs-lookup"><span data-stu-id="5efb7-117">Successful Accept Sharing Invitation response example</span></span>

### <a name="description"></a><span data-ttu-id="5efb7-118">Описание</span><span class="sxs-lookup"><span data-stu-id="5efb7-118">Description</span></span>

<span data-ttu-id="5efb7-119">В следующем примере показано успешного ответа на запрос **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="5efb7-119">The following example shows a successful response to a **CreateItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5efb7-120">Программа</span><span class="sxs-lookup"><span data-stu-id="5efb7-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="5efb7-121">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="5efb7-121">Successful response elements</span></span>

<span data-ttu-id="5efb7-122">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5efb7-122">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5efb7-123">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5efb7-123">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5efb7-124">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="5efb7-124">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="5efb7-125">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5efb7-125">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5efb7-126">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5efb7-126">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="5efb7-127">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5efb7-127">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5efb7-128">Элементы</span><span class="sxs-lookup"><span data-stu-id="5efb7-128">Items</span></span>](items.md)
    
## <a name="accept-sharing-invitation-error-response-example"></a><span data-ttu-id="5efb7-129">Пример ответа ошибка совместного доступа к с приглашением принять</span><span class="sxs-lookup"><span data-stu-id="5efb7-129">Accept Sharing Invitation Error response example</span></span>

### <a name="description"></a><span data-ttu-id="5efb7-130">Описание</span><span class="sxs-lookup"><span data-stu-id="5efb7-130">Description</span></span>

<span data-ttu-id="5efb7-131">В следующем примере показано ошибочный ответ на запрос **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="5efb7-131">The following example shows an error response to a **CreateItem** request.</span></span> <span data-ttu-id="5efb7-132">Ошибки, возникающие при попытке принять приглашение к совместному использованию, который не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5efb7-132">The error is caused by an attempt to accept a sharing invitation that cannot be found in the Exchange store.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5efb7-133">Программа</span><span class="sxs-lookup"><span data-stu-id="5efb7-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="5efb7-134">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="5efb7-134">Error response elements</span></span>

<span data-ttu-id="5efb7-135">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5efb7-135">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="5efb7-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5efb7-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5efb7-137">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="5efb7-137">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="5efb7-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5efb7-138">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5efb7-139">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5efb7-139">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="5efb7-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="5efb7-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5efb7-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5efb7-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5efb7-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5efb7-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="5efb7-143">Элементы</span><span class="sxs-lookup"><span data-stu-id="5efb7-143">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="5efb7-144">См. также</span><span class="sxs-lookup"><span data-stu-id="5efb7-144">See also</span></span>



[<span data-ttu-id="5efb7-145">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="5efb7-145">CreateItem operation</span></span>](createitem-operation.md)

