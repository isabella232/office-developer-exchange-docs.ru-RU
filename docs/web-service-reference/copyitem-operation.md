---
title: CopyItem Operation
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
description: Операция CopyItem копирует элементы и размещает элементы в другую папку.
ms.openlocfilehash: 95d2371e9185aa25f40eaec37dda54276a54d321
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761841"
---
# <a name="copyitem-operation"></a><span data-ttu-id="a2675-103">CopyItem Operation</span><span class="sxs-lookup"><span data-stu-id="a2675-103">CopyItem operation</span></span>

<span data-ttu-id="a2675-104">Операция **CopyItem** копирует элементы и размещает элементы в другую папку.</span><span class="sxs-lookup"><span data-stu-id="a2675-104">The **CopyItem** operation copies items and puts the items in a different folder.</span></span> 
  
## <a name="copyitem-request-example"></a><span data-ttu-id="a2675-105">Пример запроса CopyItem</span><span class="sxs-lookup"><span data-stu-id="a2675-105">CopyItem request example</span></span>

### <a name="description"></a><span data-ttu-id="a2675-106">Описание</span><span class="sxs-lookup"><span data-stu-id="a2675-106">Description</span></span>

<span data-ttu-id="a2675-107">В следующем примере запрос **CopyItem** показано, как для формирования запроса скопировать элемент в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="a2675-107">The following example of a **CopyItem** request shows how to form a request to copy an item to the Inbox.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a2675-108">Программа</span><span class="sxs-lookup"><span data-stu-id="a2675-108">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="a2675-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="a2675-109">Comments</span></span>

> [!NOTE]
> <span data-ttu-id="a2675-110">Идентификатор папки и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="a2675-110">The folder ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="a2675-111">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="a2675-111">Request elements</span></span>

<span data-ttu-id="a2675-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a2675-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a2675-113">CopyItem</span><span class="sxs-lookup"><span data-stu-id="a2675-113">CopyItem</span></span>](copyitem.md)
    
- [<span data-ttu-id="a2675-114">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="a2675-114">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="a2675-115">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="a2675-115">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="a2675-116">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="a2675-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="a2675-117">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="a2675-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="a2675-118">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a2675-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="a2675-119">Чтобы найти другие параметры для запроса операции **CopyItem** , изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="a2675-119">To find other options for the request message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a2675-120">Начать с [CopyItem](copyitem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="a2675-120">Start at the [CopyItem](copyitem.md) element.</span></span> 
  
## <a name="successful-copyitem-response"></a><span data-ttu-id="a2675-121">Успешного ответа CopyItem</span><span class="sxs-lookup"><span data-stu-id="a2675-121">Successful CopyItem Response</span></span>

### <a name="description"></a><span data-ttu-id="a2675-122">Описание</span><span class="sxs-lookup"><span data-stu-id="a2675-122">Description</span></span>

<span data-ttu-id="a2675-123">В следующем примере показано успешного ответа на запрос **CopyItem** .</span><span class="sxs-lookup"><span data-stu-id="a2675-123">The following example shows a successful response to the **CopyItem** request.</span></span> 
  
<span data-ttu-id="a2675-124">Идентификатор нового элемента, возвращается в сообщении ответа.</span><span class="sxs-lookup"><span data-stu-id="a2675-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="a2675-125">Идентификаторы элементов не возвращаются в ответ для нескольких почтовых или почтовых ящиков операциям **CopyItem** общей папки.</span><span class="sxs-lookup"><span data-stu-id="a2675-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **CopyItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a2675-126">Программа</span><span class="sxs-lookup"><span data-stu-id="a2675-126">Code</span></span>

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

### <a name="successful-response-elements"></a><span data-ttu-id="a2675-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a2675-127">Successful response elements</span></span>

<span data-ttu-id="a2675-128">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a2675-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a2675-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a2675-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a2675-130">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="a2675-130">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="a2675-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2675-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a2675-132">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2675-132">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="a2675-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a2675-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a2675-134">Элементы</span><span class="sxs-lookup"><span data-stu-id="a2675-134">Items</span></span>](items.md)
    
<span data-ttu-id="a2675-135">Чтобы найти другие параметры в сообщении ответа операции **CopyItem** , изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="a2675-135">To find other options for the response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a2675-136">Запустите в элементе [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a2675-136">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="copyitem-error-response"></a><span data-ttu-id="a2675-137">Отклик CopyItem</span><span class="sxs-lookup"><span data-stu-id="a2675-137">CopyItem error response</span></span>

### <a name="description"></a><span data-ttu-id="a2675-138">Описание</span><span class="sxs-lookup"><span data-stu-id="a2675-138">Description</span></span>

<span data-ttu-id="a2675-139">В следующем примере показано возврату ошибки **CopyItem** запрос.</span><span class="sxs-lookup"><span data-stu-id="a2675-139">The following example shows an error response to a **CopyItem** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a2675-140">Программа</span><span class="sxs-lookup"><span data-stu-id="a2675-140">Code</span></span>

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

### <a name="error-response-elements"></a><span data-ttu-id="a2675-141">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="a2675-141">Error response elements</span></span>

<span data-ttu-id="a2675-142">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a2675-142">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="a2675-143">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a2675-143">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a2675-144">CopyItemResponse</span><span class="sxs-lookup"><span data-stu-id="a2675-144">CopyItemResponse</span></span>](copyitemresponse.md)
    
- [<span data-ttu-id="a2675-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a2675-145">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="a2675-146">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a2675-146">CopyItemResponseMessage</span></span>](copyitemresponsemessage.md)
    
- [<span data-ttu-id="a2675-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="a2675-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a2675-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a2675-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a2675-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a2675-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="a2675-150">Элементы</span><span class="sxs-lookup"><span data-stu-id="a2675-150">Items</span></span>](items.md)
    
<span data-ttu-id="a2675-151">Чтобы найти другие параметры в сообщении об ошибке ответа операции **CopyItem** , изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="a2675-151">To find other options for the error response message of the **CopyItem** operation, explore the schema hierarchy.</span></span> <span data-ttu-id="a2675-152">Запустите в элементе [CopyItemResponse](copyitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="a2675-152">Start at the [CopyItemResponse](copyitemresponse.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a2675-153">См. также</span><span class="sxs-lookup"><span data-stu-id="a2675-153">See also</span></span>



- [<span data-ttu-id="a2675-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a2675-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

