---
title: рекуррингдатетранситион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: Элемент Рекуррингдатетранситион представляет переход часового пояса, который выполняется в определенный день каждого года.
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461578"
---
# <a name="recurringdatetransition"></a>рекуррингдатетранситион

Элемент **рекуррингдатетранситион** представляет переход часового пояса, который выполняется в определенный день каждого года. 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 **рекуррингдатетранситионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[To](to.md) <br/> |Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.  <br/> |
|[тимеоффсет](timeoffset.md) <br/> |Представляет смещение длительности от времени в формате UTC для смены часового пояса.  <br/> |
|[Month (переход часового пояса)](month-time-zone-transition.md) <br/> |Представляет месяц, в который происходит переход часового пояса.  <br/> |
|[Day](day.md) <br/> |Представляет день месяца, в который происходит переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Выполняет](transitions.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
|[транситионсграуп](transitionsgroup.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
   
## <a name="remarks"></a>Примечания

Примером перехода по часовому поясу, который может быть представлен элементом [рекуррингдатетранситион](recurringdatetransition.md) , является переход, который выполняется 15 марта каждый год. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

