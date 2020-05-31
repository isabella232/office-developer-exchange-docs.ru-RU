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
description: Операция GetAttachment используется для получения существующих вложений на элементы в хранилище Exchange.
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762701"
---
# <a name="getattachment-operation"></a>Операция GetAttachment

Операция GetAttachment используется для получения существующих вложений на элементы в хранилище Exchange.
  
## <a name="getattachment-request-example"></a>Пример запроса GetAttachment

### <a name="description"></a>Описание

В приведенном ниже примере запроса GetAttachment показано, как получить вложение.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

Элемент [аттачментшапе](attachmentshape.md) позволяет указать, какие сведения о вложении должны быть возвращены. Пустой элемент [аттачментшапе](attachmentshape.md) является допустимым и будет отображать вложения без содержимого MIME для вложений элементов, тип текста текста и без дополнительных свойств. 
  
Коллекция [аттачментидс](attachmentids.md) позволяет указать один или несколько идентификаторов вложений, которые необходимо вернуть. Обратите внимание, что они относятся к типу Рекуестаттачментидтипе, поэтому для всех Аттачментидс, получаемых из **CreateAttachment** , необходимо удалить атрибуты **рутитемид** и **рутитемчанжекэй** , прежде чем передавать их в метод **GetAttachment**.
  
> [!NOTE]
> Идентификатор и ключ вложения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [GetAttachment](getattachment.md)
    
- [аттачментшапе](attachmentshape.md)
    
- [аттачментидс](attachmentids.md)
    
- [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>Пример отклика GetAttachment

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос GetAttachment. В этом примере возвращается вложенный файл.
  
### <a name="code"></a>Код

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

### <a name="comments"></a>Comments

В ответных сообщениях для GetAttachment всегда будет содержаться полное вложение; то есть все свойства всегда будут включены. Для вложений файлов эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), идентификатором [ContentId](contentid.md), [ContentLocation](contentlocation.md)и [содержимым](content.md). Для вложений элемента эти свойства являются [именами (AttachmentType)](name-attachmenttype.md), [ContentType](contenttype.md), [ContentId](contentid.md), [ContentLocation](contentlocation.md) и всеми свойствами элемента, как если бы фигура **аллпропертиес** была использована при вызове GetItem. Элемент [аттачментшапе](attachmentshape.md) , если он присутствует, позволяет приложению-потребителю запрашивать дополнительные расширенные свойства для вложений элементов. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [жетаттачментреспонсе](getattachmentresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [жетаттачментреспонсемессаже](getattachmentresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment и DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Имя (AttachmentType)](name-attachmenttype.md)
    
- [Статья](content.md)
    
## <a name="see-also"></a>См. также



[Операция CreateAttachment](createattachment-operation.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)

