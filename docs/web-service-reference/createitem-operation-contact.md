---
title: Операция CreateItem (Contact)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateItem
api_type:
- schema
ms.assetid: 417e994b-0a17-4c24-9527-04796b80b029
description: Операция CreateItem используется для создания контактов в хранилище Exchange.
ms.openlocfilehash: e1d78392b94d328cf687655cd93e6c9568f6274f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457125"
---
# <a name="createitem-operation-contact"></a>Операция CreateItem (Contact)

Операция CreateItem используется для создания контактов в хранилище Exchange.
  
## <a name="remarks"></a>Примечания

Создание частных списков рассылки не поддерживается. Все свойства в контейнере [комплетенаме](completename.md) доступны только для чтения и не могут быть заданы для элемента контакта. 
  
## <a name="createitem-request-example"></a>Пример запроса CreateItem

### <a name="description"></a>Description

В приведенном ниже примере допустимого запроса в виде CreateItem SOAP показано, как создать контакт в папке "Контакты" по умолчанию.
  
### <a name="code"></a>Код

```XML
<soap:Envelope
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
 xmlns:xsd="http://www.w3.org/2001/XMLSchema"
 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
 xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" >
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts"/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:FileAs>SampleContact</t:FileAs>
          <t:GivenName>Tanja</t:GivenName>
          <t:CompanyName>Blue Yonder Airlines</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">tplate@example.com</t:Entry>
          </t:EmailAddresses>
          <t:PhysicalAddresses>
            <t:Entry Key="Business">
              <t:Street>1234 56th Ave</t:Street>
              <t:City>La Habra</t:City>
              <t:State>CA</t:State>
              <t: CountryOrRegion>USA</t: CountryOrRegion>
            </t:Entry>
          </t:PhysicalAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">4255550199</t:Entry>
          </t:PhoneNumbers>
          <t:JobTitle>Manager</t:JobTitle>
          <t:Surname>Plate</t:Surname>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a>Элементы Request

В отклике используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [саведитемфолдерид](saveditemfolderid.md)
    
- [дистингуишедфолдерид](distinguishedfolderid.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [контакт](contact.md);
    
- [FileAs](fileas.md)
    
- [GivenName](givenname.md)
    
- [CompanyName](companyname.md)
    
- [EmailAddresses](emailaddresses.md)
    
- [Запись (EmailAddress)](entry-emailaddress.md)
    
- [фисикаладдрессес](physicaladdresses.md)
    
- [Запись (PhysicalAddress)](entry-physicaladdress.md)
    
- [Назван](street.md)
    
- [City](city.md)
    
- [State](state-ex15websvcsotherref.md)
    
- [CountryOrRegion](countryorregion.md)
    
- [PhoneNumbers](phonenumbers.md)
    
- [Запись (PhoneNumber)](entry-phonenumber.md)
    
- [JobTitle](jobtitle.md)
    
- [ФИО](surname.md)
    
## <a name="successful-createitem-request"></a>Успешный запрос CreateItem

### <a name="description"></a>Description

В следующем примере показан успешный ответ на запрос CreateItem, который создал контакт. В этом примере ответ содержит идентификатор только что созданного элемента.
  
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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Contact>
              <t:ItemId Id="AAAtA=" ChangeKey="EQAAAB" />
            </t:Contact>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеитемреспонсе](createitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеитемреспонсемессаже](createitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [контакт](contact.md);
    
- [Идентификатор](itemid.md)
    
## <a name="invalid-createitem-request-example"></a>Недопустимый пример запроса CreateItem

### <a name="description"></a>Description

В следующем примере показан запрос, который содержит допустимый XML, но несовместимые инструкции. Невозможно создать контакт в папке поиска.
  
### <a name="code"></a>Код

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns='https://schemas.microsoft.com/exchange/services/2006/messages'>
      <SavedItemFolderId>
        <t:DistinguishedFolderId Id='searchfolders'/>
      </SavedItemFolderId>
      <Items>
        <t:Contact>
          <t:ItemClass>IPM.Contact</t:ItemClass>
        </t:Contact>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="createitem-contact-error-response"></a>Запрос ошибки CreateItem (Contact)

### <a name="description"></a>Description

В приведенном ниже примере показан ответ об ошибке для запроса CreateItem (Contact).
  
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
    <CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>Cannot create a contact in a non-contact Folder.</m:MessageText>
          <m:ResponseCode>ErrorCannotCreateContactInNonContactFolder</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеитемреспонсе](createitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеитемреспонсемессаже](createitemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
## <a name="see-also"></a>См. также



[Операция CreateItem](createitem-operation.md)

