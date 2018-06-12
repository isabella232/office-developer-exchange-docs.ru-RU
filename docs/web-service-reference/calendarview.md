---
title: Представления календаря
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: Элемент представления календаря определяет операцию FindItem как возвращение элементов календаря в наборе, отображенные в календаре.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761659"
---
# <a name="calendarview"></a>Представления календаря

Элемент **представления календаря** определяет [операции FindItem](finditem-operation.md) как возвращение элементов календаря в наборе, отображенные в календаре. 
  
[FindItem](finditem.md)
  
[Представления календаря](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**Представления календаря**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |Описывает максимальное число результатов, возвращаемых в ответе FindItem.  <br/> |
|**Дата начала** <br/> |Идентифицирует Пуск промежуток времени, запрос для элементов календаря. Все элементы календаря, время окончания перед **StartDate** не будут получены. Значение **StartDate** можно указать в формате по Гринвичу (UTC), как и в 2006-01-02T12:00:00Z, или в виде, когда указан смещение местного времени и часового пояса, как и в 2006-01-02T04:00:00-08:00.  <br/><br/>Этот атрибут является обязательным.  <br/> |
|**Дата окончания** <br/> |Определяет конец промежуток времени, запрос для элементов календаря. Не будут возвращены все элементы календаря, имеющие время начала, не ранее **EndDate** . Значение **EndDate** можно указать в формате UTC, что и 2006-02-02T12:00:00Z, или в виде, когда указан смещение местного времени и часового пояса, как и в 2006-02-02T04:00:00-08:00.  <br/><br/>**EndDate** должно быть больше или равно **StartDate**; в противном случае возвращается ошибка. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос для поиска элементов в почтовом ящике.<br/><br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Замечания

Если в запросе FindItem указан элемент **представления календаря** , веб-службы возвращает список элементов одного календаря и вхождения повторяющихся элементов календаря в диапазон, указанный с **StartDate** и **EndDate**.
  
Если элемент **представления календаря** не указан в запросе FindItem, веб-служба возвращает список элементов одного календаря и повторяющихся элементов главного календаря. Календарь вхождения повторяющегося элемента календаря не развертываются. 
  
Запросы представления календаря следует выполнять только используйте следующие свойства, поскольку они поддерживают более быстрых запросов календаря.
  
### <a name="recurrence-blob-properties"></a>Свойства повторения больших двоичных объектов
  
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
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Вычисляется из основного повторения больших двоичных объектов или образец
  
- Идентификатор элемента
    
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
    
### <a name="master-calendar-item-properties"></a>Свойства элемента главного календаря
  
- Идентификатор записи
    
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

В следующем примере показано FindItem запроса. Успешный запрос возвращает ответ, который включает в себя элементы календаря, запускаемых на 2006-05-18T00:00:00-08:00 или после, так и завершенного перед 2006-05-19T00:00:00-08:00.
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [FindItem Operation](finditem-operation.md)
- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

