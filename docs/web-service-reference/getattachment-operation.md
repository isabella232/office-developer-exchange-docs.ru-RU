---
title: Операция GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: Операция GetAttachment используется для извлечения существующие вложения для элементов в хранилище Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762701"
---
# <a name="getattachment-operation"></a><span data-ttu-id="cc44f-103">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-103">GetAttachment operation</span></span>

<span data-ttu-id="cc44f-104">Операция GetAttachment используется для извлечения существующие вложения для элементов в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="cc44f-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="cc44f-105">Пример запроса GetAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="cc44f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="cc44f-106">Description</span></span>

<span data-ttu-id="cc44f-107">В следующем примере запрос на GetAttachment показано, как для получения вложения.</span><span class="sxs-lookup"><span data-stu-id="cc44f-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="cc44f-108">Программа</span><span class="sxs-lookup"><span data-stu-id="cc44f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="cc44f-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="cc44f-109">Comments</span></span>

<span data-ttu-id="cc44f-110">Элемент [AttachmentShape](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="cc44f-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="cc44f-111">Пустой элемент [AttachmentShape](attachmentshape.md) является допустимым и будут отображаться вложения без содержимого MIME для вложений элемента с типом body текст и без любые дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="cc44f-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="cc44f-112">Коллекция [AttachmentIds](attachmentids.md) позволяет указать один или несколько идентификаторов вложений для возврата.</span><span class="sxs-lookup"><span data-stu-id="cc44f-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="cc44f-113">Обратите внимание, что это RequestAttachmentIdType, поэтому любые AttachmentIds, полученные из **CreateAttachment** должно иметь атрибуты **RootItemId** и **RootItemChangeKey** удалены перед передачей их в **GetAttachment**типа.</span><span class="sxs-lookup"><span data-stu-id="cc44f-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="cc44f-114">Идентификатор вложения и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="cc44f-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="cc44f-115">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="cc44f-115">Request elements</span></span>

<span data-ttu-id="cc44f-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cc44f-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="cc44f-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="cc44f-118">AttachmentShape</span><span class="sxs-lookup"><span data-stu-id="cc44f-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="cc44f-119">AttachmentIds</span><span class="sxs-lookup"><span data-stu-id="cc44f-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="cc44f-120">Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="cc44f-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="cc44f-121">Пример ответа GetAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="cc44f-122">Описание</span><span class="sxs-lookup"><span data-stu-id="cc44f-122">Description</span></span>

<span data-ttu-id="cc44f-123">В следующем примере показано успешного ответа на запрос GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="cc44f-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="cc44f-124">В этом примере возвращается вложенный файл.</span><span class="sxs-lookup"><span data-stu-id="cc44f-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="cc44f-125">Программа</span><span class="sxs-lookup"><span data-stu-id="cc44f-125">Code</span></span>

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
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="cc44f-126">Комментарии</span><span class="sxs-lookup"><span data-stu-id="cc44f-126">Comments</span></span>

<span data-ttu-id="cc44f-127">Ответное сообщение на GetAttachment всегда будет содержать полный вложений; то есть все свойства всегда будут включены.</span><span class="sxs-lookup"><span data-stu-id="cc44f-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="cc44f-128">Для файлов вложений эти свойства — это [имя (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)и [контента](content.md).</span><span class="sxs-lookup"><span data-stu-id="cc44f-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="cc44f-129">Для вложений элемента, эти свойства — это [имя (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) и все свойства элемента, как если бы было использовано фигуры **AllProperties** GetItem звонка.</span><span class="sxs-lookup"><span data-stu-id="cc44f-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="cc44f-130">Элемент [AttachmentShape](attachmentshape.md) , если этот параметр указан, позволяет клиентского приложения запросить дополнительные расширенные свойства для вложений элемента.</span><span class="sxs-lookup"><span data-stu-id="cc44f-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="cc44f-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="cc44f-131">Successful response elements</span></span>

<span data-ttu-id="cc44f-132">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="cc44f-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="cc44f-133">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cc44f-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="cc44f-134">GetAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="cc44f-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="cc44f-135">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cc44f-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cc44f-136">GetAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cc44f-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="cc44f-137">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cc44f-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cc44f-138">Вложения</span><span class="sxs-lookup"><span data-stu-id="cc44f-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="cc44f-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="cc44f-140">Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="cc44f-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="cc44f-141">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="cc44f-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="cc44f-142">Контентная</span><span class="sxs-lookup"><span data-stu-id="cc44f-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="cc44f-143">См. также</span><span class="sxs-lookup"><span data-stu-id="cc44f-143">See also</span></span>



[<span data-ttu-id="cc44f-144">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="cc44f-145">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="cc44f-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

