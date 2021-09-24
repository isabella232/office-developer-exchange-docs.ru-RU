---
title: RecurringDateTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: Элемент RecurringDateTransition представляет переход часовой пояс, который происходит в определенную дату каждый год.
ms.openlocfilehash: 864f3f539c5440fbfc539ca6c2042b3d9edca267
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529365"
---
# <a name="recurringdatetransition"></a>RecurringDateTransition

Элемент **RecurringDateTransition** представляет переход часовой пояс, который происходит в определенную дату каждый год. 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 **RecurringDateTransitionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[To](to.md) <br/> |Указывает период [или](period.md) [TransitionsGroup,](transitionsgroup.md) которые должны быть объектом перехода часового пояса.  <br/> |
|[TimeOffset](timeoffset.md) <br/> |Представляет смещение длительности от согласованного универсального времени (UTC) для перехода часового пояса.  <br/> |
|[Month (смена часовых поясов)](month-time-zone-transition.md) <br/> |Представляет месяц, в котором происходит переход часового пояса.  <br/> |
|[Day](day.md) <br/> |Представляет день месяца, в который происходит переход часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Transitions](transitions.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
|[TransitionsGroup](transitionsgroup.md) <br/> |Представляет коллекцию переходов часового пояса.  <br/> |
   
## <a name="remarks"></a>Заметки

Пример перехода часового пояса, который может быть представлен элементом [RecurringDateTransition,](recurringdatetransition.md) это переход, который происходит каждый год 15 марта. 
  
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

