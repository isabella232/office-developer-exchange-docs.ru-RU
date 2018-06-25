---
title: Чтобы
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- To
api_type:
- schema
ms.assetid: d14e46da-14bd-4a33-a78e-8ee314d9c1d8
description: Элемент кому указывает целевой перехода часового пояса. Целевой объект является период часовой пояс или группу переходы часового пояса.
ms.openlocfilehash: dc7df8ed3ddd6a9b4222ffab4c2b47b00ee4ba0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840194"
---
# <a name="to"></a>Чтобы

Элемент **для** указывает целевой перехода часового пояса. Целевой объект является период часовой пояс или группу переходы часового пояса. 
  
```xml
<To Kind=""/>
```

 **TransitionTargetType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Тип  <br/> |Указывает целевой перехода часовой пояс — это часовой пояс периода или группы переходы часового пояса.  <br/> |
   
#### <a name="kind-attribute-values"></a>Атрибут вида значений

|**Значение**|**Описание**|
|:-----|:-----|
|Точка  <br/> |Указывает, что целевой перехода часовой пояс периода часового пояса.  <br/> |
|Группа  <br/> |Указывает, что целевой перехода часовой пояс группы переходы часового пояса.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AbsoluteDateTransition](absolutedatetransition.md) <br/> |Представляет переход часовой пояс, который создается в конкретный день и в определенное время.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часового пояса, что происходит в тот же день каждый год.  <br/> |
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часового пояса, что происходит на указанном дня года.  <br/> |
|[Переход](transition.md) <br/> |Представляет переход часового пояса.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение — это строка, которая указывает уникальный идентификатор [периода](period.md) или [TransitionsGroup](transitionsgroup.md) , который является целевым для перехода часового пояса. 
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

