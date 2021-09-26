---
title: StartDate (Recurrence)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StartDate
api_type:
- schema
ms.assetid: bd65ac06-b3ac-4c9b-9568-3e4dc94378e7
description: Элемент StartDate представляет дату начала повторяющейся задачи или элемента календаря.
ms.openlocfilehash: 50f83e5c97d346cc3f7dfced1ee71aa3f9f38ed5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59545869"
---
# <a name="startdate-recurrence"></a>StartDate (Recurrence)

Элемент **StartDate** представляет дату начала повторяющейся задачи или элемента календаря. 
  
```xml
<StartDate/>
```

**Date**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[EndDateRecurrence](enddaterecurrence.md) <br/> |Описывает дату начала и дату окончания шаблона повторения элементов.  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |Описывает дату начала шаблона повторения элементов, который не имеет определенной конечной даты.  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |Описывает дату начала и количество вхождений повторяющегося элемента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет дату. Значение не может быть меньше 1 апреля 1601 00:00:00.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

