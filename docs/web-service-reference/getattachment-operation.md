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
description: Операция GetAttachment используется для получения существующих вложений на элементы в хранилище Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762701"
---
# <a name="getattachment-operation"></a><span data-ttu-id="69493-103">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-103">GetAttachment operation</span></span>

<span data-ttu-id="69493-104">Операция GetAttachment используется для получения существующих вложений на элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="69493-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="69493-105">Пример запроса GetAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="69493-106">Описание</span><span class="sxs-lookup"><span data-stu-id="69493-106">Description</span></span>

<span data-ttu-id="69493-107">В приведенном ниже примере запроса GetAttachment показано, как получить вложение.</span><span class="sxs-lookup"><span data-stu-id="69493-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="69493-108">Код</span><span class="sxs-lookup"><span data-stu-id="69493-108">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="69493-109">Comments</span><span class="sxs-lookup"><span data-stu-id="69493-109">Comments</span></span>

<span data-ttu-id="69493-110">Элемент [аттачментшапе](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="69493-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="69493-111">Пустой элемент [аттачментшапе](attachmentshape.md) является допустимым и будет отображать вложения без содержимого MIME для вложений элементов, тип текста текста и без дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="69493-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="69493-112">Коллекция [аттачментидс](attachmentids.md) позволяет указать один или несколько идентификаторов вложений, которые необходимо вернуть.</span><span class="sxs-lookup"><span data-stu-id="69493-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="69493-113">Обратите внимание, что они относятся к типу Рекуестаттачментидтипе, поэтому для всех Аттачментидс, получаемых из **CreateAttachment** , необходимо удалить атрибуты **рутитемид** и **рутитемчанжекэй** , прежде чем передавать их в метод **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="69493-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="69493-114">Идентификатор и ключ вложения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="69493-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="69493-115">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="69493-115">Request elements</span></span>

<span data-ttu-id="69493-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="69493-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="69493-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="69493-118">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="69493-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="69493-119">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="69493-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="69493-120">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="69493-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="69493-121">Пример отклика GetAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="69493-122">Описание</span><span class="sxs-lookup"><span data-stu-id="69493-122">Description</span></span>

<span data-ttu-id="69493-123">В следующем примере показан успешный ответ на запрос GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="69493-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="69493-124">В этом примере возвращается вложенный файл.</span><span class="sxs-lookup"><span data-stu-id="69493-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="69493-125">Код</span><span class="sxs-lookup"><span data-stu-id="69493-125">Code</span></span>

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

### <a name="comments"></a><span data-ttu-id="69493-126">Comments</span><span class="sxs-lookup"><span data-stu-id="69493-126">Comments</span></span>

<span data-ttu-id="69493-127">В ответных сообщениях для GetAttachment всегда будет содержаться полное вложение; то есть все свойства всегда будут включены.</span><span class="sxs-lookup"><span data-stu-id="69493-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="69493-128">Для вложений файлов эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), идентификатором [ContentId](contentid.md), [ContentLocation](contentlocation.md)и [содержимым](content.md).</span><span class="sxs-lookup"><span data-stu-id="69493-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="69493-129">Для вложений элемента эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) и всеми свойствами элемента, как если бы фигура **аллпропертиес** была использована при вызове GetItem.</span><span class="sxs-lookup"><span data-stu-id="69493-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="69493-130">Элемент [аттачментшапе](attachmentshape.md) , если он присутствует, позволяет приложению-потребителю запрашивать дополнительные расширенные свойства для вложений элементов.</span><span class="sxs-lookup"><span data-stu-id="69493-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="69493-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="69493-131">Successful response elements</span></span>

<span data-ttu-id="69493-132">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="69493-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="69493-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="69493-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="69493-134">жетаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="69493-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="69493-135">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="69493-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="69493-136">жетаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="69493-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="69493-137">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="69493-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="69493-138">Вложения</span><span class="sxs-lookup"><span data-stu-id="69493-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="69493-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="69493-140">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="69493-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="69493-141">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="69493-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="69493-142">Статья</span><span class="sxs-lookup"><span data-stu-id="69493-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="69493-143">См. также</span><span class="sxs-lookup"><span data-stu-id="69493-143">See also</span></span>



[<span data-ttu-id="69493-144">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="69493-145">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="69493-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

