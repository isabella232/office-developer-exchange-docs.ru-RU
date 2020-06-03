---
title: DayOfMonth
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfMonth
api_type:
- schema
ms.assetid: 09b7504e-08d8-42f9-88cc-a2a37a2e2b8b
description: Элемент DayOfMonth описывает день месяца, в который происходит повторяющийся элемент.
ms.openlocfilehash: dc333a46283d5e8eba3a79f62f8c22c22f56e190
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44442831"
---
# <a name="dayofmonth"></a>DayOfMonth

Элемент **DayOfMonth** описывает день месяца, в который происходит повторяющийся элемент. 
  
```xml
<DayOfMonth/>
```

**int**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[абсолутэйеарлирекурренце](absoluteyearlyrecurrence.md) <br/> |Представляет шаблон ежегодного повторения.  <br/> |
|[абсолутемонслирекурренце](absolutemonthlyrecurrence.md) <br/> |Представляет ежемесячный шаблон повторения.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение, представляющее целое число от 1 до 31. Если для определенного месяца это значение превышает количество дней в месяце, подразумевается последний день месяца.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

