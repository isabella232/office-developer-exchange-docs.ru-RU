---
title: Операция SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: Операция SendItem используется для отправки сообщений электронной почты, расположенных в Exchange магазине.
ms.openlocfilehash: d1e43cdceb3a594c3fa2f028502a3bfedbbf85a1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521587"
---
# <a name="senditem-operation"></a>Операция SendItem

Операция SendItem используется для отправки сообщений электронной почты, расположенных в Exchange магазине.
  
## <a name="senditem-e-mail-message-request-example"></a>Пример запроса SendItem (сообщение электронной почты)

### <a name="description"></a>Описание

В следующем примере показано, как отправлять сообщение электронной почты.
  
### <a name="code"></a>Код

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор элемента был сокращен для сохранения читаемости.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [SendItem](senditem.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a>Успешный ответ sendItem (сообщение электронной почты)

### <a name="description"></a>Описание

В следующем примере показан успешный ответ SendItem.
  
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
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
### <a name="comments"></a>Комментарии

Делегат, который пытается отправить сообщение электронной почты, расположенное в папке "Черновики" директора с набором параметра SendAndSaveCopy для сохранения копии в отличительной папке "Отправленные элементы", не сможет переместить копию отправленного элемента в папку "Отправленные элементы". Элемент останется в папке Черновики директора. Решение этой проблемы — указать почтовый ящик директора в [элементе DistinguishedFolderId.](distinguishedfolderid.md) 
  
Следует рассмотреть дополнительный сценарий, когда делегат создает сообщение электронной почты и сохраняет его в папке Черновики почтового ящика делегата. Если делегат пытается отправить элемент и сохранить копию в отличительной папке "Отправленные элементы" директора, сообщение отправляется правильно, черновик сообщения остается в папке "Черновики" делегата, отправленное сообщение не появляется ни в папке отправленных элементов делегата, ни в папке "Отправленные элементы" директора, и ответ будет успешным.
  
## <a name="invalid-senditem-e-mail-message-request-example"></a>Пример запроса на недействительный sendItem (сообщение электронной почты)

### <a name="description"></a>Описание

В следующем примере кода показан пример запроса с недопустимым идентификатором.
  
### <a name="code"></a>Код

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a>Ответ на ошибку SendItem (сообщение электронной почты)

### <a name="description"></a>Описание

В следующем примере показан ответ на ошибку на запрос SendItem, содержащий недопустимый идентификатор.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ответа на ошибки

В ответе на ошибку используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция SendItem](senditem-operation.md)
  
 **SendItemType**


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

