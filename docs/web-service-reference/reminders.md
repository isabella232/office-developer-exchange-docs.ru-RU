---
title: Reminders
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 19294300-ab84-4784-8aa7-3395a08de640
description: Элемент Reminders указывает напоминания, возвращенные в ответ на запрос GetReminders.
ms.openlocfilehash: 0b760e93bf27f0fdaad9464580fad924367dea32
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513411"
---
# <a name="reminders"></a>Reminders

Элемент **Reminders** указывает напоминания, возвращенные в ответ на **запрос GetReminders.** 
  
```XML
<Reminders>
   <Reminder></Reminder>
</Reminders>
```

 **ArrayOfRemindersType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

[Reminder](reminder.md)
  
### <a name="parent-elements"></a>Родительские элементы

[GetRemindersResponse](getremindersresponse.md)
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[GetRemindersResponse](getremindersresponse.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

