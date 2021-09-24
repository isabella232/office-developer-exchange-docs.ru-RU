---
title: To
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: Элемент To указывает цель перехода часового пояса. Целью является период часового пояса или группа переходов часового пояса.
ms.openlocfilehash: 64f3f3258fd7c2bad051eabb1b33617bb056ab39
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522553"
---
# <a name="to"></a>To

Элемент **To** указывает цель перехода часового пояса. Целью является период часового пояса или группа переходов часового пояса. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Kind  <br/> |Указывает, является ли цель перехода часового пояса периодом часового пояса или группой переходов часового пояса.  <br/> |
   
#### <a name="kind-attribute-values"></a>Значения атрибута kind

|**Значение**|**Описание**|
|:-----|:-----|
|Period  <br/> |Указывает, что целью перехода часового пояса является период часового пояса.  <br/> |
|Group  <br/> |Указывает, что целью перехода часового пояса является группа переходов часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Представляет переход часовой пояс, который происходит в определенную дату и в определенное время.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часовой зоны, который происходит каждый год в один и тот же день.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часового пояса, который происходит в указанный день года.  <br/> |
|[Transition](transition.md) <br/> |Представляет переход часовой пояс.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — это строка, которая [](period.md) указывает уникальный идентификатор Периода или [TransitionsGroup,](transitionsgroup.md) который является объектом перехода часового пояса. 
  
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

