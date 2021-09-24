---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: Элемент TransitionsGroups представляет массив групп перехода часового пояса.
ms.openlocfilehash: cd394d0ec333f639542c44cef6c992b24b69f65c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515125"
---
# <a name="transitionsgroups"></a>TransitionsGroups

Элемент **TransitionsGroups** представляет массив групп перехода часового пояса. 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 **ArrayOfTransitionsGroupsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[TransitionsGroup](transitionsgroup.md) <br/> |Представляет массив переходов часового пояса.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |Определяет часовой пояс для времени начала [работы CalendarItem](calendaritem.md) или [MeetingRequest.](meetingrequest.md)  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Определяет часовой пояс для конечного времени [calendarItem](calendaritem.md) или [MeetingRequest.](meetingrequest.md)  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |Определяет часовой пояс.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

