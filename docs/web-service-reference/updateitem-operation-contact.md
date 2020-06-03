---
title: Операция UpdateItem (Contact)
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
ms.openlocfilehash: 66e1b91ea3154d8a501339aed7b398970e8f5392
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459828"
---
# <a name="updateitem-operation-contact"></a><span data-ttu-id="5ca6b-103">Операция UpdateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-103">UpdateItem operation (contact)</span></span>

<span data-ttu-id="5ca6b-104">Операция UpdateItem используется для обновления свойств элемента контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-104">The UpdateItem operation is used to update contact item properties in the Exchange store.</span></span>
  
## <a name="updateitem-contact-request-example"></a><span data-ttu-id="5ca6b-105">Пример запроса UpdateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-105">UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5ca6b-106">Description</span><span class="sxs-lookup"><span data-stu-id="5ca6b-106">Description</span></span>

<span data-ttu-id="5ca6b-107">В приведенном ниже примере кода показано, как обновить адрес электронной почты контакта.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-107">The following code example shows how to update the e-mail address of a contact.</span></span>
  
### <a name="code"></a><span data-ttu-id="5ca6b-108">Код</span><span class="sxs-lookup"><span data-stu-id="5ca6b-108">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
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

### <a name="comments"></a><span data-ttu-id="5ca6b-109">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5ca6b-109">Comments</span></span>

<span data-ttu-id="5ca6b-110">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-110">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="request-elements"></a><span data-ttu-id="5ca6b-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="5ca6b-111">Request elements</span></span>

<span data-ttu-id="5ca6b-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5ca6b-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5ca6b-113">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5ca6b-113">UpdateItem</span></span>](updateitem.md)
    
- [<span data-ttu-id="5ca6b-114">итемчанжес</span><span class="sxs-lookup"><span data-stu-id="5ca6b-114">ItemChanges</span></span>](itemchanges.md)
    
- [<span data-ttu-id="5ca6b-115">ItemChange</span><span class="sxs-lookup"><span data-stu-id="5ca6b-115">ItemChange</span></span>](itemchange.md)
    
- [<span data-ttu-id="5ca6b-116">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5ca6b-116">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5ca6b-117">Обновления (элемент)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-117">Updates (Item)</span></span>](updates-item.md)
    
- [<span data-ttu-id="5ca6b-118">сетитемфиелд</span><span class="sxs-lookup"><span data-stu-id="5ca6b-118">SetItemField</span></span>](setitemfield.md)
    
- [<span data-ttu-id="5ca6b-119">индекседфиелдури</span><span class="sxs-lookup"><span data-stu-id="5ca6b-119">IndexedFieldURI</span></span>](indexedfielduri.md)
    
- <span data-ttu-id="5ca6b-120">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="5ca6b-120">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="5ca6b-121">EmailAddresses</span><span class="sxs-lookup"><span data-stu-id="5ca6b-121">EmailAddresses</span></span>](emailaddresses.md)
    
- [<span data-ttu-id="5ca6b-122">Запись (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-122">Entry (EmailAddress)</span></span>](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a><span data-ttu-id="5ca6b-123">Успешный ответ UpdateItem (контакт)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-123">Successful UpdateItem (Contact) Response</span></span>

### <a name="description"></a><span data-ttu-id="5ca6b-124">Description</span><span class="sxs-lookup"><span data-stu-id="5ca6b-124">Description</span></span>

<span data-ttu-id="5ca6b-125">В следующем примере кода показан успешный ответ UpdateItem.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-125">The following code example shows a successful UpdateItem response.</span></span>
  
### <a name="code"></a><span data-ttu-id="5ca6b-126">Код</span><span class="sxs-lookup"><span data-stu-id="5ca6b-126">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UpdateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="5ca6b-127">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5ca6b-127">Comments</span></span>

<span data-ttu-id="5ca6b-128">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-128">The item identifier has been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="5ca6b-129">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="5ca6b-129">Successful response elements</span></span>

<span data-ttu-id="5ca6b-130">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5ca6b-130">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5ca6b-131">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="5ca6b-131">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5ca6b-132">упдатеитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="5ca6b-132">UpdateItemResponse</span></span>](updateitemresponse.md)
    
- [<span data-ttu-id="5ca6b-133">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="5ca6b-133">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5ca6b-134">упдатеитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="5ca6b-134">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
    
- [<span data-ttu-id="5ca6b-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5ca6b-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5ca6b-136">Элементы (Нонемптяррайофаллитемстипе)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-136">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- <span data-ttu-id="5ca6b-137">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="5ca6b-137">[Contact](contact.md)</span></span>
    
- [<span data-ttu-id="5ca6b-138">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="5ca6b-138">ItemId</span></span>](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a><span data-ttu-id="5ca6b-139">Недопустимый пример запроса UpdateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-139">Invalid UpdateItem (Contact) request example</span></span>

### <a name="description"></a><span data-ttu-id="5ca6b-140">Description</span><span class="sxs-lookup"><span data-stu-id="5ca6b-140">Description</span></span>

<span data-ttu-id="5ca6b-141">В следующем примере кода показан недопустимый запрос.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-141">The following code example shows an invalid request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5ca6b-142">Код</span><span class="sxs-lookup"><span data-stu-id="5ca6b-142">Code</span></span>

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <UpdateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
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

### <a name="comments"></a><span data-ttu-id="5ca6b-143">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5ca6b-143">Comments</span></span>

<span data-ttu-id="5ca6b-144">Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-144">The item identifier has been shortened to preserve readability.</span></span>
  
## <a name="updateitem-contact-error-response"></a><span data-ttu-id="5ca6b-145">Ответ на сообщение об ошибке UpdateItem (Contact)</span><span class="sxs-lookup"><span data-stu-id="5ca6b-145">UpdateItem (Contact) error response</span></span>

### <a name="description"></a><span data-ttu-id="5ca6b-146">Description</span><span class="sxs-lookup"><span data-stu-id="5ca6b-146">Description</span></span>

<span data-ttu-id="5ca6b-147">В следующем примере кода показан ответ об ошибке для запроса UpdateItem (Contact).</span><span class="sxs-lookup"><span data-stu-id="5ca6b-147">The following code example shows an error response to an UpdateItem (Contact) request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5ca6b-148">Код</span><span class="sxs-lookup"><span data-stu-id="5ca6b-148">Code</span></span>

```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <soap:faultcode>Client</soap:faultcode>
      <soap:faultstring>The request failed schema validation.</soap:faultstring>
      <detail>
        <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The 'Key' attribute is invalid - The value 'EmailAddress4' is invalid according to its data type 'https://schemas.microsoft.com/exchange/services/2006/types:EmailAddressKeyType' - The Enumeration constraint failed.</e:Message>
        <e:Line xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">17</e:Line>
        <e:Position xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">19</e:Position>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5ca6b-149">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5ca6b-149">Comments</span></span>

<span data-ttu-id="5ca6b-150">Некоторые элементы, используемые в теле SOAP ошибочного ответа, вызванного ошибкой проверки схемы, не определены в схемах messages или Types.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-150">Some elements that are used in the SOAP body of an error response that is caused by a schema validation error are not defined in the messages or types schemas.</span></span> <span data-ttu-id="5ca6b-151">Элемент **detail** содержит сведения об ошибке.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-151">The **detail** element contains information about the error.</span></span> <span data-ttu-id="5ca6b-152">Элемент [респонсекоде](responsecode.md) содержит код ошибки.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-152">The [ResponseCode](responsecode.md) element contains the error code.</span></span> <span data-ttu-id="5ca6b-153">Элемент [Message](message-ex15websvcsotherref.md) содержит объяснение ошибки, если она доступна.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-153">The [Message](message-ex15websvcsotherref.md) element contains an explanation for the error, if one is available.</span></span> <span data-ttu-id="5ca6b-154">Элемент **line** описывает номер строки, в которой произошла ошибка проверки схемы.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-154">The **Line** element describes the line number where the schema validation error occurred.</span></span> <span data-ttu-id="5ca6b-155">Элемент **position** описывает позицию из самого левого знака XML-документа.</span><span class="sxs-lookup"><span data-stu-id="5ca6b-155">The **Position** element describes the position from the leftmost character of the XML document.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="5ca6b-156">См. также</span><span class="sxs-lookup"><span data-stu-id="5ca6b-156">See also</span></span>



[<span data-ttu-id="5ca6b-157">Операция UpdateItem</span><span class="sxs-lookup"><span data-stu-id="5ca6b-157">UpdateItem operation</span></span>](updateitem-operation.md)

