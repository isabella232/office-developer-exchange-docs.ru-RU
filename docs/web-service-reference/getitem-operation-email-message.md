---
title: Операция GetItem (сообщение электронной почты)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- GetItem
api_type:
- schema
ms.assetid: e8492e3b-1c8d-4b14-8070-9530f8306edd
description: Операция GetItem позволяет пользователю получать доступ к сведениям о сообщениях электронной почты.
localization_priority: Priority
ms.openlocfilehash: f8be01cad3d4c4534f66593cbe8bcee477726972
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459996"
---
# <a name="getitem-operation-email-message"></a><span data-ttu-id="ac78e-103">Операция GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="ac78e-103">GetItem operation (email message)</span></span>

<span data-ttu-id="ac78e-104">Операция GetItem позволяет пользователю получать доступ к сведениям о сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ac78e-104">The GetItem operation allows the user to access information about e-mail messages.</span></span>
  
## <a name="using-the-getitem-operation-for-messages"></a><span data-ttu-id="ac78e-105">Использование операции GetItem для сообщений</span><span class="sxs-lookup"><span data-stu-id="ac78e-105">Using the GetItem Operation for Messages</span></span>

<span data-ttu-id="ac78e-106">Запрос GetItem должен иметь следующие сведения:</span><span class="sxs-lookup"><span data-stu-id="ac78e-106">The GetItem request must have the following information:</span></span>
  
- <span data-ttu-id="ac78e-107">Элемент [ItemId](itemid.md) для определения возвращаемых сведений об элементе.</span><span class="sxs-lookup"><span data-stu-id="ac78e-107">The [ItemId](itemid.md) element to identify the item information to return.</span></span> 
    
- <span data-ttu-id="ac78e-108">Элемент [итемшапе](itemshape.md) для определения возвращаемых свойств элемента.</span><span class="sxs-lookup"><span data-stu-id="ac78e-108">The [ItemShape](itemshape.md) element to identify the item properties to return.</span></span> 
    
## <a name="getitem-request-example"></a><span data-ttu-id="ac78e-109">Пример запроса GetItem</span><span class="sxs-lookup"><span data-stu-id="ac78e-109">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="ac78e-110">Description</span><span class="sxs-lookup"><span data-stu-id="ac78e-110">Description</span></span>

<span data-ttu-id="ac78e-111">В приведенном ниже примере запроса GetItem показано, как получить доступ к сведениям о сообщениях электронной почты.</span><span class="sxs-lookup"><span data-stu-id="ac78e-111">The following example of a GetItem request shows how to access information about e-mail messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="ac78e-112">Код</span><span class="sxs-lookup"><span data-stu-id="ac78e-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope
  xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
  xmlns:xsd="http://www.w3.org/2001/XMLSchema"
  xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem
      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="request-elements"></a><span data-ttu-id="ac78e-113">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="ac78e-113">Request elements</span></span>

<span data-ttu-id="ac78e-114">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac78e-114">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ac78e-115">GetItem</span><span class="sxs-lookup"><span data-stu-id="ac78e-115">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="ac78e-116">итемшапе</span><span class="sxs-lookup"><span data-stu-id="ac78e-116">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="ac78e-117">басешапе</span><span class="sxs-lookup"><span data-stu-id="ac78e-117">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="ac78e-118">инклудемимеконтент</span><span class="sxs-lookup"><span data-stu-id="ac78e-118">IncludeMimeContent</span></span>](includemimecontent.md)
    
- [<span data-ttu-id="ac78e-119">итемидс</span><span class="sxs-lookup"><span data-stu-id="ac78e-119">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="ac78e-120">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ac78e-120">ItemId</span></span>](itemid.md)
    
## <a name="successful-getitem-e-mail-message-response-example"></a><span data-ttu-id="ac78e-121">Пример ответа на сообщение об успешном выполнении операции GetItem (сообщение электронной почты)</span><span class="sxs-lookup"><span data-stu-id="ac78e-121">Successful GetItem (E-mail Message) response example</span></span>

### <a name="description"></a><span data-ttu-id="ac78e-122">Description</span><span class="sxs-lookup"><span data-stu-id="ac78e-122">Description</span></span>

<span data-ttu-id="ac78e-123">В следующем примере показан успешный ответ на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="ac78e-123">The following example shows a successful response to the GetItem request.</span></span>
  
### <a name="code"></a><span data-ttu-id="ac78e-124">Код</span><span class="sxs-lookup"><span data-stu-id="ac78e-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="comments"></a><span data-ttu-id="ac78e-125">Комментарии</span><span class="sxs-lookup"><span data-stu-id="ac78e-125">Comments</span></span>

<span data-ttu-id="ac78e-126">Идентификаторы контента, папки и элемента MIME были сокращены для сохранения удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="ac78e-126">The MIME content, folder, and item identifiers have been shortened to preserve readability.</span></span>
  
### <a name="successful-response-elements"></a><span data-ttu-id="ac78e-127">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="ac78e-127">Successful response elements</span></span>

<span data-ttu-id="ac78e-128">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac78e-128">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ac78e-129">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ac78e-129">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ac78e-130">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="ac78e-130">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="ac78e-131">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ac78e-131">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ac78e-132">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ac78e-132">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="ac78e-133">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ac78e-133">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ac78e-134">Items</span><span class="sxs-lookup"><span data-stu-id="ac78e-134">Items</span></span>](items.md)
    
- [<span data-ttu-id="ac78e-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="ac78e-135">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="ac78e-136">Сохранитьmimecontent</span><span class="sxs-lookup"><span data-stu-id="ac78e-136">MimeContent</span></span>](mimecontent.md)
    
- [<span data-ttu-id="ac78e-137">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="ac78e-137">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="ac78e-138">Тема</span><span class="sxs-lookup"><span data-stu-id="ac78e-138">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="ac78e-139">Sensitivity</span><span class="sxs-lookup"><span data-stu-id="ac78e-139">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="ac78e-140">Body</span><span class="sxs-lookup"><span data-stu-id="ac78e-140">Body</span></span>](body.md)
    
- [<span data-ttu-id="ac78e-141">Размер</span><span class="sxs-lookup"><span data-stu-id="ac78e-141">Size</span></span>](size.md)
    
- [<span data-ttu-id="ac78e-142">датетимесент</span><span class="sxs-lookup"><span data-stu-id="ac78e-142">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="ac78e-143">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="ac78e-143">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="ac78e-144">респонсеобжектс</span><span class="sxs-lookup"><span data-stu-id="ac78e-144">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="ac78e-145">реплитоитем</span><span class="sxs-lookup"><span data-stu-id="ac78e-145">ReplyToItem</span></span>](replytoitem.md)
    
- [<span data-ttu-id="ac78e-146">репляллтоитем</span><span class="sxs-lookup"><span data-stu-id="ac78e-146">ReplyAllToItem</span></span>](replyalltoitem.md)
    
- [<span data-ttu-id="ac78e-147">форвардитем</span><span class="sxs-lookup"><span data-stu-id="ac78e-147">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="ac78e-148">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ac78e-148">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="ac78e-149">ToRecipients</span><span class="sxs-lookup"><span data-stu-id="ac78e-149">ToRecipients</span></span>](torecipients.md)
    
- [<span data-ttu-id="ac78e-150">Mailbox</span><span class="sxs-lookup"><span data-stu-id="ac78e-150">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="ac78e-151">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ac78e-151">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="ac78e-152">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="ac78e-152">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="ac78e-153">Раутингтипе (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ac78e-153">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="ac78e-154">исреадрецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="ac78e-154">IsReadReceiptRequested</span></span>](isreadreceiptrequested.md)
    
- [<span data-ttu-id="ac78e-155">исделиверирецеиптрекуестед</span><span class="sxs-lookup"><span data-stu-id="ac78e-155">IsDeliveryReceiptRequested</span></span>](isdeliveryreceiptrequested.md)
    
- [<span data-ttu-id="ac78e-156">From</span><span class="sxs-lookup"><span data-stu-id="ac78e-156">From</span></span>](from.md)
    
- [<span data-ttu-id="ac78e-157">IsRead</span><span class="sxs-lookup"><span data-stu-id="ac78e-157">IsRead</span></span>](isread.md)
    
## <a name="getitem-e-mail-message-error-response-example"></a><span data-ttu-id="ac78e-158">Пример отклика "GetItem (сообщение электронной почты)"</span><span class="sxs-lookup"><span data-stu-id="ac78e-158">GetItem (E-mail Message) Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ac78e-159">Description</span><span class="sxs-lookup"><span data-stu-id="ac78e-159">Description</span></span>

<span data-ttu-id="ac78e-160">В следующем примере показан ответ об ошибке для запроса GetItem.</span><span class="sxs-lookup"><span data-stu-id="ac78e-160">The following example shows an error response to a GetItem request.</span></span> <span data-ttu-id="ac78e-161">Ошибка вызвана попыткой получения недопустимого дополнительного свойства.</span><span class="sxs-lookup"><span data-stu-id="ac78e-161">The error was caused by an attempt to get an invalid additional property.</span></span>
  
### <a name="code"></a><span data-ttu-id="ac78e-162">Код</span><span class="sxs-lookup"><span data-stu-id="ac78e-162">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="error-response-elements"></a><span data-ttu-id="ac78e-163">Элементы ошибочного ответа</span><span class="sxs-lookup"><span data-stu-id="ac78e-163">Error response elements</span></span>

<span data-ttu-id="ac78e-164">В ответе на сообщение об ошибке используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ac78e-164">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="ac78e-165">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ac78e-165">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ac78e-166">жетитемреспонсе</span><span class="sxs-lookup"><span data-stu-id="ac78e-166">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="ac78e-167">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="ac78e-167">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="ac78e-168">жетитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="ac78e-168">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="ac78e-169">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ac78e-169">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ac78e-170">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ac78e-170">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ac78e-171">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ac78e-171">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="ac78e-172">мессажексмл</span><span class="sxs-lookup"><span data-stu-id="ac78e-172">MessageXml</span></span>](messagexml.md)
    
- [<span data-ttu-id="ac78e-173">фиелдури</span><span class="sxs-lookup"><span data-stu-id="ac78e-173">FieldURI</span></span>](fielduri.md)
    
## <a name="see-also"></a><span data-ttu-id="ac78e-174">См. также</span><span class="sxs-lookup"><span data-stu-id="ac78e-174">See also</span></span>



[<span data-ttu-id="ac78e-175">Операция GetItem</span><span class="sxs-lookup"><span data-stu-id="ac78e-175">GetItem operation</span></span>](getitem-operation.md)

