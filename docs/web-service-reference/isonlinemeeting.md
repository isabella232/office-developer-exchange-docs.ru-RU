---
title: IsOnlineMeeting
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsOnlineMeeting
api_type:
- schema
ms.assetid: c29df676-0f3a-4694-a42f-522c6d16872f
description: Элемент IsOnlineMeeting указывает, находится ли собрание в сети.
ms.openlocfilehash: 3521cf82f2b6b2b2514b82478fc4e1e5c6edb563
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514517"
---
# <a name="isonlinemeeting"></a>IsOnlineMeeting

Элемент **IsOnlineMeeting** указывает, находится ли собрание в сети. 
  
```xml
<IsOnlineMeeting/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MeetingRequest](meetingrequest.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если этот элемент используется, требуется текстовое значение, представляю которое представляет значение Boolean. Значение true **указывает,** что собрание находится в сети. Значение false **указывает** на то, что собрание не находится в сети. 
  
## <a name="remarks"></a>Заметки

Свойство IsOnlineMeeting можно прочитать для элемента календаря организатора. Это только для чтения запросов на собрания и для элементов календаря участников.
  
Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS под управлением MicrosoftExchange 2007 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

