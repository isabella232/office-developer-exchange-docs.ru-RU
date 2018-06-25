---
title: StartDate (повторения)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: Элемент StartDate представляет дату начала повторяющейся задачи или элемента календаря.
ms.openlocfilehash: 6a38e63bbcf010ab6dca8f66440a2b0a559cf88d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835551"
---
# <a name="startdate-recurrence"></a>StartDate (повторения)

Элемент **StartDate** представляет дату начала повторяющейся задачи или элемента календаря. 
  
```xml
<StartDate/>
```

**Дата**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Описание, Дата начала и Дата окончания повторения элемента.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Описывает дату начала повторения элемента, для которого не определенные дату.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Описание, Дата начала и число вхождений повторяющегося элемента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, которое представляет дату является обязательным, если данный элемент используется. Значение не может быть меньше, чем апреля, 1 1601 00:00:00.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

