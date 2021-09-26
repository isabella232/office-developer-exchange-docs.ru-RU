---
title: GetAttachment
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
ms.assetid: 9443cf96-b451-4530-b868-490dff798673
description: Элемент GetAttachment — это корневой элемент запроса на вложение из Exchange магазина.
ms.openlocfilehash: 057b42e78845f583cf1e52804e0108f335ef951c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546373"
---
# <a name="getattachment"></a>GetAttachment

Элемент **GetAttachment** — это корневой элемент запроса на вложение из Exchange магазина. 
  
```xml
<GetAttachment>
   <AttachmentShape/>
   <AttachmentIds/>
</GetAttachment>
```

 **GetAttachmentType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> |Определяет дополнительные свойства расширенных элементов, которые возвращаются в ответ на запрос [GetAttachment.](getattachment.md) Этот элемент является необязательным.  <br/> |
|[AttachmentIds](attachmentids.md) <br/> |Содержит массив идентификаторов вложений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Элемент [AttachmentShape](attachmentshape.md) не требуется для определения свойств, возвращенных в ответе. Операция [GetAttachment](getattachment-operation.md) возвращает свойства Name, ContentType, ContentId, ContentLocation и свойств контента для вложений файлов. Для вложений элементов возвращаются свойства Name, ContentType, ContentId, ContentLocation и все свойства присоединенного элемента. Это эквивалентно использованию базовой формы AllProperties в [запросе GetItem.](getitem.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetAttachment](getattachment-operation.md)
  
[GetAttachmentResponse](getattachmentresponse.md)

