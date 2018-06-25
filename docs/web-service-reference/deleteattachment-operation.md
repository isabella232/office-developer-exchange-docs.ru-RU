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
description: Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в хранилище Exchange.
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762022"
---
# <a name="deleteattachment-operation"></a>Операция DeleteAttachment

Операция DeleteAttachment используется для удаления вложений файлов и элементов из существующего элемента в хранилище Exchange.
  
## <a name="remarks"></a>Замечания

Эта операция позволяет удалить один или несколько вложений по идентификатору.
  
## <a name="deleteattachment-request-example"></a>Пример запроса DeleteAttachment

### <a name="description"></a>Описание

В следующем примере запрос DeleteAttachment показано, как удалить вложение элемента.
  
### <a name="code"></a>Программа

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>Комментарии

Идентификатор вложения был усечен, чтобы сохранить удобочитаемость.
  
### <a name="request-elements"></a>Элементы запроса

В запросе используются следующие элементы:
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [Идентификатора вложения AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>Пример ответа DeleteAttachment

### <a name="description"></a>Описание

В следующем примере показано успешного ответа на запрос DeleteAttachment.
  
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
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

Операция CreateAttachment возвращает элемент AttachmentIdType типа, который включает в себя **RootItemId** и **RootItemChangeKey**. Эти атрибуты не допускаются для идентификаторов в запросе DeleteAttachment. DeleteAttachment использует элементы типа RequestAttachmentIdType, которая не включает следующие атрибуты.
  
Ответ DeleteAttachment включает в себя идентификатор родительского элемента. После удаления вложения из элемента изменяется ключ изменения элемента. Новый ключ изменения элемента можно получить из ответа DeleteAttachment.
  
> [!NOTE]
> Идентификатор [RootItemId](rootitemid.md) и ChangeKey URL были сокращены, чтобы сохранить удобочитаемость. 
  
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

