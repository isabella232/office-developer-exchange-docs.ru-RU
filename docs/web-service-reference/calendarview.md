---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: Элемент CalendarView определяет операцию FindItem как возвращающие элементы календаря в наборе по мере их появления в календаре.
ms.openlocfilehash: 5e0180bb5e8a6d9fcbe42380abbe32820117ae29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518829"
---
# <a name="calendarview"></a>CalendarView

Элемент **CalendarView** определяет операцию [FindItem](finditem-operation.md) как возвращающие элементы календаря в наборе по мере их появления в календаре. 
  
[FindItem](finditem.md)
  
[CalendarView](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**CalendarView**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное количество результатов, возвращаемых в ответе FindItem.  <br/> |
|**StartDate** <br/> |Определяет начало периода времени, запрашиваемого для элементов календаря. Все элементы календаря с конечным временем до **начала startDate** не возвращаются. Значение **StartDate** можно указать в согласованном формате универсального времени (UTC), как в формате 2006-01-02T12:00:00:00Z, или в формате, в котором указывается смещение времени и часового пояса, как в 2006-01-02T04:00-00-08:00.  <br/><br/>Этот атрибут является обязательным.  <br/> |
|**EndDate** <br/> |Определяет конец периода времени, запрашиваемого для элементов календаря. Все элементы календаря с временем начала или после **EndDate** не возвращаются. Значение **EndDate** можно указать в формате UTC, как в формате 2006-02-02T12:00:00Z, или в формате, в котором задан смещение местного времени и часового пояса, как в 2006-02-02T04:00-00-08:00.  <br/><br/>**EndDate** должен быть больше или равняться **StartDate;** в противном случае возвращается ошибка. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.<br/><br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Заметки

Если элемент **CalendarView** указан в запросе FindItem, веб-служба возвращает список элементов календаря и случаев повторения элементов календаря в диапазоне, заданном **StartDate** и **EndDate.**
  
Если элемент **CalendarView** не указан в запросе FindItem, веб-служба возвращает список элементов одного календаря и повторяющихся основных элементов календаря. Календарь возникновения повторяющегося элемента календаря не расширяется. 
  
Запросы CalendarView должны использовать только следующие свойства, так как они поддерживают более быстрые запросы календаря.
  
### <a name="recurrence-blob-properties"></a>Свойства blob повторения
  
- MapiStartTime
    
- MapiEndTime
    
- SubjectPrefixInternal
    
- NormalizedSubjectInternal
    
- MapiSubject
    
- Location
    
- AppointmentColor
    
- MapiIsAllDayEvent
    
- MapiHasAttachment
    
- FreeBusyStatus
    
- ReminderIsSetInternal
    
- ReminderMinutesBeforeStartInternal
    
- AppointmentState
    
- AllAttachmentsHidden
    
- ChangeHighlight
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Вычисляется из основного blob-blob или master рецидива
  
- ItemId
    
- IsRecurring
    
- IsException
    
- AppointmentRecurring
    
- MapiStartTime
    
- MapiPRStartDate
    
- MapiEndTime
    
- MapiPREndDate
    
- CalendarItemType
    
- GlobalObjectId
    
- TimeZoneDefinitionStart
    
- TimeZoneDefinitionEnd
    
### <a name="master-calendar-item-properties"></a>Свойства элемента Master calendar
  
- EntryId
    
- ChangeKey
    
- ItemClass
    
- SentRepresentingEmailAddress
    
- SentRepresentingDisplayName
    
- SentRepresentingEntryId
    
- AppointmentRecurrenceBlob
    
- TimeZone
    
- TimeZoneBlob
    
- TimeZoneDefinitionRecurring
    
- CleanGlobalObjectId
    
- AppointmentRecurring
    
- IsException
    
- IsRecurring
    
- MapiSensitivity
    
- ContainerClass
    
- MapiPRStartDate
    
- MapiPREndDate
    
- Categories
    
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере показан запрос FindItem. Успешный запрос возвращает ответ, который включает элементы календаря, которые начались в 2006-05-18T00:00:00-08:00 или после и закончились до 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

