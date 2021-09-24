---
title: CreateAttachment
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e33b403a-b7d3-48ee-8d24-6b7abf0d70bc
description: Элемент CreateAttachment определяет запрос на создание вложения к элементу в Exchange магазине.
ms.openlocfilehash: 6716a83b0d1ba9d7f39351da60f7009df04a3fa0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515875"
---
# <a name="createattachment"></a>CreateAttachment

Элемент **CreateAttachment** определяет запрос на создание вложения к элементу в Exchange магазине. 
  
```xml
<CreateAttachment>
   <ParentItemId/>
   <Attachments/>
</CreateAttachment>
```

 **CreateAttachmentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ParentItemId](parentitemid.md) <br/> |Определяет элемент родительского Exchange, содержащий созданное вложение. Элемент [ParentItemId](parentitemid.md) должен предоставить ID элемента Exchange магазина. Элементы реального магазина можно получить с помощью [операции GetItem;](getitem-operation.md) Вложения извлекаются с помощью [операции GetAttachment.](getattachment-operation.md) Ошибка возникает, если [parentItemId](parentitemid.md) передается ID вложения файла. Если [ParentItemId](parentitemid.md) представляет ID существующего вложения элемента, операция [CreateAttachment](createattachment-operation.md) добавляет новое вложение в существующее вложение.  <br/> Этот элемент необходим для операции [CreateAttachment.](createattachment-operation.md)  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, которые необходимо прикрепить к элементу в Exchange магазине.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Вложение элемента не существует как элемент магазина. Он существует только в качестве вложения к элементу или другому вложению. Вложения элементов можно получить только с помощью [запроса GetAttachment.](getattachment.md) 
  
Можно создать следующие вложения элемента:
  
- Item
    
- Сообщение
    
- CalendarItem
    
- Контакт
    
- Задача
    
- MeetingMessage
    
- MeetingRequest
    
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="example"></a>Пример

В следующем примере показано, как создать и прикрепить элемент к другому элементу в Exchange магазине.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
                  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="ASkAS"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>MyAttachment</t:Name>
          <t:Message>
            <t:ItemClass>IPM>Note</t:ItemClass>
            <t:Subject>My attachment subject</t:Subject>
            <t:Body BodyType="Text">My attachment body</t:Body>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateAttachment](createattachment-operation.md)
  
[Операция DeleteAttachment](deleteattachment-operation.md)
  
[Операция GetAttachment](getattachment-operation.md)

