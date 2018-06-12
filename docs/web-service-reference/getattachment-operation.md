---
title: Операция GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: Операция GetAttachment используется для извлечения существующие вложения для элементов в хранилище Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762701"
---
# <a name="getattachment-operation"></a>Операция GetAttachment

Операция GetAttachment используется для извлечения существующие вложения для элементов в хранилище Exchange.
  
## <a name="getattachment-request-example"></a>Пример запроса GetAttachment

### <a name="description"></a>Описание

В следующем примере запрос на GetAttachment показано, как для получения вложения.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Элемент [AttachmentShape](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены. Пустой элемент [AttachmentShape](attachmentshape.md) является допустимым и будут отображаться вложения без содержимого MIME для вложений элемента с типом body текст и без любые дополнительные свойства. 
  
Коллекция [AttachmentIds](attachmentids.md) позволяет указать один или несколько идентификаторов вложений для возврата. Обратите внимание, что это RequestAttachmentIdType, поэтому любые AttachmentIds, полученные из **CreateAttachment** должно иметь атрибуты **RootItemId** и **RootItemChangeKey** удалены перед передачей их в **GetAttachment**типа.
  
> [!NOTE]
> Идентификатор вложения и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Пример ответа GetAttachment

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос GetAttachment. В этом примере возвращается вложенный файл.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Ответное сообщение на GetAttachment всегда будет содержать полный вложений; то есть все свойства всегда будут включены. Для файлов вложений эти свойства — это [имя (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md)и [контента](content.md). Для вложений элемента, эти свойства — это [имя (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) и все свойства элемента, как если бы было использовано фигуры **AllProperties** GetItem звонка. Элемент [AttachmentShape](attachmentshape.md) , если этот параметр указан, позволяет клиентского приложения запросить дополнительные расширенные свойства для вложений элемента. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Имя (AttachmentType)](name-attachmenttype.md)
    
- [Контентная](content.md)
    
## <a name="see-also"></a>См. также



[Операция CreateAttachment](createattachment-operation.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)

