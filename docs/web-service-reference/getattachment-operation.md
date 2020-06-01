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
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461291"
---
# <a name="getattachment-operation"></a><span data-ttu-id="7d72b-103">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-103">GetAttachment operation</span></span>

<span data-ttu-id="7d72b-104">Операция GetAttachment используется для получения существующих вложений на элементы в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="7d72b-104">The GetAttachment operation is used to retrieve existing attachments on items in the Exchange store.</span></span>
  
## <a name="getattachment-request-example"></a><span data-ttu-id="7d72b-105">Пример запроса GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-105">GetAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="7d72b-106">Описание</span><span class="sxs-lookup"><span data-stu-id="7d72b-106">Description</span></span>

<span data-ttu-id="7d72b-107">В приведенном ниже примере запроса GetAttachment показано, как получить вложение.</span><span class="sxs-lookup"><span data-stu-id="7d72b-107">The following example of GetAttachment request shows how to get an attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d72b-108">Код</span><span class="sxs-lookup"><span data-stu-id="7d72b-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="7d72b-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="7d72b-109">Comments</span></span>

<span data-ttu-id="7d72b-110">Элемент [аттачментшапе](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены.</span><span class="sxs-lookup"><span data-stu-id="7d72b-110">The [AttachmentShape](attachmentshape.md) element allows you to specify which attachment information should be returned.</span></span> <span data-ttu-id="7d72b-111">Пустой элемент [аттачментшапе](attachmentshape.md) является допустимым и будет отображать вложения без содержимого MIME для вложений элементов, тип текста текста и без дополнительных свойств.</span><span class="sxs-lookup"><span data-stu-id="7d72b-111">An empty [AttachmentShape](attachmentshape.md) element is valid and will render your attachments without MIME content for item attachments, with a text body type, and without any additional properties.</span></span> 
  
<span data-ttu-id="7d72b-112">Коллекция [аттачментидс](attachmentids.md) позволяет указать один или несколько идентификаторов вложений, которые необходимо вернуть.</span><span class="sxs-lookup"><span data-stu-id="7d72b-112">The [AttachmentIds](attachmentids.md) collection allows you to specify one or more attachment identifiers to return.</span></span> <span data-ttu-id="7d72b-113">Обратите внимание, что они относятся к типу Рекуестаттачментидтипе, поэтому для всех Аттачментидс, получаемых из **CreateAttachment** , необходимо удалить атрибуты **рутитемид** и **рутитемчанжекэй** , прежде чем передавать их в метод **GetAttachment**.</span><span class="sxs-lookup"><span data-stu-id="7d72b-113">Note that these are of type RequestAttachmentIdType, so any AttachmentIds that you receive from **CreateAttachment** must have the **RootItemId** and **RootItemChangeKey** attributes removed before passing them to **GetAttachment**.</span></span>
  
> [!NOTE]
> <span data-ttu-id="7d72b-114">Идентификатор и ключ вложения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="7d72b-114">The attachment identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="7d72b-115">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="7d72b-115">Request elements</span></span>

<span data-ttu-id="7d72b-116">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7d72b-116">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="7d72b-117">GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-117">GetAttachment</span></span>](getattachment.md)
    
- [<span data-ttu-id="7d72b-118">аттачментшапе</span><span class="sxs-lookup"><span data-stu-id="7d72b-118">AttachmentShape</span></span>](attachmentshape.md)
    
- [<span data-ttu-id="7d72b-119">аттачментидс</span><span class="sxs-lookup"><span data-stu-id="7d72b-119">AttachmentIds</span></span>](attachmentids.md)
    
- [<span data-ttu-id="7d72b-120">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="7d72b-120">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a><span data-ttu-id="7d72b-121">Пример отклика GetAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-121">GetAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="7d72b-122">Описание</span><span class="sxs-lookup"><span data-stu-id="7d72b-122">Description</span></span>

<span data-ttu-id="7d72b-123">В следующем примере показан успешный ответ на запрос GetAttachment.</span><span class="sxs-lookup"><span data-stu-id="7d72b-123">The following example shows a successful response to a GetAttachment request.</span></span> <span data-ttu-id="7d72b-124">В этом примере возвращается вложенный файл.</span><span class="sxs-lookup"><span data-stu-id="7d72b-124">This example returns a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="7d72b-125">Код</span><span class="sxs-lookup"><span data-stu-id="7d72b-125">Code</span></span>

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
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="7d72b-126">Комментарии</span><span class="sxs-lookup"><span data-stu-id="7d72b-126">Comments</span></span>

<span data-ttu-id="7d72b-127">В ответных сообщениях для GetAttachment всегда будет содержаться полное вложение; то есть все свойства всегда будут включены.</span><span class="sxs-lookup"><span data-stu-id="7d72b-127">The response messages for GetAttachment will always contain the full attachment; that is, all properties will always be included.</span></span> <span data-ttu-id="7d72b-128">Для вложений файлов эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), идентификатором [ContentId](contentid.md), [ContentLocation](contentlocation.md)и [содержимым](content.md).</span><span class="sxs-lookup"><span data-stu-id="7d72b-128">For file attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md), and [Content](content.md).</span></span> <span data-ttu-id="7d72b-129">Для вложений элемента эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) и всеми свойствами элемента, как если бы фигура **аллпропертиес** была использована при вызове GetItem.</span><span class="sxs-lookup"><span data-stu-id="7d72b-129">For item attachments, those properties are [Name (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) and all of the item's properties, as if the **AllProperties** shape had been used in a GetItem call.</span></span> <span data-ttu-id="7d72b-130">Элемент [аттачментшапе](attachmentshape.md) , если он присутствует, позволяет приложению-потребителю запрашивать дополнительные расширенные свойства для вложений элементов.</span><span class="sxs-lookup"><span data-stu-id="7d72b-130">The [AttachmentShape](attachmentshape.md) element, if present, will allow a consumer application to request additional extended properties for item attachments.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="7d72b-131">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="7d72b-131">Successful response elements</span></span>

<span data-ttu-id="7d72b-132">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7d72b-132">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="7d72b-133">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="7d72b-133">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="7d72b-134">жетаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="7d72b-134">GetAttachmentResponse</span></span>](getattachmentresponse.md)
    
- [<span data-ttu-id="7d72b-135">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="7d72b-135">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7d72b-136">жетаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="7d72b-136">GetAttachmentResponseMessage</span></span>](getattachmentresponsemessage.md)
    
- [<span data-ttu-id="7d72b-137">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="7d72b-137">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7d72b-138">Вложения</span><span class="sxs-lookup"><span data-stu-id="7d72b-138">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7d72b-139">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-139">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="7d72b-140">AttachmentId (GetAttachment и DeleteAttachment)</span><span class="sxs-lookup"><span data-stu-id="7d72b-140">AttachmentId (GetAttachment and DeleteAttachment)</span></span>](attachmentid-getattachment-and-deleteattachment.md)
    
- [<span data-ttu-id="7d72b-141">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="7d72b-141">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="7d72b-142">Content</span><span class="sxs-lookup"><span data-stu-id="7d72b-142">Content</span></span>](content.md)
    
## <a name="see-also"></a><span data-ttu-id="7d72b-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7d72b-143">See also</span></span>



[<span data-ttu-id="7d72b-144">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-144">CreateAttachment operation</span></span>](createattachment-operation.md)
  
[<span data-ttu-id="7d72b-145">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="7d72b-145">DeleteAttachment operation</span></span>](deleteattachment-operation.md)

