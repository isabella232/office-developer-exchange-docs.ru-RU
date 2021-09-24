---
title: Occurrence (смена часовых поясов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: Элемент Occurrence представляет возникновение дня недели в месяце, когда происходит переход часового пояса.
ms.openlocfilehash: 9790b0e9541da0c22f2eac59850b8a361645c7b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539280"
---
# <a name="occurrence-time-zone-transition"></a>Occurrence (смена часовых поясов)

Элемент **Occurrence** представляет возникновение дня недели в месяце, когда происходит переход часового пояса. 
  
```xml
<Occurrence/>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часовой зоны, который происходит каждый год в один и тот же день.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет собой integer, которое представляет возникновение дня недели в месяце, когда происходит переход часового пояса. В следующей таблице перечислены возможные значения.
  
|**Значение**|**Описание**|
|:-----|:-----|
|1  <br/> |Первое появление указанного дня недели с начала месяца.  <br/> |
|2  <br/> |Второе появление указанного дня недели с начала месяца.  <br/> |
|3   <br/> |Третье появление указанного дня недели с начала месяца.  <br/> |
|4   <br/> |Четвертое появление указанного дня недели с начала месяца.  <br/> |
|-1  <br/> |Первое появление указанного дня недели с конца месяца.  <br/> |
|–2  <br/> |Второе появление указанного дня недели с конца месяца.  <br/> |
|–3  <br/> |Третье появление указанного дня недели с конца месяца.  <br/> |
|-4  <br/> |Четвертое появление указанного дня недели с конца месяца.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, на Microsoft Exchange Server установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

