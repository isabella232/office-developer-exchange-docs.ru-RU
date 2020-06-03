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
# <a name="updateitem-operation-contact"></a>Операция UpdateItem (Contact)

Операция UpdateItem используется для обновления свойств элемента контакта в хранилище Exchange.
  
## <a name="updateitem-contact-request-example"></a>Пример запроса UpdateItem (Contact)

### <a name="description"></a>Description

В приведенном ниже примере кода показано, как обновить адрес электронной почты контакта.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [итемчанжес](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [сетитемфиелд](setitemfield.md)
    
- [индекседфиелдури](indexedfielduri.md)
    
- [контакт](contact.md);
    
- [EmailAddresses](emailaddresses.md)
    
- [Запись (EmailAddress)](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a>Успешный ответ UpdateItem (контакт)

### <a name="description"></a>Description

В следующем примере кода показан успешный ответ UpdateItem.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [упдатеитемреспонсе](updateitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [упдатеитемреспонсемессаже](updateitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [контакт](contact.md);
    
- [Идентификатор](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a>Недопустимый пример запроса UpdateItem (Contact)

### <a name="description"></a>Description

В следующем примере кода показан недопустимый запрос.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.
  
## <a name="updateitem-contact-error-response"></a>Ответ на сообщение об ошибке UpdateItem (Contact)

### <a name="description"></a>Description

В следующем примере кода показан ответ об ошибке для запроса UpdateItem (Contact).
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Комментарии

Некоторые элементы, используемые в теле SOAP ошибочного ответа, вызванного ошибкой проверки схемы, не определены в схемах messages или Types. Элемент **detail** содержит сведения об ошибке. Элемент [респонсекоде](responsecode.md) содержит код ошибки. Элемент [Message](message-ex15websvcsotherref.md) содержит объяснение ошибки, если она доступна. Элемент **line** описывает номер строки, в которой произошла ошибка проверки схемы. Элемент **position** описывает позицию из самого левого знака XML-документа. 
  
## <a name="see-also"></a>См. также



[Операция UpdateItem](updateitem-operation.md)

