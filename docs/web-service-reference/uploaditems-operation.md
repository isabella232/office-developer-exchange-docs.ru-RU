---
title: Операция UploadItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItems
api_type:
- schema
ms.assetid: a88cbe99-7968-454d-a545-4f92c330909f
description: Операция UploadItems загружает поток элементов в почтовый ящик Exchange.
ms.openlocfilehash: 6b002d531c7011b18ae1f88adfc2923d5a51e81c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840386"
---
# <a name="uploaditems-operation"></a>Операция UploadItems

Операция **UploadItems** загружает поток элементов в почтовый ящик Exchange. 
  
> [!IMPORTANT]
> Операция **UploadItems** ограничен полезных максимальное импорта 25 МБ данных в кодировке base64 в MicrosoftExchange Server 2010 с пакетом обновления 1 (SP1). Параметр может быть изменен в файле web.config. 
  
## <a name="uploaditems-request-example"></a>Пример запроса UploadItems

### <a name="description"></a>Описание

В следующем примере запрос **UploadItems** показано, как загружать два элемента в почтовом ящике. Первый элемент — это новый элемент. Второй элемент является обновленной версией существующего элемента в почтовом ящике. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UploadItems>
      <m:Items>
        <t:Item CreateAction="CreateNew">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAA==" ChangeKey="AQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAAcSMAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAADACYAAAAAAAsAKQAAAAMALgAAAAAAAwA2AAAAAACwhw4=
          </t:Data>
        </t:Item>
        <t:Item CreateAction="Update">
          <t:ParentFolderId Id="AQMkADhhOGIgAAAB==" ChangeKey="AQAAAA=="/>
          <t:ItemId Id="AAMkADhhOGU0MGM7AAA=" ChangeKey="CQAAAA=="/>
          <t:Data>
            AQAAAAgAAAAAAAAAAQAAAAMAAAAYAAAAAQAAAAcDAgAAAAAAwAAAAA
            AAAEYAJACABAAAAAYAAAABDqSAAAACAAAANiAAAOSECEBbAAAAL089
            RklSU1QgT1JHQU5JWkFUSU9OL09VPUVYQ0hBTkdFIEFETUlOSVNUUk
            FUSVZFIEdST1VQIChGWURJQk9IRjIzU1BETFQpL0NOPVJFQ0lQSUVO
            VFMvQ049AAMAFwABAAAAsIQaABIAAABJAFAATQAuAE4AbwB0AGUAAA
            ALACMAAAALACkAAAADADYAAAAAALCENwAyAAAASQBuAHQAZQByAGUA
            cwB0AGkAbgBnACAALQAgAGYAcgBvAG0AIABFAFcAUwBNAEEAAABAAD
            kAgJ2chyHuygECATsAZQAAAEVYOi9PPUZJUlNUIE9SR0FOSVpBVBMO
          </t:Data>
        </t:Item>
      </m:Items>
    </m:UploadItems>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификаторы и данные элементов URL были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [RequestServerVersion](requestserverversion.md)
    
- [UploadItems](uploaditems.md)
    
- [Элементы (NonEmptyArrayOfUploadItemsType)](items-nonemptyarrayofuploaditemstype.md)
    
- [Элемент (UploadItemType)](item-uploaditemtype.md)
    
- [ParentFolderId](parentfolderid.md)
    
- [Данные (base64Binary)](data-base64binary.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="successful-uploaditems-response-example"></a>Пример успешного ответа UploadItems

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос **UploadItems** . 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14"
                         MinorVersion="1"
                         MajorBuildNumber="164"
                         MinorBuildNumber="0"
                         Version="Exchange2010_SP1"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhUFZ/AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQm"/>
        </m:UploadItemsResponseMessage>
        <m:UploadItemsResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:ItemId Id="AAMkADhhOGZ7AAA=" ChangeKey="CQAAABYAAABsMBS3hrihS7voMf0GPIQeAAAAULQn"/>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификаторы элементов URL-были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="response-elements"></a>Элементы ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UploadItemsResponse](uploaditemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UploadItemsResponseMessage](uploaditemsresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Идентификатор элемента](itemid.md)
    
## <a name="uploaditems-error-response-example"></a>Пример ответа об ошибке UploadItems

### <a name="description"></a>Описание

В следующем примере показано ответа на запрос **UploadItems** , который содержит ошибки, возникающие при попытке обновить элемент, который не удается найти в почтовом ящике. 
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="164" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:UploadItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:UploadItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UploadItemsResponseMessage>
      </m:ResponseMessages>
    </m:UploadItemsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа об ошибках

В ответ на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UploadItemsResponse](uploaditemsresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UploadItemsResponseMessage](uploaditemsresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция ExportItems](exportitems-operation.md)


[Операции EWS в Exchange](ews-operations-in-exchange.md)
  
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

