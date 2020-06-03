---
title: аттачментшапе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: Элемент Аттачментшапе определяет дополнительные свойства, возвращаемые в ответе на запрос GetAttachment.
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529667"
---
# <a name="attachmentshape"></a>аттачментшапе

Элемент **аттачментшапе** определяет дополнительные свойства, возвращаемые в ответе на запрос [GetAttachment](getattachment.md) . 
  
- [GetAttachment](getattachment.md)
  
- [аттачментшапе](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 **аттачментреспонсешапетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[инклудемимеконтент](includemimecontent.md) <br/> |Указывает, возвращается ли в ответе MIME-контент элемента или вложения. Этот элемент является необязательным.  <br/> |
|[BodyType](bodytype.md) <br/> |Определяет способ форматирования основного текста в отклике. Этот элемент является необязательным.  <br/> |
|[филтерхтмлконтент](filterhtmlcontent.md) <br/> |Указывает, фильтруется ли потенциально небезопасное содержимое HTML из вложения. Этот элемент является необязательным.  <br/> |
|[аддитионалпропертиес](additionalproperties.md) <br/> |Определяет дополнительные свойства, возвращаемые в ответе. Этот элемент является необязательным.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |Элемент, определяющий запрос на получение вложения из почтового ящика в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция GetAttachment](getattachment-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

