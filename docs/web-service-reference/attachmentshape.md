---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: Элемент AttachmentShape определяет дополнительные свойства, возвращающиеся в ответ на запрос GetAttachment.
ms.openlocfilehash: 2c7ceb25f481ec07577117e46e26537e657e18c7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520040"
---
# <a name="attachmentshape"></a>AttachmentShape

Элемент **AttachmentShape** определяет дополнительные свойства, возвращающиеся в ответ на запрос [GetAttachment.](getattachment.md) 
  
- [GetAttachment](getattachment.md)
  
- [AttachmentShape](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 **AttachmentResponseShapeType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |Указывает, возвращается ли в ответ многоцелевой контент расширения интернет-почты (MIME) элемента или вложения. Этот элемент является необязательным.  <br/> |
|[BodyType](bodytype.md) <br/> |Определяет форматирование текста тела в ответе. Этот элемент является необязательным.  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |Указывает, фильтруется ли потенциально небезопасное содержимое HTML из вложения. Этот элемент является необязательным.  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответ. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |Элемент, определяющие запрос на вложение из почтового ящика в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetAttachment](getattachment-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

