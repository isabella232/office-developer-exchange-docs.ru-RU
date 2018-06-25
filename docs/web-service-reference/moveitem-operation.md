---
title: MoveItem Operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItem
api_type:
- schema
ms.assetid: dcf40fa7-7796-4a5c-bf5b-7a509a18d208
description: Операция MoveItem используется для перемещения одного или нескольких элементов в одну целевую папку.
ms.openlocfilehash: c5619befb02ec20ef0911992484dcc00cc2c5e92
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834492"
---
# <a name="moveitem-operation"></a><span data-ttu-id="21a3b-103">MoveItem Operation</span><span class="sxs-lookup"><span data-stu-id="21a3b-103">MoveItem operation</span></span>

<span data-ttu-id="21a3b-104">Операция **MoveItem** используется для перемещения одного или нескольких элементов в одну целевую папку.</span><span class="sxs-lookup"><span data-stu-id="21a3b-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="21a3b-105">Пример запроса MoveItem</span><span class="sxs-lookup"><span data-stu-id="21a3b-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="21a3b-106">Описание</span><span class="sxs-lookup"><span data-stu-id="21a3b-106">Description</span></span>

<span data-ttu-id="21a3b-107">Приведенный ниже запрос **MoveItem** показано перемещение элемента в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="21a3b-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="21a3b-108">Программа</span><span class="sxs-lookup"><span data-stu-id="21a3b-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <MoveItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ToFolderId>
        <t:DistinguishedFolderId Id="drafts"/>
      </ToFolderId>
      <ItemIds>
        <t:ItemId Id="AAAtAEF/swbAAA=" ChangeKey="EwAAABYA/s4b"/>
      </ItemIds>
    </MoveItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="21a3b-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="21a3b-109">Comments</span></span>

<span data-ttu-id="21a3b-110">Элемент [ToFolderId](tofolderid.md) указывает папку, в который перемещается элементы.</span><span class="sxs-lookup"><span data-stu-id="21a3b-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="21a3b-111">Обратите внимание на то, что все элементы, перечисленные в коллекции [что ItemID](itemids.md) окажутся в папке назначения.</span><span class="sxs-lookup"><span data-stu-id="21a3b-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="21a3b-112">Необходимо включить для отдельных вызовов **MoveItem** размещение элементов в разных конечные папки.</span><span class="sxs-lookup"><span data-stu-id="21a3b-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="21a3b-113">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="21a3b-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="21a3b-114">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="21a3b-114">Request elements</span></span>

<span data-ttu-id="21a3b-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="21a3b-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="21a3b-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="21a3b-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="21a3b-117">ToFolderId</span><span class="sxs-lookup"><span data-stu-id="21a3b-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="21a3b-118">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="21a3b-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="21a3b-119">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="21a3b-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="21a3b-120">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="21a3b-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="21a3b-121">Пример ответа MoveItem</span><span class="sxs-lookup"><span data-stu-id="21a3b-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="21a3b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="21a3b-122">Description</span></span>

<span data-ttu-id="21a3b-123">В следующем примере показано успешного ответа на запрос **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="21a3b-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="21a3b-124">Идентификатор нового элемента, возвращается в сообщении ответа.</span><span class="sxs-lookup"><span data-stu-id="21a3b-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="21a3b-125">Идентификаторы элементов не возвращаются в ответ для нескольких почтовых или почтовых ящиков операциям **MoveItem** общей папки.</span><span class="sxs-lookup"><span data-stu-id="21a3b-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="21a3b-126">Программа</span><span class="sxs-lookup"><span data-stu-id="21a3b-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <MoveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:MoveItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemID Id="AAMkAd" ChangeKey="FwAAABY" />
            </t:Message>
          </m:Items>
        </m:MoveItemResponseMessage>
      </m:ResponseMessages>
    </MoveItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="21a3b-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="21a3b-127">Comments</span></span>

<span data-ttu-id="21a3b-128">Операция **MoveItem** содержатся сведения о успешное перемещение выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="21a3b-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="21a3b-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="21a3b-129">Successful response elements</span></span>

<span data-ttu-id="21a3b-130">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="21a3b-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="21a3b-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="21a3b-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="21a3b-132">MoveItemResponse</span><span class="sxs-lookup"><span data-stu-id="21a3b-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="21a3b-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21a3b-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="21a3b-134">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21a3b-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="21a3b-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21a3b-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="21a3b-136">Элементы</span><span class="sxs-lookup"><span data-stu-id="21a3b-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="21a3b-137">См. также</span><span class="sxs-lookup"><span data-stu-id="21a3b-137">See also</span></span>



- [<span data-ttu-id="21a3b-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="21a3b-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

