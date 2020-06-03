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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459996"
---
# <a name="getitem-operation-email-message"></a>Операция GetItem (сообщение электронной почты)

Операция GetItem позволяет пользователю получать доступ к сведениям о сообщениях электронной почты.
  
## <a name="using-the-getitem-operation-for-messages"></a>Использование операции GetItem для сообщений

Запрос GetItem должен иметь следующие сведения:
  
- Элемент [ItemId](itemid.md) для определения возвращаемых сведений об элементе. 
    
- Элемент [итемшапе](itemshape.md) для определения возвращаемых свойств элемента. 
    
## <a name="getitem-request-example"></a>Пример запроса GetItem

### <a name="description"></a>Description

В приведенном ниже примере запроса GetItem показано, как получить доступ к сведениям о сообщениях электронной почты.
  
### <a name="code"></a>Код

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

### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [GetItem](getitem.md)
    
- [итемшапе](itemshape.md)
    
- [басешапе](baseshape.md)
    
- [инклудемимеконтент](includemimecontent.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="successful-getitem-e-mail-message-response-example"></a>Пример ответа на сообщение об успешном выполнении операции GetItem (сообщение электронной почты)

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос GetItem.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

Идентификаторы контента, папки и элемента MIME были сокращены для сохранения удобочитаемости.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетитемреспонсе](getitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [жетитемреспонсемессаже](getitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
- [Сообщение](message-ex15websvcsotherref.md)
    
- [Сохранитьmimecontent](mimecontent.md)
    
- [Идентификатор](itemid.md)
    
- [Тема](subject.md)
    
- [Sensitivity](sensitivity.md)
    
- [Body](body.md)
    
- [Размер](size.md)
    
- [датетимесент](datetimesent.md)
    
- [DateTimeCreated](datetimecreated.md)
    
- [респонсеобжектс](responseobjects.md)
    
- [реплитоитем](replytoitem.md)
    
- [репляллтоитем](replyalltoitem.md)
    
- [форвардитем](forwarditem.md)
    
- [HasAttachments](hasattachments.md)
    
- [ToRecipients](torecipients.md)
    
- [Mailbox](mailbox.md)
    
- [Имя (EmailAddressType)](name-emailaddresstype.md)
    
- [EmailAddress (Нонемптистрингтипе)](emailaddress-nonemptystringtype.md)
    
- [Раутингтипе (EmailAddressType)](routingtype-emailaddresstype.md)
    
- [исреадрецеиптрекуестед](isreadreceiptrequested.md)
    
- [исделиверирецеиптрекуестед](isdeliveryreceiptrequested.md)
    
- [From](from.md)
    
- [IsRead](isread.md)
    
## <a name="getitem-e-mail-message-error-response-example"></a>Пример отклика "GetItem (сообщение электронной почты)"

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса GetItem. Ошибка вызвана попыткой получения недопустимого дополнительного свойства.
  
### <a name="code"></a>Код

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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетитемреспонсе](getitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [жетитемреспонсемессаже](getitemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [мессажексмл](messagexml.md)
    
- [фиелдури](fielduri.md)
    
## <a name="see-also"></a>См. также



[Операция GetItem](getitem-operation.md)

