---
title: Месяц (часовой пояс переходов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: 5e6aac75-366d-43d0-8ccb-956285474662
description: Элемент Month представляет месяц, в котором осуществляется часового пояса.
ms.openlocfilehash: 887bd750b9cad1e28e6f7603c7b3289da8f8dc07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834483"
---
# <a name="month-time-zone-transition"></a>Месяц (часовой пояс переходов)

Элемент **Month** представляет месяц, в котором осуществляется часового пояса. 
  
```xml
<Month/>
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
|[RecurringDateTransition](recurringdatetransition.md) <br/> |Представляет переход часового пояса, что происходит в конкретный день каждый год.  <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |Представляет переход часового пояса, что происходит в тот же день каждый год.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет собой целое число, представляющее месяц, в котором осуществляется часового пояса.
  
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

