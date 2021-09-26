---
title: Операция DeleteAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в Exchange магазине.
ms.openlocfilehash: bd08776e1f4e75204819ef5463e297e3770a34a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546688"
---
# <a name="deleteattachment-operation"></a>Операция DeleteAttachment

Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в Exchange магазине.
  
## <a name="remarks"></a>Заметки

Эта операция позволяет удалить одно или несколько вложений по ID.
  
## <a name="deleteattachment-request-example"></a>Пример запроса deleteAttachment

### <a name="description"></a>Описание

В следующем примере запроса DeleteAttachment показано, как удалить вложение элемента.
  
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

Идентификатор вложения был сокращен для сохранения читаемости.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>Пример ответа DeleteAttachment

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

Операция CreateAttachment возвращает элемент типа AttachmentIdType, который включает **RootItemId** и **RootItemChangeKey.** Эти атрибуты не разрешены для идентификаторов в запросе DeleteAttachment. DeleteAttachment использует элементы типа RequestAttachmentIdType, которые не включают эти атрибуты.
  
Ответ DeleteAttachment включает в себя ID родительского элемента. При удалении вложений из элемента меняется ключ изменения элемента. Ключ изменения элемента можно получить в ответе DeleteAttachment.
  
> [!NOTE]
> Идентификатор [RootItemId](rootitemid.md) и ChangeKey были сокращены для сохранения читаемости. 
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В ответе используются следующие элементы:
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteAttachmentResponse](deleteattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootItemId](rootitemid.md)
    
## <a name="see-also"></a>См. также

- [Операция CreateAttachment](createattachment-operation.md) 
- [Операция GetAttachment](getattachment-operation.md)

