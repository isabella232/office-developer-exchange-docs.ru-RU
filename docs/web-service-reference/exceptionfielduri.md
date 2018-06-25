---
title: ExceptionFieldURI
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExceptionFieldURI
api_type:
- schema
ms.assetid: 7afda93a-0f8c-4c9e-8e09-f1b0bfc928bf
description: Элемент ExceptionFieldURI идентифицирует определенные ошибки в запросе. Этот элемент используется только как часть ответа об ошибке в узле MessageXml.
ms.openlocfilehash: 79909405179cec0d0b86ad12bf52031e1daeb790
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762408"
---
# <a name="exceptionfielduri"></a>ExceptionFieldURI

Элемент **ExceptionFieldURI** идентифицирует определенные ошибки в запросе. Этот элемент используется только как часть ответа об ошибке в узле [MessageXml](messagexml.md) . 
  
```xml
<ExceptionFieldURI FieldURI="" />
```

 **ExceptionPropertyURIType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**FieldURI** <br/> |Определяет свойство вхождения повторяющегося элемента. Этот атрибут является обязательным.  <br/> |
   
#### <a name="fielduri-attribute"></a>Атрибут FieldURI

|**Значение**|**Описание**|
|:-----|:-----|
|Имя: вложения  <br/> |Определяет имя вложения, содержащий ошибку.  <br/> |
|вложения: ContentType  <br/> |Идентифицирует тип контента как содержащий ошибки.  <br/> |
|Содержимое вложения:  <br/> |Задает содержимое, как содержащий ошибки.  <br/> |
|Повторение: месяц  <br/> |Определяет поле месяц как содержащий ошибки.  <br/> |
|Повторение: DayOfWeekIndex  <br/> |Определяет день недели индекса, содержащее ошибку.  <br/> |
|Повторение: DaysOfWeek  <br/> |Определяет свойство DaysOfWeek как содержащий ошибки.  <br/> |
|Повторение: день месяца  <br/> |Определяет день месяца, содержащее ошибку.  <br/> |
|Интервал повторения:  <br/> |Задает интервал, содержащее ошибку.  <br/> |
|Повторение: NumberOfOccurrences  <br/> |Определяет число вхождений как содержащий ошибки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MessageXml](messagexml.md) <br/> |Предоставляет дополнительные сведения об ошибке ответа.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

