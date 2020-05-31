---
title: StartDate (повторение)
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
# <a name="startdate-recurrence"></a>StartDate (повторение)

Элемент **StartDate** представляет дату начала повторяющейся задачи или элемента календаря. 
  
```xml
<StartDate/>
```

**Date**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[енддатерекурренце](enddaterecurrence.md) <br/> |Описывает дату начала и дату окончания расписания повторения элемента.  <br/> |
|[ноендрекурренце](noendrecurrence.md) <br/> |Описывает дату начала для шаблона повторения элемента, у которого нет определенной конечной даты.  <br/> |
|[нумбередрекурренце](numberedrecurrence.md) <br/> |Описывает дату начала и число повторений повторяющегося элемента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее дату, является обязательным при использовании этого элемента. Значение не может быть меньше Апр, 1, 1601 00:00:00.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

