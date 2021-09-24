---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: Элемент ExceptionFieldURI определяет определенные ошибки в запросе. Этот элемент используется только в качестве части ответа на ошибку в узле MessageXml.
ms.openlocfilehash: 7368fd51e8eca2081b1fd50c86bce9ffa469c6b1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524331"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

Элемент **ExceptionFieldURI** определяет определенные ошибки в запросе. Этот элемент используется только в качестве части ответа на ошибку в узле [MessageXml.](messagexml.md) 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**FieldURI** <br/> |Определяет свойство возникновения повторяющегося элемента. Этот атрибут является обязательным.  <br/> |
   
#### <a name="fielduri-attribute"></a>Атрибут FieldURI

|**Значение**|**Описание**|
|:-----|:-----|
|attachment:Name  <br/> |Определяет имя вложения как содержащее ошибку.  <br/> |
|attachment:ContentType  <br/> |Определяет тип контента как содержащий ошибку.  <br/> |
|attachment:Content  <br/> |Определяет содержимое как содержащее ошибку.  <br/> |
|recurrence:Month  <br/> |Определяет поле месяца как содержащее ошибку.  <br/> |
|recurrence:DayOfWeekIndex  <br/> |Определяет день индекса недели как содержащий ошибку.  <br/> |
|recurrence:DaysOfWeek  <br/> |Определяет свойство DaysOfWeek как содержащее ошибку.  <br/> |
|recurrence:DayOfMonth  <br/> |Определяет DayOfMonth как содержащий ошибку.  <br/> |
|recurrence:Interval  <br/> |Определяет интервал как содержащий ошибку.  <br/> |
|recurrence:NumberOfOccurrences  <br/> |Определяет количество случаев, содержащих ошибку.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об отклике с ошибкой.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

