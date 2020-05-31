---
title: CalendarView
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
description: Элемент CalendarView определяет операцию FindItem, возвращая элементы календаря в наборе в том виде, в котором они отображаются в календаре.
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761659"
---
# <a name="calendarview"></a>CalendarView

Элемент **CalendarView** определяет [операцию FindItem](finditem-operation.md) , возвращая элементы календаря в наборе в том виде, в котором они отображаются в календаре. 
  
[FindItem](finditem.md)
  
[CalendarView](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**CalendarView**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**максентриесретурнед** <br/> |Описывает максимальное число результатов, возвращаемых в ответе FindItem.  <br/> |
|**StartDate** <br/> |Указывает начало интервала времени, запрашиваемого для элементов календаря. Все элементы календаря с временем окончания, предшествующим **StartDate** , не будут возвращены. Значение **StartDate** может указываться в формате UTC, как в 2006 – 01-02T12:00:00Z или в формате, где указано местное время и смещение часового пояса, как в 2006 – 01-02T04:00:00-08:00.  <br/><br/>Этот атрибут является обязательным.  <br/> |
|**EndDate** <br/> |Определяет конец интервала времени, запрашиваемого для элементов календаря. Все элементы календаря, время начала которых находится в начале или после **даты окончания** , не будут возвращены. Значение параметра **EndDate** можно указать в формате UTC, как в 2006-02-02T12:00:00Z, или в формате, где указаны местное время и смещение часового пояса, например, в 2006-02-02T04:00:00-08:00.  <br/><br/>Значение **EndDate** должно быть больше или равно значению **StartDate**; в противном случае возвращается ошибка. Этот атрибут является обязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |Определяет запрос на поиск элементов в почтовом ящике.<br/><br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>Примечания

Если элемент **CalendarView** указан в запросе FindItem, веб-служба возвращает список одиночных элементов календаря и повторение повторяющихся элементов календаря в диапазоне, заданном в параметрах **StartDate** и **EndDate**.
  
Если элемент **CalendarView** не указан в запросе FindItem, веб-служба возвращает список одиночных элементов календаря и повторяющихся элементов основного календаря. Экземпляры повторяющегося элемента календаря не разворачиваются. 
  
В запросах CalendarView следует использовать только следующие свойства, так как они поддерживают более быстрые запросы в календаре.
  
### <a name="recurrence-blob-properties"></a>Свойства больших двоичных объектов повторения
  
- мапистарттиме
    
- мапиендтиме
    
- субжектпрефиксинтернал
    
- нормализедсубжектинтернал
    
- маписубжект
    
- Расположение
    
- аппоинтментколор
    
- мапиисаллдайевент
    
- мапихасаттачмент
    
- фрибусистатус
    
- реминдериссетинтернал
    
- реминдерминутесбефорестартинтернал
    
- аппоинтментстате
    
- AllAttachmentsHidden
    
- чанжехигхлигхт
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>Рассчитывается на основе основного объекта BLOB или основного объекта повторения
  
- Идентификатор
    
- IsRecurring
    
- Исключение
    
- аппоинтментрекурринг
    
- мапистарттиме
    
- мапипрстартдате
    
- мапиендтиме
    
- мапипренддате
    
- календаритемтипе
    
- глобалобжектид
    
- тимезонедефинитионстарт
    
- тимезонедефинитионенд
    
### <a name="master-calendar-item-properties"></a>Свойства элемента главного календаря
  
- Код
    
- чанжекэй
    
- ItemClass
    
- сентрепресентинжемаиладдресс
    
- сентрепресентингдисплайнаме
    
- сентрепресентинжентрид
    
- аппоинтментрекурренцеблоб
    
- TimeZone
    
- тимезонеблоб
    
- тимезонедефинитионрекурринг
    
- клеанглобалобжектид
    
- аппоинтментрекурринг
    
- Исключение
    
- IsRecurring
    
- маписенситивити
    
- контаинеркласс
    
- мапипрстартдате
    
- мапипренддате
    
- Категории
    
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В приведенном ниже примере показан запрос FindItem. Успешный запрос возвращает ответ, включающий элементы календаря, запущенные в 2006 г. 05 – 18T00:00:00 – 08:00 или позже и заканчиваются до 2006 г. 05 – 19T00:00:00:00.
  
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
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция FindItem](finditem-operation.md)
- [Поиск элементов](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

