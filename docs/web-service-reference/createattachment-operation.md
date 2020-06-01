---
title: Операция CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: Операция CreateAttachment создает элемент или вложенный файл и прикрепляет его к указанному элементу.
ms.openlocfilehash: 8028c56aa306774b54b39e5ee1ac0382b9113fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456572"
---
# <a name="createattachment-operation"></a><span data-ttu-id="afa09-103">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-103">CreateAttachment operation</span></span>

<span data-ttu-id="afa09-104">Операция CreateAttachment создает элемент или вложенный файл и прикрепляет его к указанному элементу.</span><span class="sxs-lookup"><span data-stu-id="afa09-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="afa09-105">Пример запроса файла CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="afa09-106">Описание</span><span class="sxs-lookup"><span data-stu-id="afa09-106">Description</span></span>

<span data-ttu-id="afa09-107">В приведенном ниже примере запроса CreateAttachment показано, как создать вложенный файл.</span><span class="sxs-lookup"><span data-stu-id="afa09-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="afa09-108">Код</span><span class="sxs-lookup"><span data-stu-id="afa09-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="afa09-109">Comment</span><span class="sxs-lookup"><span data-stu-id="afa09-109">Comment</span></span>

<span data-ttu-id="afa09-110">Необходимо указать имя вложения.</span><span class="sxs-lookup"><span data-stu-id="afa09-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="afa09-111">Идентификатор родительского элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="afa09-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="afa09-112">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="afa09-112">Request elements</span></span>

<span data-ttu-id="afa09-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="afa09-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="afa09-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="afa09-115">парентитемид</span><span class="sxs-lookup"><span data-stu-id="afa09-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="afa09-116">Вложения</span><span class="sxs-lookup"><span data-stu-id="afa09-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="afa09-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="afa09-118">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="afa09-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="afa09-119">Content</span><span class="sxs-lookup"><span data-stu-id="afa09-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="afa09-120">Пример успешного ответа файла CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="afa09-121">Описание</span><span class="sxs-lookup"><span data-stu-id="afa09-121">Description</span></span>

<span data-ttu-id="afa09-122">В следующем примере показан успешный ответ на запрос CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="afa09-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="afa09-123">Код</span><span class="sxs-lookup"><span data-stu-id="afa09-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="afa09-124">Comment</span><span class="sxs-lookup"><span data-stu-id="afa09-124">Comment</span></span>

<span data-ttu-id="afa09-125">Ответ содержит идентификатор вложенного файла.</span><span class="sxs-lookup"><span data-stu-id="afa09-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="afa09-126">Он также содержит идентификатор и ключ изменения корневого элемента.</span><span class="sxs-lookup"><span data-stu-id="afa09-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="afa09-127">Для сохранения удобочитаемости идентификаторы и ключ изменения были сокращены.</span><span class="sxs-lookup"><span data-stu-id="afa09-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="afa09-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="afa09-128">Successful response elements</span></span>

<span data-ttu-id="afa09-129">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="afa09-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="afa09-130">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="afa09-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="afa09-131">креатеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="afa09-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="afa09-132">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="afa09-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="afa09-133">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="afa09-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="afa09-134">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="afa09-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="afa09-135">Вложения</span><span class="sxs-lookup"><span data-stu-id="afa09-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="afa09-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="afa09-137">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="afa09-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="afa09-138">Пример запроса CreateAttachment для элемента</span><span class="sxs-lookup"><span data-stu-id="afa09-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="afa09-139">Описание</span><span class="sxs-lookup"><span data-stu-id="afa09-139">Description</span></span>

<span data-ttu-id="afa09-140">В приведенном ниже примере запроса CreateAttachment показано, как создать вложение элемента.</span><span class="sxs-lookup"><span data-stu-id="afa09-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="afa09-141">Код</span><span class="sxs-lookup"><span data-stu-id="afa09-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="afa09-142">Comment</span><span class="sxs-lookup"><span data-stu-id="afa09-142">Comment</span></span>

<span data-ttu-id="afa09-143">Необходимо указать имя вложения.</span><span class="sxs-lookup"><span data-stu-id="afa09-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="afa09-144">**Note (Примечание** ) Идентификатор родительского элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="afa09-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="afa09-145">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="afa09-145">Request elements</span></span>

<span data-ttu-id="afa09-146">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="afa09-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="afa09-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="afa09-148">парентитемид</span><span class="sxs-lookup"><span data-stu-id="afa09-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="afa09-149">Вложения</span><span class="sxs-lookup"><span data-stu-id="afa09-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="afa09-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="afa09-151">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="afa09-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="afa09-152">Message</span><span class="sxs-lookup"><span data-stu-id="afa09-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="afa09-153">Тема</span><span class="sxs-lookup"><span data-stu-id="afa09-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="afa09-154">Пример успешного ответа элемента CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="afa09-155">Описание</span><span class="sxs-lookup"><span data-stu-id="afa09-155">Description</span></span>

<span data-ttu-id="afa09-156">В следующем примере показан успешный ответ на запрос CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="afa09-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="afa09-157">Код</span><span class="sxs-lookup"><span data-stu-id="afa09-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a><span data-ttu-id="afa09-158">Comment</span><span class="sxs-lookup"><span data-stu-id="afa09-158">Comment</span></span>

<span data-ttu-id="afa09-159">Ответ содержит идентификатор нового вложения.</span><span class="sxs-lookup"><span data-stu-id="afa09-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="afa09-160">Он также содержит идентификатор и ключ изменения корневого элемента.</span><span class="sxs-lookup"><span data-stu-id="afa09-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="afa09-161">Корневым элементом является элемент, содержащий вложение.</span><span class="sxs-lookup"><span data-stu-id="afa09-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="afa09-162">Для сохранения удобочитаемости идентификаторы и ключ изменения были сокращены.</span><span class="sxs-lookup"><span data-stu-id="afa09-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="afa09-163">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="afa09-163">Successful response elements</span></span>

<span data-ttu-id="afa09-164">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="afa09-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="afa09-165">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="afa09-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="afa09-166">креатеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="afa09-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="afa09-167">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="afa09-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="afa09-168">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="afa09-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="afa09-169">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="afa09-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="afa09-170">Вложения</span><span class="sxs-lookup"><span data-stu-id="afa09-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="afa09-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="afa09-172">AttachmentId</span><span class="sxs-lookup"><span data-stu-id="afa09-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="afa09-173">Пример ответа на сообщение об ошибке CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="afa09-174">Описание</span><span class="sxs-lookup"><span data-stu-id="afa09-174">Description</span></span>

<span data-ttu-id="afa09-175">В следующем примере показан ответ об ошибке для запроса CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="afa09-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="afa09-176">Ошибка вызвана тем, что имя вложения не было указано.</span><span class="sxs-lookup"><span data-stu-id="afa09-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="afa09-177">Код</span><span class="sxs-lookup"><span data-stu-id="afa09-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="afa09-178">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="afa09-178">Error response elements</span></span>

<span data-ttu-id="afa09-179">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="afa09-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="afa09-180">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="afa09-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="afa09-181">креатеаттачментреспонсе</span><span class="sxs-lookup"><span data-stu-id="afa09-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="afa09-182">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="afa09-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="afa09-183">креатеаттачментреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="afa09-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="afa09-184">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="afa09-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="afa09-185">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="afa09-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="afa09-186">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="afa09-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="afa09-187">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="afa09-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="afa09-188">ексцептионфиелдури</span><span class="sxs-lookup"><span data-stu-id="afa09-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="afa09-189">Вложения</span><span class="sxs-lookup"><span data-stu-id="afa09-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="afa09-190">Примечания</span><span class="sxs-lookup"><span data-stu-id="afa09-190">Remarks</span></span>

<span data-ttu-id="afa09-191">Если к элементу присоединяется несколько вложений в одном цикле обработки, Рутитемчанжекэй в последнем ответе — это то, которое представляет новый ключ изменения элемента, содержащего вложения.</span><span class="sxs-lookup"><span data-stu-id="afa09-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="afa09-192">См. также</span><span class="sxs-lookup"><span data-stu-id="afa09-192">See also</span></span>



[<span data-ttu-id="afa09-193">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="afa09-194">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="afa09-194">GetAttachment operation</span></span>](getattachment-operation.md)

