---
title: реминдертипе
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: Элемент Реминдертипе указывает тип напоминаний, которые необходимо вернуть.
ms.openlocfilehash: 4ac20143bbfb29fb8f962515f2faba224b2f973f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465529"
---
# <a name="remindertype"></a>реминдертипе

Элемент **реминдертипе** указывает тип напоминаний, которые необходимо вернуть. 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **строка**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **реминдертипе** — это тип напоминаний, которые возвращаются ( **ALL**, **Current**или **Old**). Для этого элемента рекомендуется использовать значение **ALL** . Дополнительные сведения о связи между элементом Реминдертипе и элементами [бегинтиме](begintime.md) и [EndTime](endtime-remindermessagedatatype.md) можно найти в разделе [Операция](getreminders-operation.md) **ReminderType** .
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[GetReminders](getreminders.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

