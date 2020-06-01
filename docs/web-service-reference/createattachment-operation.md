---
title: Операция CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: Операция CreateAttachment создает элемент или вложенный файл и прикрепляет его к указанному элементу.
ms.openlocfilehash: 8028c56aa306774b54b39e5ee1ac0382b9113fa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456572"
---
# <a name="createattachment-operation"></a>Операция CreateAttachment

Операция CreateAttachment создает элемент или вложенный файл и прикрепляет его к указанному элементу.
  
## <a name="file-createattachment-request-example"></a>Пример запроса файла CreateAttachment

### <a name="description"></a>Описание

В приведенном ниже примере запроса CreateAttachment показано, как создать вложенный файл.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

Необходимо указать имя вложения.
  
> [!NOTE]
> Идентификатор родительского элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateAttachment](createattachment.md)
    
- [парентитемид](parentitemid.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [Имя (AttachmentType)](name-attachmenttype.md)
    
- [Content](content.md)
    
## <a name="successful-file-createattachment-response-example"></a>Пример успешного ответа файла CreateAttachment

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateAttachment.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

Ответ содержит идентификатор вложенного файла. Он также содержит идентификатор и ключ изменения корневого элемента. Для сохранения удобочитаемости идентификаторы и ключ изменения были сокращены.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеаттачментреспонсе](createattachmentresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеаттачментреспонсемессаже](createattachmentresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a>Пример запроса CreateAttachment для элемента

### <a name="description"></a>Описание

В приведенном ниже примере запроса CreateAttachment показано, как создать вложение элемента.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

Необходимо указать имя вложения.
  
 **Note (Примечание** ) Идентификатор родительского элемента и ключ изменения были сокращены, чтобы сохранить удобочитаемость. 
  
### <a name="request-elements"></a>Элементы Request

В запросе используются следующие элементы:
  
- [CreateAttachment](createattachment.md)
    
- [парентитемид](parentitemid.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [ItemAttachment](itemattachment.md)
    
- [Имя (AttachmentType)](name-attachmenttype.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [Тема](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a>Пример успешного ответа элемента CreateAttachment

### <a name="description"></a>Описание

В следующем примере показан успешный ответ на запрос CreateAttachment.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>Comment

Ответ содержит идентификатор нового вложения. Он также содержит идентификатор и ключ изменения корневого элемента. Корневым элементом является элемент, содержащий вложение. Для сохранения удобочитаемости идентификаторы и ключ изменения были сокращены.
  
### <a name="successful-response-elements"></a>Элементы успешного ответа

В отклике используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеаттачментреспонсе](createattachmentresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеаттачментреспонсемессаже](createattachmentresponsemessage.md)
    
- [респонсекоде](responsecode.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
- [ItemAttachment](itemattachment.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a>Пример ответа на сообщение об ошибке CreateAttachment

### <a name="description"></a>Описание

В следующем примере показан ответ об ошибке для запроса CreateAttachment. Ошибка вызвана тем, что имя вложения не было указано.
  
### <a name="code"></a>Код

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>Элементы ошибочного ответа

В ответе на сообщение об ошибке используются следующие элементы:
  
- [серверверсионинфо](serverversioninfo.md)
    
- [креатеаттачментреспонсе](createattachmentresponse.md)
    
- [респонсемессажес](responsemessages.md)
    
- [креатеаттачментреспонсемессаже](createattachmentresponsemessage.md)
    
- [мессажетекст](messagetext.md)
    
- [респонсекоде](responsecode.md)
    
- [дескриптивелинккэй](descriptivelinkkey.md)
    
- [мессажексмл](messagexml.md)
    
- [ексцептионфиелдури](exceptionfielduri.md)
    
- [Вложения](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a>Примечания

Если к элементу присоединяется несколько вложений в одном цикле обработки, Рутитемчанжекэй в последнем ответе — это то, которое представляет новый ключ изменения элемента, содержащего вложения.
  
## <a name="see-also"></a>См. также



[Операция DeleteAttachment](deleteattachment-operation.md)
  
[Операция GetAttachment](getattachment-operation.md)

