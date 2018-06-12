---
title: Операция UpdateItem (контактов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 298fdd71-a83d-4407-9728-4f0a8e2d857c
description: Операция UpdateItem используется для обновления свойств элемента контакта в хранилище Exchange.
ms.openlocfilehash: f2a501ce8e69068cd30b58011adf4defc68ce365
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840348"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="613d7-103">Операция UpdateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="613d7-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="613d7-104">Операция UpdateItem используется для обновления свойств элемента контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="613d7-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="613d7-105">Пример запроса UpdateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="613d7-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="613d7-106">Описание</span><span class="sxs-lookup"><span data-stu-id="613d7-106">Description</span></span>

<span data-ttu-id="613d7-107">В следующем примере кода показано, как обновить контактный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="613d7-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="613d7-108">Программа</span><span class="sxs-lookup"><span data-stu-id="613d7-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAA=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress1"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress1">changedemail@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="613d7-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="613d7-109">Comments</span></span>

<span data-ttu-id="613d7-110">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="613d7-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="613d7-111">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="613d7-111">Request elements</span></span>

<span data-ttu-id="613d7-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="613d7-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="613d7-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="613d7-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="613d7-114">ItemChanges</span><span class="sxs-lookup"><span data-stu-id="613d7-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="613d7-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="613d7-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="613d7-116">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="613d7-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="613d7-117">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="613d7-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="613d7-118">SetItemField</span><span class="sxs-lookup"><span data-stu-id="613d7-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="613d7-119">IndexedFieldURI</span><span class="sxs-lookup"><span data-stu-id="613d7-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- [<span data-ttu-id="613d7-120">Контакт</span><span class="sxs-lookup"><span data-stu-id="613d7-120">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="613d7-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="613d7-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="613d7-122">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="613d7-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="613d7-123">Успешные UpdateItem (контакт) ответа</span><span class="sxs-lookup"><span data-stu-id="613d7-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="613d7-124">Описание</span><span class="sxs-lookup"><span data-stu-id="613d7-124">Description</span></span>

<span data-ttu-id="613d7-125">В следующем примере кода показано успешного ответа UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="613d7-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="613d7-126">Программа</span><span class="sxs-lookup"><span data-stu-id="613d7-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UpdateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtAE=" ChangeKey="EQAAABYx" />
            </t:Contact>
          </m:Items>
        </m:UpdateItemResponseMessage>
      </m:ResponseMessages>
    </UpdateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="613d7-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="613d7-127">Comments</span></span>

<span data-ttu-id="613d7-128">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="613d7-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="613d7-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="613d7-129">Successful response elements</span></span>

<span data-ttu-id="613d7-130">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="613d7-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="613d7-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="613d7-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="613d7-132">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="613d7-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="613d7-133">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="613d7-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="613d7-134">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="613d7-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="613d7-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="613d7-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="613d7-136">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="613d7-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="613d7-137">Контакт</span><span class="sxs-lookup"><span data-stu-id="613d7-137">Contact</span></span>](contact.md)
    
- [<span data-ttu-id="613d7-138">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="613d7-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="613d7-139">Пример запроса недопустимый UpdateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="613d7-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="613d7-140">Описание</span><span class="sxs-lookup"><span data-stu-id="613d7-140">Description</span></span>

<span data-ttu-id="613d7-141">В следующем примере кода показано недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="613d7-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="613d7-142">Программа</span><span class="sxs-lookup"><span data-stu-id="613d7-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                ConflictResolution="AlwaysOverwrite">
      <ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="AAAtAEF=" ChangeKey="EQAAABYi" />
          <t:Updates>
            <t:SetItemField>
              <t:IndexedFieldURI FieldURI="contacts:EmailAddress" FieldIndex="EmailAddress4"/>
              <t:Contact>
                <t:EmailAddresses>
                  <t:Entry Key="EmailAddress4">changedemail2@example.com</t:Entry>
                </t:EmailAddresses>
              </t:Contact>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </ItemChanges>
    </UpdateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="613d7-143">Комментарии</span><span class="sxs-lookup"><span data-stu-id="613d7-143">Comments</span></span>

<span data-ttu-id="613d7-144">Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="613d7-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="613d7-145">Отклик UpdateItem (контактов)</span><span class="sxs-lookup"><span data-stu-id="613d7-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="613d7-146">Описание</span><span class="sxs-lookup"><span data-stu-id="613d7-146">Description</span></span>

<span data-ttu-id="613d7-147">В следующем примере кода показано ошибочный ответ на запрос UpdateItem (контактов).</span><span class="sxs-lookup"><span data-stu-id="613d7-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="613d7-148">Программа</span><span class="sxs-lookup"><span data-stu-id="613d7-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'http://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="613d7-149">Комментарии</span><span class="sxs-lookup"><span data-stu-id="613d7-149">Comments</span></span>

<span data-ttu-id="613d7-150">Некоторые элементы, которые используются в тексте SOAP возврату ошибки, возникающие при ошибке проверки схемы не определены в схемах типов или сообщений.</span><span class="sxs-lookup"><span data-stu-id="613d7-150">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas.</span></span> <span data-ttu-id="613d7-151">Элемент **детализации** содержит сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="613d7-151">The **detail** element contains information about the error.</span></span> <span data-ttu-id="613d7-152">Элемент [ResponseCode](responsecode.md) содержит код ошибки.</span><span class="sxs-lookup"><span data-stu-id="613d7-152">The [ResponseCode](responsecode.md) element contains the error code.</span></span> <span data-ttu-id="613d7-153">Элемент [сообщение](message-ex15websvcsotherref.md) содержит описание ошибки, если она доступна.</span><span class="sxs-lookup"><span data-stu-id="613d7-153">The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available.</span></span> <span data-ttu-id="613d7-154">Элемент **строки** описываются номер строки, где произошла ошибка проверки схемы.</span><span class="sxs-lookup"><span data-stu-id="613d7-154">The **Line** element describes the line number where the schema validation error occurred.</span></span> <span data-ttu-id="613d7-155">Элемент **позиции** описывает положение из первого символа XML-документа.</span><span class="sxs-lookup"><span data-stu-id="613d7-155">The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="613d7-156">См. также</span><span class="sxs-lookup"><span data-stu-id="613d7-156">See also</span></span>



[<span data-ttu-id="613d7-157">UpdateItem Operation</span><span class="sxs-lookup"><span data-stu-id="613d7-157">UpdateItem operation</span></span>](updateitem-operation.md)

