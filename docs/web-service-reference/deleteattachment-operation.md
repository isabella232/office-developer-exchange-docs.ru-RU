---
title: Операция DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: Операция DeleteAttachment используется для удаления вложенных файлов и вложений элементов из существующего элемента в хранилище Exchange.
ms.openlocfilehash: 1d34ce4c5ba1d955989a35dafb8ab3c5d229d505
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457335"
---
# <a name="deleteattachment-operation"></a>Операция DeleteAttachment

Операция DeleteAttachment используется для удаления вложенных файлов и вложений элементов из существующего элемента в хранилище Exchange.
  
## <a name="remarks"></a>Примечания

Эта операция позволяет удалить одно или несколько вложений по ИДЕНТИФИКАТОРу.
  
## <a name="deleteattachment-request-example"></a>Пример запроса DeleteAttachment

### <a name="description"></a>Описание

В приведенном ниже примере запроса DeleteAttachment показано, как удалить вложение элемента.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор вложения был сокращен, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [DeleteAttachment](deleteattachment.md)
    
- [аттачментидс](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>Пример отклика DeleteAttachment

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос DeleteAttachment.
  
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
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Операция CreateAttachment Возвращает элемент типа Аттачментидтипе, включающий в себя **рутитемид** и **рутитемчанжекэй**. Эти атрибуты не разрешены для идентификаторов в запросе DeleteAttachment. DeleteAttachment использует элементы типа Рекуестаттачментидтипе, которые не включают эти атрибуты.
  
Ответ DeleteAttachment включает идентификатор родительского элемента. При удалении вложений из элемента изменяется ключ изменения элемента. Новый ключ изменения элемента можно получить из отклика DeleteAttachment.
  
> [!NOTE]
> Идентификатор [рутитемид](rootitemid.md) и чанжекэй были сокращены для сохранения удобочитаемости. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [делетеаттачментреспонсе](deleteattachmentresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [делетеаттачментреспонсемессаже](deleteattachmentresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [рутитемид](rootitemid.md)
    
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md) 
- [Операция GetAttachment](getattachment-operation.md)

