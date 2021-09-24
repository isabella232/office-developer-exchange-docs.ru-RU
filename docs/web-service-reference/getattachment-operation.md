---
title: Операция GetAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: Операция GetAttachment используется для получения существующих вложений для элементов в Exchange магазине.
ms.openlocfilehash: 44a9e1988deb513039f7700e11c645c366641519
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509939"
---
# <a name="getattachment-operation"></a>Операция GetAttachment

Операция GetAttachment используется для получения существующих вложений для элементов в Exchange магазине.
  
## <a name="getattachment-request-example"></a>Пример запроса GetAttachment

### <a name="description"></a>Описание

В следующем примере запроса GetAttachment показано, как получить вложение.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Элемент [AttachmentShape](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены. Пустой [элемент AttachmentShape](attachmentshape.md) действителен и будет отрисовка вложений без содержимого MIME для вложений элементов, с типом текстового тела и без дополнительных свойств. 
  
Коллекция [AttachmentIds](attachmentids.md) позволяет указать один или несколько идентификаторов вложений для возврата. Обратите внимание, что они имеют тип RequestAttachmentIdType, поэтому все вложения, которые вы получаете от **CreateAttachment,** должны иметь атрибуты **RootItemId** и **RootItemChangeKey,** удалены перед передачей их **в GetAttachment**.
  
> [!NOTE]
> Идентификатор вложения и ключ изменения были сокращены для сохранения читаемости. 
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Пример ответа GetAttachment

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос GetAttachment. В этом примере возвращается вложение файла.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

Сообщения ответа для GetAttachment всегда будут содержать полное вложение; то есть все свойства всегда будут включены. Для вложений файлов эти [свойства: Name (AttachmentType),](name-attachmenttype.md) [ContentType,](contenttype.md) [ContentId,](contentid.md) [ContentLocation](contentlocation.md)и [Content](content.md). Для вложений элементов эти свойства: [Name (AttachmentType),](name-attachmenttype.md) [ContentType,](contenttype.md) [ContentId,](contentid.md) [ContentLocation](contentlocation.md) и все свойства элемента, как если бы форма **AllProperties** была использована в вызове GetItem. Элемент [AttachmentShape,](attachmentshape.md) если он присутствует, позволит приложению-потребителю запрашивать дополнительные расширенные свойства для вложений элементов. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Name (AttachmentType)](name-attachmenttype.md)
    
- [Статья](content.md)
    
## <a name="see-also"></a>См. также



[Операция CreateAttachment](createattachment-operation.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)

