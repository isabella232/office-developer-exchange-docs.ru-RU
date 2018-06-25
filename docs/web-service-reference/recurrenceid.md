---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: Элемент RecurrenceId используется для идентификации определенный экземпляр повторяющегося элемента календаря.
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835005"
---
# <a name="recurrenceid"></a>RecurrenceId

Элемент **RecurrenceId** используется для идентификации определенный экземпляр повторяющегося элемента календаря. 
  
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
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашения на собрание.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмены собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение даты и времени, которое идентифицирует вхождение календаря.
  
## <a name="remarks"></a>Замечания

Это свойство используется со свойством [Уникальный идентификатор](uid.md) для идентификации определенный экземпляр повторяющегося элемента календаря. 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

