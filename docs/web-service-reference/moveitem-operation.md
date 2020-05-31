---
title: Операция MoveItem
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
# <a name="moveitem-operation"></a><span data-ttu-id="94233-103">Операция MoveItem</span><span class="sxs-lookup"><span data-stu-id="94233-103">MoveItem operation</span></span>

<span data-ttu-id="94233-104">Операция **MoveItem** используется для перемещения одного или нескольких элементов в одну целевую папку.</span><span class="sxs-lookup"><span data-stu-id="94233-104">The **MoveItem** operation is used to move one or more items to a single destination folder.</span></span> 
  
## <a name="moveitem-request-example"></a><span data-ttu-id="94233-105">Пример запроса MoveItem</span><span class="sxs-lookup"><span data-stu-id="94233-105">MoveItem request example</span></span>

### <a name="description"></a><span data-ttu-id="94233-106">Описание</span><span class="sxs-lookup"><span data-stu-id="94233-106">Description</span></span>

<span data-ttu-id="94233-107">В приведенном ниже примере запроса **MoveItem** показано, как переместить элемент в папку "Черновики".</span><span class="sxs-lookup"><span data-stu-id="94233-107">The following example of a **MoveItem** request shows how to move an item to the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="94233-108">Код</span><span class="sxs-lookup"><span data-stu-id="94233-108">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="94233-109">Comments</span><span class="sxs-lookup"><span data-stu-id="94233-109">Comments</span></span>

<span data-ttu-id="94233-110">Элемент [тофолдерид](tofolderid.md) указывает папку, в которую будут перемещены элементы.</span><span class="sxs-lookup"><span data-stu-id="94233-110">The [ToFolderId](tofolderid.md) element specifies the folder to which the items will be moved.</span></span> <span data-ttu-id="94233-111">Обратите внимание, что все элементы, перечисленные в коллекции [итемидс](itemids.md) , будут находиться в конечной папке.</span><span class="sxs-lookup"><span data-stu-id="94233-111">Note that all items listed in the [ItemIds](itemids.md) collection will end up in the destination folder.</span></span> <span data-ttu-id="94233-112">Для размещения элементов в разных папках назначения необходимо выполнить отдельные вызовы **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="94233-112">You must make separate **MoveItem** calls to place items in different destination folders.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="94233-113">Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="94233-113">The item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="94233-114">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="94233-114">Request elements</span></span>

<span data-ttu-id="94233-115">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="94233-115">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="94233-116">MoveItem</span><span class="sxs-lookup"><span data-stu-id="94233-116">MoveItem</span></span>](moveitem.md)
    
- [<span data-ttu-id="94233-117">тофолдерид</span><span class="sxs-lookup"><span data-stu-id="94233-117">ToFolderId</span></span>](tofolderid.md)
    
- [<span data-ttu-id="94233-118">дистингуишедфолдерид</span><span class="sxs-lookup"><span data-stu-id="94233-118">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="94233-119">итемидс</span><span class="sxs-lookup"><span data-stu-id="94233-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="94233-120">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="94233-120">ItemId</span></span>](itemid.md)
    
## <a name="moveitem-response-example"></a><span data-ttu-id="94233-121">Пример отклика MoveItem</span><span class="sxs-lookup"><span data-stu-id="94233-121">MoveItem response example</span></span>

### <a name="description"></a><span data-ttu-id="94233-122">Описание</span><span class="sxs-lookup"><span data-stu-id="94233-122">Description</span></span>

<span data-ttu-id="94233-123">В следующем примере показан успешный ответ на запрос **MoveItem** .</span><span class="sxs-lookup"><span data-stu-id="94233-123">The following example shows a successful response to a **MoveItem** request.</span></span> 
  
<span data-ttu-id="94233-124">В ответном сообщении возвращается идентификатор элемента нового элемента.</span><span class="sxs-lookup"><span data-stu-id="94233-124">The item identifier of the new item is returned in the response message.</span></span> <span data-ttu-id="94233-125">Идентификаторы элементов не возвращаются в ответах на операции **MoveItem** для нескольких почтовых ящиков или почтовых ящиков в общедоступных папках.</span><span class="sxs-lookup"><span data-stu-id="94233-125">Item identifiers are not returned in responses for cross-mailbox or mailbox to public folder **MoveItem** operations.</span></span> 
  
### <a name="code"></a><span data-ttu-id="94233-126">Код</span><span class="sxs-lookup"><span data-stu-id="94233-126">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="94233-127">Comments</span><span class="sxs-lookup"><span data-stu-id="94233-127">Comments</span></span>

<span data-ttu-id="94233-128">Если перемещение прошло успешно, операция **MoveItem** будет указывать на успешное выполнение.</span><span class="sxs-lookup"><span data-stu-id="94233-128">The **MoveItem** operation will indicate success if the move was successful.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="94233-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="94233-129">Successful response elements</span></span>

<span data-ttu-id="94233-130">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="94233-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="94233-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="94233-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="94233-132">мовеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="94233-132">MoveItemResponse</span></span>](moveitemresponse.md)
    
- [<span data-ttu-id="94233-133">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="94233-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="94233-134">мовеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="94233-134">MoveItemResponseMessage</span></span>](moveitemresponsemessage.md)
    
- [<span data-ttu-id="94233-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="94233-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="94233-136">Items</span><span class="sxs-lookup"><span data-stu-id="94233-136">Items</span></span>](items.md)
    
## <a name="see-also"></a><span data-ttu-id="94233-137">См. также</span><span class="sxs-lookup"><span data-stu-id="94233-137">See also</span></span>



- [<span data-ttu-id="94233-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="94233-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

