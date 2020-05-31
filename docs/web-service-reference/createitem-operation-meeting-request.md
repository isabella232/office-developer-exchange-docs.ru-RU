---
title: Операция CreateItem (приглашение на собрание)
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
ms.assetid: fe136881-a804-456a-8552-8a1bea5eb9c8
description: Операция CreateItem используется для ответа на приглашения на собрания.
ms.openlocfilehash: a8aea688e46376906554952ce8ec45022cf613e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761895"
---
# <a name="createitem-operation-meeting-request"></a>Операция CreateItem (приглашение на собрание)

Операция CreateItem используется для ответа на приглашения на собрания.
  
## <a name="remarks"></a>Примечания

Операция CreateItem предоставляет три варианта ответа на приглашение на собрание: принять, под вопросом или отклонить. 
  
## <a name="accept-meeting-request-example"></a>Пример принятия приглашения на собрание

### <a name="description"></a>Описание

В приведенном ниже примере показано, как принять приглашение на собрание.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                MessageDisposition="SendAndSaveCopy">
      <Items>
        <AcceptItem xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ReferenceItemId Id="AAAlAFVzZ"
                           ChangeKey="CwAAABYAA"/>
        </AcceptItem>
      </Items>
    </CreateItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Comments

Чтобы принять или отклонить приглашение на собрание, используйте элементы [тентативелякцептитем](tentativelyacceptitem.md) или [Деклинеитем](declineitem.md) вместо элемента [акцептитем](acceptitem.md) . 
  
Идентификатор элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость.
  
### <a name="accepting-meeting-request-elements"></a>Принятие элементов приглашения на собрание

В запросе используются следующие элементы:
  
- [CreateItem](createitem.md)
    
- [Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md)
    
- [акцептитем](acceptitem.md)
    
- [референцеитемид](referenceitemid.md)
    
## <a name="successful-accept-meeting-response-example"></a>Пример успешного принятия ответа на приглашение на собрание

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateItem.
  
### <a name="code"></a>Код

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items />
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </CreateItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеитемреспонсе](createitemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеитемреспонсемессаже](createitemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Items](items.md)
    
## <a name="accept-meeting-error-response-example"></a>Пример принятия ответа на сообщение об ошибке собрания

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса CreateItem. Ошибка вызвана попыткой принять приглашение на собрание, которое не удается найти в хранилище Exchange.
  
### <a name="code"></a>Код

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
    <CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                        xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
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
    
- [Items](items.md)
    
## <a name="see-also"></a>См. также



[Операция CreateItem](createitem-operation.md)
  
[Операция CreateItem (элемент календаря)](createitem-operation-calendar-item.md)

