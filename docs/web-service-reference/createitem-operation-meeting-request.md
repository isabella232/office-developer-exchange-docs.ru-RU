---
title: Операции CreateItem (запрос на собрание)
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
ms.assetid: fe136881-a804-456a-8552-8a1bea5eb9c8
description: Операция CreateItem используется в ответ на приглашения на собрания.
ms.openlocfilehash: a8aea688e46376906554952ce8ec45022cf613e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761895"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="49c64-103">Операции CreateItem (запрос на собрание)</span><span class="sxs-lookup"><span data-stu-id="49c64-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="49c64-104">Операция CreateItem используется в ответ на приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="49c64-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49c64-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="49c64-105">Remarks</span></span>

<span data-ttu-id="49c64-106">Операции CreateItem предоставляет три варианта реагирования на приглашения на собрание: принять, под вопросом принять или отклонить.</span><span class="sxs-lookup"><span data-stu-id="49c64-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="49c64-107">Примите примере запрос на собрание</span><span class="sxs-lookup"><span data-stu-id="49c64-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="49c64-108">Описание</span><span class="sxs-lookup"><span data-stu-id="49c64-108">Description</span></span>

<span data-ttu-id="49c64-109">Следующий пример демонстрирует приняли приглашение на собрание запроса приглашения.</span><span class="sxs-lookup"><span data-stu-id="49c64-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="49c64-110">Программа</span><span class="sxs-lookup"><span data-stu-id="49c64-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="49c64-111">Комментарии</span><span class="sxs-lookup"><span data-stu-id="49c64-111">Comments</span></span>

<span data-ttu-id="49c64-112">Чтобы принять под вопросом или отклонить приглашение на собрание, используйте [TentativelyAcceptItem](tentativelyacceptitem.md) или [DeclineItem](declineitem.md) элементов вместо [AcceptItem](acceptitem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="49c64-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="49c64-113">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="49c64-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="49c64-114">Принятие элементы запроса на собрание</span><span class="sxs-lookup"><span data-stu-id="49c64-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="49c64-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49c64-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="49c64-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="49c64-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="49c64-117">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="49c64-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="49c64-118">AcceptItem</span><span class="sxs-lookup"><span data-stu-id="49c64-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="49c64-119">ReferenceItemId</span><span class="sxs-lookup"><span data-stu-id="49c64-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="49c64-120">Успешные пример ответа принимать собрания</span><span class="sxs-lookup"><span data-stu-id="49c64-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="49c64-121">Описание</span><span class="sxs-lookup"><span data-stu-id="49c64-121">Description</span></span>

<span data-ttu-id="49c64-122">В следующем примере показано успешного ответа на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="49c64-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="49c64-123">Программа</span><span class="sxs-lookup"><span data-stu-id="49c64-123">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="49c64-124">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="49c64-124">Successful response elements</span></span>

<span data-ttu-id="49c64-125">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49c64-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="49c64-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="49c64-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="49c64-127">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="49c64-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="49c64-128">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="49c64-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="49c64-129">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49c64-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="49c64-130">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="49c64-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="49c64-131">Элементы</span><span class="sxs-lookup"><span data-stu-id="49c64-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="49c64-132">Примите пример ответа об ошибке собрания</span><span class="sxs-lookup"><span data-stu-id="49c64-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="49c64-133">Описание</span><span class="sxs-lookup"><span data-stu-id="49c64-133">Description</span></span>

<span data-ttu-id="49c64-134">В следующем примере показано отклик на запрос CreateItem ошибку.</span><span class="sxs-lookup"><span data-stu-id="49c64-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="49c64-135">Ошибки, возникающие при попытке принятия приглашения на собрание, который не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="49c64-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="49c64-136">Программа</span><span class="sxs-lookup"><span data-stu-id="49c64-136">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="49c64-137">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="49c64-137">Error response elements</span></span>

<span data-ttu-id="49c64-138">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="49c64-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="49c64-139">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="49c64-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="49c64-140">CreateItemResponse</span><span class="sxs-lookup"><span data-stu-id="49c64-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="49c64-141">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="49c64-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="49c64-142">CreateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="49c64-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="49c64-143">MessageText</span><span class="sxs-lookup"><span data-stu-id="49c64-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="49c64-144">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="49c64-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="49c64-145">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="49c64-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="49c64-146">Элементы</span><span class="sxs-lookup"><span data-stu-id="49c64-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="49c64-147">См. также</span><span class="sxs-lookup"><span data-stu-id="49c64-147">See also</span></span>



[<span data-ttu-id="49c64-148">CreateItem Operation</span><span class="sxs-lookup"><span data-stu-id="49c64-148">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="49c64-149">Операции CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="49c64-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

