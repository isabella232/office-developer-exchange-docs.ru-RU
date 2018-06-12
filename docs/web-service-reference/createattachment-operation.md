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
description: Операция CreateAttachment создает вложение элемента или файла и подключает ее для заданного элемента.
ms.openlocfilehash: fed60275a007f2796c60d936def7a937e4982f29
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761855"
---
# <a name="createattachment-operation"></a><span data-ttu-id="ef19c-103">Операция CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-103">CreateAttachment operation</span></span>

<span data-ttu-id="ef19c-104">Операция CreateAttachment создает вложение элемента или файла и подключает ее для заданного элемента.</span><span class="sxs-lookup"><span data-stu-id="ef19c-104">The CreateAttachment operation creates either an item or file attachment and attaches it to the specified item.</span></span>
  
## <a name="file-createattachment-request-example"></a><span data-ttu-id="ef19c-105">Пример запроса CreateAttachment файла</span><span class="sxs-lookup"><span data-stu-id="ef19c-105">File CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="ef19c-106">Описание</span><span class="sxs-lookup"><span data-stu-id="ef19c-106">Description</span></span>

<span data-ttu-id="ef19c-107">В следующем примере запрос CreateAttachment показано, как создать подключение файла.</span><span class="sxs-lookup"><span data-stu-id="ef19c-107">The following example of a CreateAttachment request shows how to create a file attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef19c-108">Программа</span><span class="sxs-lookup"><span data-stu-id="ef19c-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="ef19c-109">Комментарий</span><span class="sxs-lookup"><span data-stu-id="ef19c-109">Comment</span></span>

<span data-ttu-id="ef19c-110">Необходимо указать имя для вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-110">A name for the attachment must be provided.</span></span>
  
> [!NOTE]
> <span data-ttu-id="ef19c-111">Идентификатор родительского элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ef19c-111">The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ef19c-112">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="ef19c-112">Request elements</span></span>

<span data-ttu-id="ef19c-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ef19c-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ef19c-114">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-114">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="ef19c-115">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="ef19c-115">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="ef19c-116">Вложения</span><span class="sxs-lookup"><span data-stu-id="ef19c-116">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ef19c-117">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-117">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="ef19c-118">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ef19c-118">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="ef19c-119">Контентная</span><span class="sxs-lookup"><span data-stu-id="ef19c-119">Content</span></span>](content.md)
    
## <a name="successful-file-createattachment-response-example"></a><span data-ttu-id="ef19c-120">Пример успешного ответа CreateAttachment файла</span><span class="sxs-lookup"><span data-stu-id="ef19c-120">Successful File CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="ef19c-121">Описание</span><span class="sxs-lookup"><span data-stu-id="ef19c-121">Description</span></span>

<span data-ttu-id="ef19c-122">В следующем примере показано успешного ответа на запрос CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="ef19c-122">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef19c-123">Программа</span><span class="sxs-lookup"><span data-stu-id="ef19c-123">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="ef19c-124">Комментарий</span><span class="sxs-lookup"><span data-stu-id="ef19c-124">Comment</span></span>

<span data-ttu-id="ef19c-125">Ответ содержит идентификатор вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-125">The response contains the identifier of the attached file.</span></span> <span data-ttu-id="ef19c-126">Он также содержит идентификатор и ключ изменения корневого элемента.</span><span class="sxs-lookup"><span data-stu-id="ef19c-126">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="ef19c-127">Идентификаторы элементов и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ef19c-127">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ef19c-128">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ef19c-128">Successful response elements</span></span>

<span data-ttu-id="ef19c-129">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ef19c-129">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ef19c-130">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ef19c-130">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ef19c-131">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ef19c-131">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="ef19c-132">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef19c-132">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ef19c-133">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef19c-133">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="ef19c-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ef19c-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ef19c-135">Вложения</span><span class="sxs-lookup"><span data-stu-id="ef19c-135">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ef19c-136">FileAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-136">FileAttachment</span></span>](fileattachment.md)
    
- [<span data-ttu-id="ef19c-137">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ef19c-137">AttachmentId</span></span>](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a><span data-ttu-id="ef19c-138">Пример запроса CreateAttachment элемента</span><span class="sxs-lookup"><span data-stu-id="ef19c-138">Item CreateAttachment request example</span></span>

### <a name="description"></a><span data-ttu-id="ef19c-139">Описание</span><span class="sxs-lookup"><span data-stu-id="ef19c-139">Description</span></span>

<span data-ttu-id="ef19c-140">В следующем примере запрос CreateAttachment показано, как создать элемент вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-140">The following example of a CreateAttachment request shows how to create an item attachment.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef19c-141">Программа</span><span class="sxs-lookup"><span data-stu-id="ef19c-141">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comment"></a><span data-ttu-id="ef19c-142">Комментарий</span><span class="sxs-lookup"><span data-stu-id="ef19c-142">Comment</span></span>

<span data-ttu-id="ef19c-143">Необходимо указать имя для вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-143">A name for the attachment must be provided.</span></span>
  
 <span data-ttu-id="ef19c-144">**Примечание** Идентификатор родительского элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ef19c-144">**Note** The parent item identifier and change key have been shortened to preserve readability.</span></span> 
  
### <a name="request-elements"></a><span data-ttu-id="ef19c-145">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="ef19c-145">Request elements</span></span>

<span data-ttu-id="ef19c-146">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ef19c-146">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ef19c-147">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-147">CreateAttachment</span></span>](createattachment.md)
    
- [<span data-ttu-id="ef19c-148">ParentItemId</span><span class="sxs-lookup"><span data-stu-id="ef19c-148">ParentItemId</span></span>](parentitemid.md)
    
- [<span data-ttu-id="ef19c-149">Вложения</span><span class="sxs-lookup"><span data-stu-id="ef19c-149">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ef19c-150">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-150">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="ef19c-151">Имя (AttachmentType)</span><span class="sxs-lookup"><span data-stu-id="ef19c-151">Name (AttachmentType)</span></span>](name-attachmenttype.md)
    
- [<span data-ttu-id="ef19c-152">Message</span><span class="sxs-lookup"><span data-stu-id="ef19c-152">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ef19c-153">Subject</span><span class="sxs-lookup"><span data-stu-id="ef19c-153">Subject</span></span>](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a><span data-ttu-id="ef19c-154">Пример успешного ответа CreateAttachment элемента</span><span class="sxs-lookup"><span data-stu-id="ef19c-154">Successful Item CreateAttachment response example</span></span>

### <a name="description"></a><span data-ttu-id="ef19c-155">Описание</span><span class="sxs-lookup"><span data-stu-id="ef19c-155">Description</span></span>

<span data-ttu-id="ef19c-156">В следующем примере показано успешного ответа на запрос CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="ef19c-156">The following example shows a successful response to the CreateAttachment request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef19c-157">Программа</span><span class="sxs-lookup"><span data-stu-id="ef19c-157">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comment"></a><span data-ttu-id="ef19c-158">Комментарий</span><span class="sxs-lookup"><span data-stu-id="ef19c-158">Comment</span></span>

<span data-ttu-id="ef19c-159">Ответ содержит идентификатор нового вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-159">The response contains the identifier of the new attachment.</span></span> <span data-ttu-id="ef19c-160">Он также содержит идентификатор и ключ изменения корневого элемента.</span><span class="sxs-lookup"><span data-stu-id="ef19c-160">It also contains the identifier and change key of the root item.</span></span> <span data-ttu-id="ef19c-161">Корневой элемент — это элемент, который содержит вложение.</span><span class="sxs-lookup"><span data-stu-id="ef19c-161">The root item is the item that contains the attachment.</span></span> <span data-ttu-id="ef19c-162">Идентификаторы элементов и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="ef19c-162">The item identifiers and change key have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ef19c-163">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ef19c-163">Successful response elements</span></span>

<span data-ttu-id="ef19c-164">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ef19c-164">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ef19c-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ef19c-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ef19c-166">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ef19c-166">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="ef19c-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef19c-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ef19c-168">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef19c-168">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="ef19c-169">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ef19c-169">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ef19c-170">Вложения</span><span class="sxs-lookup"><span data-stu-id="ef19c-170">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ef19c-171">ItemAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-171">ItemAttachment</span></span>](itemattachment.md)
    
- [<span data-ttu-id="ef19c-172">Идентификатора вложения AttachmentId</span><span class="sxs-lookup"><span data-stu-id="ef19c-172">AttachmentId</span></span>](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a><span data-ttu-id="ef19c-173">Пример ответа об ошибке CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-173">CreateAttachment Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ef19c-174">Описание</span><span class="sxs-lookup"><span data-stu-id="ef19c-174">Description</span></span>

<span data-ttu-id="ef19c-175">В следующем примере показано ошибочный ответ на запрос CreateAttachment.</span><span class="sxs-lookup"><span data-stu-id="ef19c-175">The following example shows an error response to the CreateAttachment request.</span></span> <span data-ttu-id="ef19c-176">Ошибка: того, что не было указано имя вложения.</span><span class="sxs-lookup"><span data-stu-id="ef19c-176">The error is due to the fact that the name of the attachment was not specified.</span></span>
  
### <a name="code"></a><span data-ttu-id="ef19c-177">Программа</span><span class="sxs-lookup"><span data-stu-id="ef19c-177">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ef19c-178">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="ef19c-178">Error response elements</span></span>

<span data-ttu-id="ef19c-179">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ef19c-179">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ef19c-180">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="ef19c-180">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ef19c-181">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="ef19c-181">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
    
- [<span data-ttu-id="ef19c-182">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ef19c-182">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ef19c-183">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ef19c-183">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
    
- [<span data-ttu-id="ef19c-184">MessageText</span><span class="sxs-lookup"><span data-stu-id="ef19c-184">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ef19c-185">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ef19c-185">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ef19c-186">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ef19c-186">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ef19c-187">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ef19c-187">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="ef19c-188">ExceptionFieldURI</span><span class="sxs-lookup"><span data-stu-id="ef19c-188">ExceptionFieldURI</span></span>](exceptionfielduri.md)
    
- [<span data-ttu-id="ef19c-189">Вложения</span><span class="sxs-lookup"><span data-stu-id="ef19c-189">Attachments</span></span>](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a><span data-ttu-id="ef19c-190">Замечания</span><span class="sxs-lookup"><span data-stu-id="ef19c-190">Remarks</span></span>

<span data-ttu-id="ef19c-191">Если несколько вложений присоединены к элементу в одном кругового пути, RootItemChangeKey в последнее сообщение ответа — это, соответствующий новый ключ изменения элемента с вложениями.</span><span class="sxs-lookup"><span data-stu-id="ef19c-191">If multiple attachments are attached to an item in a single round trip, the RootItemChangeKey in the last response message is the one that represents the new change key of the item that has the attachments.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ef19c-192">См. также</span><span class="sxs-lookup"><span data-stu-id="ef19c-192">See also</span></span>



[<span data-ttu-id="ef19c-193">Операция DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-193">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
  
[<span data-ttu-id="ef19c-194">Операция GetAttachment</span><span class="sxs-lookup"><span data-stu-id="ef19c-194">GetAttachment operation</span></span>](getattachment-operation.md)

