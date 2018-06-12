---
title: Операция DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в хранилище Exchange.
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762022"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="33b74-103">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-103">DeleteAttachment operation</span></span>

<span data-ttu-id="33b74-104">Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="33b74-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33b74-105">Замечания</span><span class="sxs-lookup"><span data-stu-id="33b74-105">Remarks</span></span>

<span data-ttu-id="33b74-106">Эта операция позволяет удалить один или несколько вложений по идентификатору.</span><span class="sxs-lookup"><span data-stu-id="33b74-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="33b74-107">Пример запроса DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="33b74-108">Описание</span><span class="sxs-lookup"><span data-stu-id="33b74-108">Description</span></span>

<span data-ttu-id="33b74-109">В следующем примере запрос DeleteAttachment показано, как удалить вложение элемента.</span><span class="sxs-lookup"><span data-stu-id="33b74-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="33b74-110">Программа</span><span class="sxs-lookup"><span data-stu-id="33b74-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="33b74-111">Комментарии</span><span class="sxs-lookup"><span data-stu-id="33b74-111">Comments</span></span>

<span data-ttu-id="33b74-112">Идентификатор вложения был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="33b74-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="33b74-113">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="33b74-113">Request elements</span></span>

<span data-ttu-id="33b74-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="33b74-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="33b74-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="33b74-116">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="33b74-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="33b74-117">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="33b74-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="33b74-118">Пример ответа DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="33b74-119">Описание</span><span class="sxs-lookup"><span data-stu-id="33b74-119">Description</span></span>

<span data-ttu-id="33b74-120">В следующем примере показано успешного ответа на запрос DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="33b74-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="33b74-121">Программа</span><span class="sxs-lookup"><span data-stu-id="33b74-121">Code</span></span>

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
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="33b74-122">Комментарии</span><span class="sxs-lookup"><span data-stu-id="33b74-122">Comments</span></span>

<span data-ttu-id="33b74-123">Операция CreateAttachment возвращает элемент AttachmentIdType типа, который включает в себя **RootItemId** и **RootItemChangeKey**.</span><span class="sxs-lookup"><span data-stu-id="33b74-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="33b74-124">Эти атрибуты не допускаются для идентификаторов в запросе DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="33b74-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="33b74-125">DeleteAttachment использует элементы типа RequestAttachmentIdType, которая не включает следующие атрибуты.</span><span class="sxs-lookup"><span data-stu-id="33b74-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="33b74-126">Ответ DeleteAttachment включает в себя идентификатор родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="33b74-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="33b74-127">После удаления вложения из элемента изменяется ключ изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="33b74-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="33b74-128">Новый ключ изменения элемента можно получить из ответа DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="33b74-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="33b74-129">Идентификатор [RootItemId](rootitemid.md) и ChangeKey URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="33b74-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="33b74-130">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="33b74-130">Successful response elements</span></span>

<span data-ttu-id="33b74-131">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="33b74-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="33b74-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="33b74-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="33b74-133">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="33b74-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="33b74-134">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="33b74-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="33b74-135">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="33b74-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="33b74-136">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="33b74-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="33b74-137">RootItemId</span><span class="sxs-lookup"><span data-stu-id="33b74-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="33b74-138">См. также</span><span class="sxs-lookup"><span data-stu-id="33b74-138">See also</span></span>

- [<span data-ttu-id="33b74-139">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="33b74-140">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="33b74-140">GetAttachment operation</span></span>](getattachment-operation.md)

