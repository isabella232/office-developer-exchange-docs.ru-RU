---
title: Операция CopyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItem
api_type:
- schema
ms.assetid: bcc68f9e-d511-4c29-bba6-ed535524624a
description: Операция CopyItem копирует элементы и размещает их в другой папке.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761841"
---
# <a name="copyitem-operation"></a><span data-ttu-id="ca763-103">Операция CopyItem</span><span class="sxs-lookup"><span data-stu-id="ca763-103">CopyItem operation</span></span>

<span data-ttu-id="ca763-104">Операция **CopyItem** копирует элементы и размещает их в другой папке.</span><span class="sxs-lookup"><span data-stu-id="ca763-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="ca763-105">Пример запроса CopyItem</span><span class="sxs-lookup"><span data-stu-id="ca763-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="ca763-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ca763-106">Description</span></span>

<span data-ttu-id="ca763-107">В приведенном ниже примере запроса **CopyItem** показано, как сформировать запрос на копирование элемента в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="ca763-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ca763-108">Код</span><span class="sxs-lookup"><span data-stu-id="ca763-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CopyItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ToFolderId>
        <t:DistinguishedFolderId Id="inbox"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AS4AUnV="/>
      </ItemIds>
    </CopyItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="ca763-109">Comments</span><span class="sxs-lookup"><span data-stu-id="ca763-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="ca763-110">Идентификатор папки и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ca763-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ca763-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="ca763-111">Request elements</span></span>

<span data-ttu-id="ca763-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ca763-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ca763-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="ca763-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="ca763-114">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="ca763-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="ca763-115">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="ca763-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="ca763-116">итемидс</span><span class="sxs-lookup"><span data-stu-id="ca763-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="ca763-117">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ca763-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="ca763-118">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ca763-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="ca763-119">Чтобы найти другие параметры сообщения Request операции **CopyItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="ca763-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ca763-120">Начните с элемента [CopyItem](copyitem.md) .</span><span class="sxs-lookup"><span data-stu-id="ca763-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="ca763-121">Успешный ответ CopyItem</span><span class="sxs-lookup"><span data-stu-id="ca763-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="ca763-122">Описание</span><span class="sxs-lookup"><span data-stu-id="ca763-122">Description</span></span>

<span data-ttu-id="ca763-123">В следующем примере показан успешный ответ на запрос **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="ca763-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="ca763-124">В ответном сообщении возвращается идентификатор элемента нового элемента.</span><span class="sxs-lookup"><span data-stu-id="ca763-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="ca763-125">Идентификаторы элементов не возвращаются в ответах на операции **CopyItem** для нескольких почтовых ящиков или почтовых ящиков в общедоступных папках.</span><span class="sxs-lookup"><span data-stu-id="ca763-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ca763-126">Код</span><span class="sxs-lookup"><span data-stu-id="ca763-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="ca763-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ca763-127">Successful response elements</span></span>

<span data-ttu-id="ca763-128">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ca763-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ca763-129">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ca763-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ca763-130">копитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="ca763-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="ca763-131">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ca763-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ca763-132">копитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ca763-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="ca763-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ca763-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ca763-134">Items</span><span class="sxs-lookup"><span data-stu-id="ca763-134">Items</span></span>](items.md)
    
<span data-ttu-id="ca763-135">Чтобы найти другие параметры для ответного сообщения операции **CopyItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="ca763-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ca763-136">Начните с элемента [копитемреспонсе](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="ca763-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="ca763-137">Ответ об ошибке CopyItem</span><span class="sxs-lookup"><span data-stu-id="ca763-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="ca763-138">Описание</span><span class="sxs-lookup"><span data-stu-id="ca763-138">Description</span></span>

<span data-ttu-id="ca763-139">В следующем примере показан ответ об ошибке для запроса **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="ca763-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ca763-140">Код</span><span class="sxs-lookup"><span data-stu-id="ca763-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="595" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <CopyItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CopyItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CopyItemResponseMessage>
      </m:ResponseMessages>
    </CopyItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="ca763-141">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="ca763-141">Error response elements</span></span>

<span data-ttu-id="ca763-142">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ca763-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ca763-143">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ca763-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ca763-144">копитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="ca763-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="ca763-145">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ca763-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ca763-146">копитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ca763-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="ca763-147">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ca763-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ca763-148">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ca763-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ca763-149">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ca763-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ca763-150">Items</span><span class="sxs-lookup"><span data-stu-id="ca763-150">Items</span></span>](items.md)
    
<span data-ttu-id="ca763-151">Чтобы найти другие параметры сообщения об ошибке при выполнении операции **CopyItem** , изучите иерархию схемы.</span><span class="sxs-lookup"><span data-stu-id="ca763-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="ca763-152">Начните с элемента [копитемреспонсе](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="ca763-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ca763-153">См. также</span><span class="sxs-lookup"><span data-stu-id="ca763-153">See also</span></span>



- [<span data-ttu-id="ca763-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ca763-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

