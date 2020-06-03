---
title: Операция SendItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: Операция SendItem используется для отправки сообщений электронной почты, размещенных в хранилище Exchange.
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530340"
---
# <a name="senditem-operation"></a>Операция SendItem

Операция SendItem используется для отправки сообщений электронной почты, размещенных в хранилище Exchange.
  
## <a name="senditem-e-mail-message-request-example"></a>Пример запроса SendItem (сообщение электронной почты)

### <a name="description"></a>Description

В приведенном ниже примере показано, как отправить сообщение электронной почты.
  
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

Идентификатор элемента был сокращен, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [SendItem](senditem.md)
    
- [итемидс](itemids.md)
    
- [Идентификатор](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a>Успешный ответ SendItem (сообщение электронной почты)

### <a name="description"></a>Description

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

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [сендитемреспонсе](senditemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [сендитемреспонсемессаже](senditemresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
### <a name="comments"></a>Комментарии

Представитель, пытающийся отправить сообщение электронной почты, размещенное в папке "Черновики" основного приложения с параметром SendAndSaveCopy, чтобы сохранить копию в папке "Отправленные", не будет автоматически перемещать копию отправленного элемента в папку "Отправленные". Элемент останется в папке "Черновики" основного приложения. Чтобы устранить эту ошибку, необходимо указать почтовый ящик участника в элементе [дистингуишедфолдерид](distinguishedfolderid.md) . 
  
Если делегат создает сообщение электронной почты и сохраняет его в папке "Черновики" почтового ящика представителя, необходимо учитывать дополнительный сценарий. Если делегат пытается отправить элемент и сохранить копию в различающейся папке "Отправленные" участника, сообщение отправляется правильно, черновик остается в папке "Черновики" делегата, а отправленное сообщение не будет отображаться в папке "Отправленные" представителя или субъекта "Отправленные", а ответ является успешным.
  
## <a name="invalid-senditem-e-mail-message-request-example"></a>Недопустимый пример запроса SendItem (сообщение электронной почты)

### <a name="description"></a>Description

В приведенном ниже примере кода показан пример запроса с недопустимым идентификатором.
  
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

## <a name="senditem-e-mail-message-error-response"></a>Сообщение об ошибке SendItem (сообщение электронной почты)

### <a name="description"></a>Description

В следующем примере показан ответ об ошибке для запроса SendItem, который содержит недопустимый идентификатор.
  
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

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [сендитемреспонсе](senditemresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [сендитемреспонсемессаже](senditemresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
## <a name="see-also"></a>См. также



[Операция SendItem](senditem-operation.md)
  
 **сендитемтипе**


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

