---
title: Операции GetItem (сообщение электронной почты)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: e8492e3b-1c8d-4b14-8070-9530f8306edd
description: Операции GetItem позволяет пользователям получать доступ к информации о сообщениях электронной почты.
ms.openlocfilehash: 133a893ec7cd0c206d9db573f8b952eb3c2286df
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762833"
---
# <a name="getitem-operation-email-message"></a><span data-ttu-id="d3434-103">Операции GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="d3434-103">GetItem operation (email message)</span></span>

<span data-ttu-id="d3434-104">Операции GetItem позволяет пользователям получать доступ к информации о сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d3434-104">The GetItem operation allows the user to access information about e-mail messages.</span></span>
  
## <a name="using-the-getitem-operation-for-messages"></a><span data-ttu-id="d3434-105">С помощью операции GetItem для сообщений</span><span class="sxs-lookup"><span data-stu-id="d3434-105">Using the GetItem Operation for Messages</span></span>

<span data-ttu-id="d3434-106">Запрос GetItem должен иметь следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="d3434-106">The GetItem request must have the following information:</span></span>
  
- <span data-ttu-id="d3434-107">Элемент [ItemId](itemid.md) для идентификации возвращаемых данных элемента.</span><span class="sxs-lookup"><span data-stu-id="d3434-107">The [ItemId](itemid.md) element to identify the item information to return.</span></span> 
    
- <span data-ttu-id="d3434-108">Элемент [ItemShape](itemshape.md) для идентификации возвращаемых свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="d3434-108">The [ItemShape](itemshape.md) element to identify the item properties to return.</span></span> 
    
## <a name="getitem-request-example"></a><span data-ttu-id="d3434-109">Пример запроса GetItem</span><span class="sxs-lookup"><span data-stu-id="d3434-109">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="d3434-110">Описание</span><span class="sxs-lookup"><span data-stu-id="d3434-110">Description</span></span>

<span data-ttu-id="d3434-111">Приведенный ниже запрос GetItem показано, как получить доступ к информации о сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="d3434-111">The following example of a GetItem request shows how to access information about e-mail messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="d3434-112">Программа</span><span class="sxs-lookup"><span data-stu-id="d3434-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem
      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <ItemShape>
        <t:BaseShape>Default</t:BaseShape>
        <t:IncludeMimeContent>true</t:IncludeMimeContent>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AAAlAF" ChangeKey="CQAAAB" />
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="d3434-113">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="d3434-113">Request elements</span></span>

<span data-ttu-id="d3434-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d3434-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="d3434-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="d3434-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="d3434-116">ItemShape</span><span class="sxs-lookup"><span data-stu-id="d3434-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="d3434-117">BaseShape</span><span class="sxs-lookup"><span data-stu-id="d3434-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="d3434-118">IncludeMimeContent</span><span class="sxs-lookup"><span data-stu-id="d3434-118">IncludeMimeContent</span></span>](includemimecontent.md)
    
- [<span data-ttu-id="d3434-119">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="d3434-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="d3434-120">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="d3434-120">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-e-mail-message-response-example"></a><span data-ttu-id="d3434-121">Пример успешного ответа GetItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="d3434-121">Successful GetItem (E-mail Message) response example</span></span>

### <a name="description"></a><span data-ttu-id="d3434-122">Описание</span><span class="sxs-lookup"><span data-stu-id="d3434-122">Description</span></span>

<span data-ttu-id="d3434-123">В следующем примере показано успешного ответа на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="d3434-123">The following example shows a successful response to the GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="d3434-124">Программа</span><span class="sxs-lookup"><span data-stu-id="d3434-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:MimeContent CharacterSet="UTF-8">UmVjZWl</t:MimeContent>
              <t:ItemId Id="AAAlAFVz" ChangeKey="CQAAAB" />
              <t:Subject />
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="HTML">
                <html dir="ltr">
                  <head>
                    <meta http-equiv="Content-Type" content="text/html; charset=utf-8">
                      <meta content="MSHTML 6.00.3790.2759" name="GENERATOR">
                        <style title="owaParaStyle">P { MARGIN-TOP: 0px; MARGIN-BOTTOM: 0px } </style>
                      </head>
                  <body ocsi="x">
                    <div dir="ltr">
                      <font face="Tahoma" color="#000000" size="2"></font>&amp;nbsp;
                    </div>
                  </body>
                </html>
              </t:Body>
              <t:Size>881</t:Size>
              <t:DateTimeSent>2006-10-28T01:37:06Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-10-28T01:37:06Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ReplyToItem />
                <t:ReplyAllToItem />
                <t:ForwardItem />
              </t:ResponseObjects>
              <t:HasAttachments>false</t:HasAttachments>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>User1</t:Name>
                  <t:EmailAddress>User1@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:ToRecipients>
              <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
              <t:IsDeliveryReceiptRequested>false</t:IsDeliveryReceiptRequested>
              <t:From>
                <t:Mailbox>
                  <t:Name>User2</t:Name>
                  <t:EmailAddress>User2@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:From>
              <t:IsRead>false</t:IsRead>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="d3434-125">Комментарии</span><span class="sxs-lookup"><span data-stu-id="d3434-125">Comments</span></span>

<span data-ttu-id="d3434-126">Содержимое MIME, папки и идентификаторы элементов URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="d3434-126">The MIME content, folder, and item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="d3434-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="d3434-127">Successful response elements</span></span>

<span data-ttu-id="d3434-128">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d3434-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="d3434-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d3434-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d3434-130">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="d3434-130">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="d3434-131">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3434-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d3434-132">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3434-132">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="d3434-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3434-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d3434-134">Элементы</span><span class="sxs-lookup"><span data-stu-id="d3434-134">Items</span></span>](items.md)
    
- [<span data-ttu-id="d3434-135">Message</span><span class="sxs-lookup"><span data-stu-id="d3434-135">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="d3434-136">MimeContent</span><span class="sxs-lookup"><span data-stu-id="d3434-136">MimeContent</span></span>](mimecontent.md)
    
- [<span data-ttu-id="d3434-137">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="d3434-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="d3434-138">Subject</span><span class="sxs-lookup"><span data-stu-id="d3434-138">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="d3434-139">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="d3434-139">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="d3434-140">Body</span><span class="sxs-lookup"><span data-stu-id="d3434-140">Body</span></span>](body.md)
    
- [<span data-ttu-id="d3434-141">Размер</span><span class="sxs-lookup"><span data-stu-id="d3434-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="d3434-142">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="d3434-142">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="d3434-143">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="d3434-143">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="d3434-144">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="d3434-144">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="d3434-145">ReplyToItem</span><span class="sxs-lookup"><span data-stu-id="d3434-145">ReplyToItem</span></span>](replytoitem.md)
    
- [<span data-ttu-id="d3434-146">ReplyAllToItem</span><span class="sxs-lookup"><span data-stu-id="d3434-146">ReplyAllToItem</span></span>](replyalltoitem.md)
    
- [<span data-ttu-id="d3434-147">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="d3434-147">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="d3434-148">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="d3434-148">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="d3434-149">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="d3434-149">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="d3434-150">Mailbox</span><span class="sxs-lookup"><span data-stu-id="d3434-150">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="d3434-151">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d3434-151">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="d3434-152">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="d3434-152">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="d3434-153">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="d3434-153">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="d3434-154">IsReadReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d3434-154">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md)
    
- [<span data-ttu-id="d3434-155">IsDeliveryReceiptRequested</span><span class="sxs-lookup"><span data-stu-id="d3434-155">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md)
    
- [<span data-ttu-id="d3434-156">From</span><span class="sxs-lookup"><span data-stu-id="d3434-156">From</span></span>](from.md)
    
- [<span data-ttu-id="d3434-157">IsRead</span><span class="sxs-lookup"><span data-stu-id="d3434-157">IsRead</span></span>](isread.md)
    
## <a name="getitem-e-mail-message-error-response-example"></a><span data-ttu-id="d3434-158">Пример ответа об ошибке GetItem (сообщения электронной почты)</span><span class="sxs-lookup"><span data-stu-id="d3434-158">GetItem (E-mail Message) Error response example</span></span>

### <a name="description"></a><span data-ttu-id="d3434-159">Описание</span><span class="sxs-lookup"><span data-stu-id="d3434-159">Description</span></span>

<span data-ttu-id="d3434-160">В следующем примере показано возврату ошибки GetItem запрос.</span><span class="sxs-lookup"><span data-stu-id="d3434-160">The following example shows an error response to a GetItem request.</span></span> <span data-ttu-id="d3434-161">Ошибка была вызвана при попытке получения недопустимый дополнительные свойства.</span><span class="sxs-lookup"><span data-stu-id="d3434-161">The error was caused by an attempt to get an invalid additional property.</span></span>
  
### <a name="code"></a><span data-ttu-id="d3434-162">Программа</span><span class="sxs-lookup"><span data-stu-id="d3434-162">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Error">
          <m:MessageText>Property is not valid for this object type.</m:MessageText>
          <m:ResponseCode>ErrorInvalidPropertyRequest</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:FieldURI FieldURI="meeting:AssociatedCalendarItemId" />
          </m:MessageXml>
          <m:Items />
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="d3434-163">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="d3434-163">Error response elements</span></span>

<span data-ttu-id="d3434-164">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d3434-164">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="d3434-165">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d3434-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="d3434-166">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="d3434-166">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="d3434-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d3434-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="d3434-168">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d3434-168">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="d3434-169">MessageText</span><span class="sxs-lookup"><span data-stu-id="d3434-169">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d3434-170">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d3434-170">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d3434-171">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d3434-171">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="d3434-172">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d3434-172">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="d3434-173">FieldURI</span><span class="sxs-lookup"><span data-stu-id="d3434-173">FieldURI</span></span>](fielduri.md)
    
## <a name="see-also"></a><span data-ttu-id="d3434-174">См. также</span><span class="sxs-lookup"><span data-stu-id="d3434-174">See also</span></span>



[<span data-ttu-id="d3434-175">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="d3434-175">GetItem operation</span></span>](getitem-operation.md)

