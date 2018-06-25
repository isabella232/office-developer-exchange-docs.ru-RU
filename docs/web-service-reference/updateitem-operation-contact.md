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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840348"
---
# <a name="updateitem-operation-contact"></a>Операция UpdateItem (контактов)

Операция UpdateItem используется для обновления свойств элемента контакта в хранилище Exchange.
  
## <a name="updateitem-contact-request-example"></a>Пример запроса UpdateItem (контактов)

### <a name="description"></a>Описание

В следующем примере кода показано, как обновить контактный адрес электронной почты.
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [UpdateItem](updateitem.md)
    
- [ItemChanges](itemchanges.md)
    
- [ItemChange](itemchange.md)
    
- [Идентификатор элемента](itemid.md)
    
- [Обновления (элемент)](updates-item.md)
    
- [SetItemField](setitemfield.md)
    
- [IndexedFieldURI](indexedfielduri.md)
    
- [Контакт](contact.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Запись (EmailAddress)](entry-emailaddress.md)
    
## <a name="successful-updateitem-contact-response"></a>Успешные UpdateItem (контакт) ответа

### <a name="description"></a>Описание

В следующем примере кода показано успешного ответа UpdateItem.
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UpdateItemResponse](updateitemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UpdateItemResponseMessage](updateitemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md)
    
- [Контакт](contact.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="invalid-updateitem-contact-request-example"></a>Пример запроса недопустимый UpdateItem (контактов)

### <a name="description"></a>Описание

В следующем примере кода показано недопустимый запрос.
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

Идентификатор элемента был усечен, чтобы сохранить удобочитаемость.
  
## <a name="updateitem-contact-error-response"></a>Отклик UpdateItem (контактов)

### <a name="description"></a>Описание

В следующем примере кода показано ошибочный ответ на запрос UpdateItem (контактов).
  
### <a name="code"></a>Программа

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

### <a name="comments"></a>Комментарии

Некоторые элементы, которые используются в тексте SOAP возврату ошибки, возникающие при ошибке проверки схемы не определены в схемах типов или сообщений. Элемент **детализации** содержит сведения об ошибке. Элемент [ResponseCode](responsecode.md) содержит код ошибки. Элемент [сообщение](message-ex15websvcsotherref.md) содержит описание ошибки, если она доступна. Элемент **строки** описываются номер строки, где произошла ошибка проверки схемы. Элемент **позиции** описывает положение из первого символа XML-документа. 
  
## <a name="see-also"></a>См. также



[UpdateItem Operation](updateitem-operation.md)

