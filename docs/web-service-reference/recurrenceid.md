---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: Элемент RecurrenceId используется для определения определенного экземпляра повторяющегося элемента календаря.
ms.openlocfilehash: 863673f7439c12ce4c74e8e0ef4ddea996fb4eb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527566"
---
# <a name="recurrenceid"></a>RecurrenceId

Элемент **RecurrenceId** используется для определения определенного экземпляра повторяющегося элемента календаря. 
  
```xml
<RecurrenceId/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет запрос на собрание.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ собрания.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение даты и времени, которое определяет возникновение календаря.
  
## <a name="remarks"></a>Заметки

Это свойство используется с свойством [UID](uid.md) для определения определенного экземпляра повторяющегося элемента календаря. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

