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
description: Операция DeleteAttachment используется для удаления вложенных файлов и вложений элементов из существующего элемента в хранилище Exchange.
ms.openlocfilehash: 1d34ce4c5ba1d955989a35dafb8ab3c5d229d505
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457335"
---
# <a name="deleteattachment-operation"></a><span data-ttu-id="fa26d-103">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-103">DeleteAttachment operation</span></span>

<span data-ttu-id="fa26d-104">Операция DeleteAttachment используется для удаления вложенных файлов и вложений элементов из существующего элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fa26d-104">The DeleteAttachment operation is used to delete file and item attachments from an existing item in the Exchange store.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa26d-105">Примечания</span><span class="sxs-lookup"><span data-stu-id="fa26d-105">Remarks</span></span>

<span data-ttu-id="fa26d-106">Эта операция позволяет удалить одно или несколько вложений по ИДЕНТИФИКАТОРу.</span><span class="sxs-lookup"><span data-stu-id="fa26d-106">This operation allows you to delete one or more attachments by ID.</span></span>
  
## <a name="deleteattachment-request-example"></a><span data-ttu-id="fa26d-107">Пример запроса DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-107">DeleteAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="fa26d-108">Описание</span><span class="sxs-lookup"><span data-stu-id="fa26d-108">Description</span></span>

<span data-ttu-id="fa26d-109">В приведенном ниже примере запроса DeleteAttachment показано, как удалить вложение элемента.</span><span class="sxs-lookup"><span data-stu-id="fa26d-109">The following example of a DeleteAttachment request shows how to delete an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="fa26d-110">Код</span><span class="sxs-lookup"><span data-stu-id="fa26d-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="fa26d-111">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fa26d-111">Comments</span></span>

<span data-ttu-id="fa26d-112">Идентификатор вложения был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="fa26d-112">The attachment identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="fa26d-113">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="fa26d-113">Request elements</span></span>

<span data-ttu-id="fa26d-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fa26d-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="fa26d-115">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-115">DeleteAttachment</span></span>](deleteattachment.md)
    
- [<span data-ttu-id="fa26d-116">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="fa26d-116">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="fa26d-117">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="fa26d-117">AttachmentId</span></span>](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a><span data-ttu-id="fa26d-118">Пример отклика DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-118">DeleteAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="fa26d-119">Описание</span><span class="sxs-lookup"><span data-stu-id="fa26d-119">Description</span></span>

<span data-ttu-id="fa26d-120">В следующем примере показан успешный ответ на запрос DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="fa26d-120">The following example shows a successful response to a DeleteAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fa26d-121">Код</span><span class="sxs-lookup"><span data-stu-id="fa26d-121">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="fa26d-122">Комментарии</span><span class="sxs-lookup"><span data-stu-id="fa26d-122">Comments</span></span>

<span data-ttu-id="fa26d-123">Операция CreateAttachment Возвращает элемент типа Аттачментидтипе, включающий в себя **рутитемид** и **рутитемчанжекэй**.</span><span class="sxs-lookup"><span data-stu-id="fa26d-123">The CreateAttachment operation returns an element of AttachmentIdType type that includes a **RootItemId** and **RootItemChangeKey**.</span></span> <span data-ttu-id="fa26d-124">Эти атрибуты не разрешены для идентификаторов в запросе DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="fa26d-124">These attributes are not permitted for identifiers within a DeleteAttachment request.</span></span> <span data-ttu-id="fa26d-125">DeleteAttachment использует элементы типа Рекуестаттачментидтипе, которые не включают эти атрибуты.</span><span class="sxs-lookup"><span data-stu-id="fa26d-125">DeleteAttachment uses elements of type RequestAttachmentIdType, which does not include these attributes.</span></span>
  
<span data-ttu-id="fa26d-126">Ответ DeleteAttachment включает идентификатор родительского элемента.</span><span class="sxs-lookup"><span data-stu-id="fa26d-126">The DeleteAttachment response includes the ID of the parent item.</span></span> <span data-ttu-id="fa26d-127">При удалении вложений из элемента изменяется ключ изменения элемента.</span><span class="sxs-lookup"><span data-stu-id="fa26d-127">When attachments are removed from an item, the item's change key is modified.</span></span> <span data-ttu-id="fa26d-128">Новый ключ изменения элемента можно получить из отклика DeleteAttachment.</span><span class="sxs-lookup"><span data-stu-id="fa26d-128">The new item change key can be obtained from the DeleteAttachment response.</span></span>
  
> [!NOTE]
> <span data-ttu-id="fa26d-129">Идентификатор [рутитемид](rootitemid.md) и чанжекэй были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="fa26d-129">The [RootItemId](rootitemid.md) identifier and ChangeKey have been shortened to preserve readability.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="fa26d-130">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="fa26d-130">Successful response elements</span></span>

<span data-ttu-id="fa26d-131">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="fa26d-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="fa26d-132">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="fa26d-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="fa26d-133">делетеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="fa26d-133">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)
    
- [<span data-ttu-id="fa26d-134">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="fa26d-134">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="fa26d-135">делетеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="fa26d-135">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
    
- [<span data-ttu-id="fa26d-136">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="fa26d-136">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="fa26d-137">рутитемид</span><span class="sxs-lookup"><span data-stu-id="fa26d-137">RootItemId</span></span>](rootitemid.md)
    
## <a name="see-also"></a><span data-ttu-id="fa26d-138">См. также</span><span class="sxs-lookup"><span data-stu-id="fa26d-138">See also</span></span>

- [<span data-ttu-id="fa26d-139">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-139">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="fa26d-140">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="fa26d-140">GetAttachment operation</span></span>](getattachment-operation.md)

