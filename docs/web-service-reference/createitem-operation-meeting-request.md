---
title: Операция CreateItem (приглашение на собрание)
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
description: Операция CreateItem используется для ответа на приглашения на собрания.
ms.openlocfilehash: f9e6bd1742e6a30d08736ea67c0ff80b7a18e88a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457111"
---
# <a name="createitem-operation-meeting-request"></a><span data-ttu-id="6e0b6-103">Операция CreateItem (приглашение на собрание)</span><span class="sxs-lookup"><span data-stu-id="6e0b6-103">CreateItem operation (meeting request)</span></span>

<span data-ttu-id="6e0b6-104">Операция CreateItem используется для ответа на приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-104">The CreateItem operation is used to respond to meeting requests.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6e0b6-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="6e0b6-105">Remarks</span></span>

<span data-ttu-id="6e0b6-106">Операция CreateItem предоставляет три варианта ответа на приглашение на собрание: принять, под вопросом или отклонить.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-106">The CreateItem operation provides three options for responding to a meeting request: accept, tentatively accept, or decline.</span></span> 
  
## <a name="accept-meeting-request-example"></a><span data-ttu-id="6e0b6-107">Пример принятия приглашения на собрание</span><span class="sxs-lookup"><span data-stu-id="6e0b6-107">Accept Meeting request example</span></span>

### <a name="description"></a><span data-ttu-id="6e0b6-108">Description</span><span class="sxs-lookup"><span data-stu-id="6e0b6-108">Description</span></span>

<span data-ttu-id="6e0b6-109">В приведенном ниже примере показано, как принять приглашение на собрание.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-109">The following example shows how to accept a meeting request invitation.</span></span>
  
### <a name="code"></a><span data-ttu-id="6e0b6-110">Код</span><span class="sxs-lookup"><span data-stu-id="6e0b6-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="6e0b6-111">Комментарии</span><span class="sxs-lookup"><span data-stu-id="6e0b6-111">Comments</span></span>

<span data-ttu-id="6e0b6-112">Чтобы принять или отклонить приглашение на собрание, используйте элементы [тентативелякцептитем](tentativelyacceptitem.md) или [Деклинеитем](declineitem.md) вместо элемента [акцептитем](acceptitem.md) .</span><span class="sxs-lookup"><span data-stu-id="6e0b6-112">To tentatively accept or to decline the meeting request, use the [TentativelyAcceptItem](tentativelyacceptitem.md) or [DeclineItem](declineitem.md) elements in place of the [AcceptItem](acceptitem.md) element.</span></span> 
  
<span data-ttu-id="6e0b6-113">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-113">The item identifier and change key have been shortened to preserve readability.</span></span>
  
### <a name="accepting-meeting-request-elements"></a><span data-ttu-id="6e0b6-114">Принятие элементов приглашения на собрание</span><span class="sxs-lookup"><span data-stu-id="6e0b6-114">Accepting Meeting Request Elements</span></span>

<span data-ttu-id="6e0b6-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6e0b6-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="6e0b6-116">CreateItem</span><span class="sxs-lookup"><span data-stu-id="6e0b6-116">CreateItem</span></span>](createitem.md)
    
- [<span data-ttu-id="6e0b6-117">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="6e0b6-117">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="6e0b6-118">акцептитем</span><span class="sxs-lookup"><span data-stu-id="6e0b6-118">AcceptItem</span></span>](acceptitem.md)
    
- [<span data-ttu-id="6e0b6-119">референцеитемид</span><span class="sxs-lookup"><span data-stu-id="6e0b6-119">ReferenceItemId</span></span>](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a><span data-ttu-id="6e0b6-120">Пример успешного принятия ответа на приглашение на собрание</span><span class="sxs-lookup"><span data-stu-id="6e0b6-120">Successful Accept Meeting response example</span></span>

### <a name="description"></a><span data-ttu-id="6e0b6-121">Description</span><span class="sxs-lookup"><span data-stu-id="6e0b6-121">Description</span></span>

<span data-ttu-id="6e0b6-122">В следующем примере показан успешный ответ на запрос CreateItem.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-122">The following example shows a successful response to the CreateItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="6e0b6-123">Код</span><span class="sxs-lookup"><span data-stu-id="6e0b6-123">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="successful-response-elements"></a><span data-ttu-id="6e0b6-124">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="6e0b6-124">Successful response elements</span></span>

<span data-ttu-id="6e0b6-125">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6e0b6-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="6e0b6-126">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6e0b6-126">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6e0b6-127">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="6e0b6-127">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="6e0b6-128">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6e0b6-128">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6e0b6-129">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6e0b6-129">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="6e0b6-130">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6e0b6-130">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6e0b6-131">Items</span><span class="sxs-lookup"><span data-stu-id="6e0b6-131">Items</span></span>](items.md)
    
## <a name="accept-meeting-error-response-example"></a><span data-ttu-id="6e0b6-132">Пример принятия ответа на сообщение об ошибке собрания</span><span class="sxs-lookup"><span data-stu-id="6e0b6-132">Accept Meeting Error response example</span></span>

### <a name="description"></a><span data-ttu-id="6e0b6-133">Description</span><span class="sxs-lookup"><span data-stu-id="6e0b6-133">Description</span></span>

<span data-ttu-id="6e0b6-134">В следующем примере показан ответ об ошибке для запроса CreateItem.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-134">The following example shows an error response to CreateItem request.</span></span> <span data-ttu-id="6e0b6-135">Ошибка вызвана попыткой принять приглашение на собрание, которое не удается найти в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="6e0b6-135">The error is caused by an attempt to accept a meeting request that cannot be found in the Exchange store.</span></span>
  
### <a name="code"></a><span data-ttu-id="6e0b6-136">Код</span><span class="sxs-lookup"><span data-stu-id="6e0b6-136">Code</span></span>

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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="6e0b6-137">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="6e0b6-137">Error response elements</span></span>

<span data-ttu-id="6e0b6-138">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6e0b6-138">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="6e0b6-139">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6e0b6-139">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6e0b6-140">креатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="6e0b6-140">CreateItemResponse</span></span>](createitemresponse.md)
    
- [<span data-ttu-id="6e0b6-141">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="6e0b6-141">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="6e0b6-142">креатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6e0b6-142">CreateItemResponseMessage</span></span>](createitemresponsemessage.md)
    
- [<span data-ttu-id="6e0b6-143">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="6e0b6-143">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="6e0b6-144">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6e0b6-144">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6e0b6-145">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="6e0b6-145">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="6e0b6-146">Items</span><span class="sxs-lookup"><span data-stu-id="6e0b6-146">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="6e0b6-147">См. также</span><span class="sxs-lookup"><span data-stu-id="6e0b6-147">See also</span></span>



[<span data-ttu-id="6e0b6-148">Операция CreateItem</span><span class="sxs-lookup"><span data-stu-id="6e0b6-148">CreateItem operation</span></span>](createitem-operation.md)
  
[<span data-ttu-id="6e0b6-149">Операция CreateItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="6e0b6-149">CreateItem operation (calendar item)</span></span>](createitem-operation-calendar-item.md)

