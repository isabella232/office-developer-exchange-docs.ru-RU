---
title: Шаблоны повторения и EWS
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Сведения о шаблонах повторения и повторяющихся рядах в Exchange.
ms.openlocfilehash: 681dfee7e0a66a483b8638810da5e4e0ac0f05ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459330"
---
# <a name="recurrence-patterns-and-ews"></a>Шаблоны повторения и EWS

Сведения о шаблонах повторения и повторяющихся рядах в Exchange.
  
Повторяющийся ряд — это встреча или собрание, повторяющиеся в соответствии с определенным шаблоном. Повторяющиеся ряды могут иметь определенное количество повторений или может повторяться в течение неопределенного периода. Кроме того, повторяющиеся ряды могут содержать исключения, которые не следуют шаблону остальных вхождений, и могут иметь экземпляры, удаленные из шаблона. Вы можете использовать управляемый API EWS и EWS для работы с повторяющимися сериями и связанными с ними элементами календаря.
  
## <a name="recurring-calendar-items"></a>Повторяющиеся элементы календаря

Все элементы календаря делятся на одну из следующих четырех категорий:
  
- Неповторяющиеся элементы календаря
    
- Повторяющиеся шаблоны
    
- Вхождения в серии
    
- Измененные экземпляры в серии, называемые исключениями
    
В этой статье мы рассмотрим три типа элементов календаря, которые входят в повторяющиеся ряды.
  
Полезно знать, как повторяющиеся ряды реализуются на сервере Exchange. Вместо того чтобы создавать отдельный отдельный элемент для каждого вхождения в повторяющейся серии, сервер создает в календаре только один фактический элемент, называемый повторяющимся образцом. Формат повторяющейся основной схемы очень похож на неповторяющуюся встречу с добавлением сведений о расписании повторения. Затем сервер создает экземпляры на основе шаблона повторения в ответ на клиентские запросы для сведений о встрече, используя процесс, называемый расширением. Эти созданные экземпляры не будут безвозвратно храниться на сервере. Это важно понимать, так как поиск элементов календаря определяет, какие сведения вы получаете и как происходит расширение.
  
## <a name="recurrence-patterns"></a>Расписания повторения

Основной частью ряда повторяющихся данных является периодичность расширения. Шаблон повторения находится на повторяющейся основной странице, а также описывает набор критериев для расчета вхождений на основе даты и времени повторяющегося образца.
  
**Таблица 1. Доступные шаблоны повторения**

|**Класс управляемого API EWS**|**Элемент EWS**|**Примеры**|
|:-----|:-----|:-----|
|[Повторение. Даилипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[даилирекурренце](https://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Повторять каждый день.  <br/> Повторять каждый день.  <br/> |
|[Повторение. Монслипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[абсолутемонслирекурренце](https://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Повторять каждый месяц на десятый день месяца.  <br/> Повторять каждый второй месяц в двадцать первый день месяца.  <br/> |
|[Повторение. Релативемонслипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[релативемонслирекурренце](https://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Повторяйте во второй вторник каждого месяца.  <br/> Повторяйте в третий четверг месяца каждые три месяца.  <br/> |
|[Повторение. Релативэйеарлипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[релативэйеарлирекурренце](https://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Повторяйте на первом понедельник августа каждый год.  <br/> |
|[Повторение. Виклипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[виклирекурренце](https://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Повторяйте каждый понедельник.  <br/> Повторяйте каждый вторник и четверг каждую вторую неделю.  <br/> |
|[Повторение. Еарлипаттерн](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[абсолутэйеарлирекурренце](https://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Повторяйте каждый год 1 сентября.  <br/> |
   
Другой важный фрагмент данных для шаблона повторения — по окончании повторения. Может быть выражено как заданное число повторений, как Дата окончания, так и без окончания.
  
**Таблица 2. Варианты для конца повторяющейся серии**

|**Метод или свойство управляемого API EWS**|**Элемент EWS**|**Описание**|
|:-----|:-----|:-----|
|[Повторение. Нумберофоккурренцес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[нумбередрекурренце](https://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |Значение этого свойства или элемента указывает количество повторений.  <br/> |
|[Повторение. EndDate](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[енддатерекурренце](https://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |Последнее вхождение в ряду приходится на или предшествует дате, указанной этим свойством или элементом.  <br/> |
|[Повторение. Хасенд](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Повторение. Неверендс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[ноендрекурренце](https://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |У ряда нет конца.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Расширенные и нерасширенные представления

Вызов процесса расширения с помощью метода **FindAppointments** в УПРАВЛЯЕМОМ API EWS (или операции **FindItem** с элементом **CalendarView** в EWS). Это скрывает повторяющиеся основные встречи из набора результатов, а вместо этого предоставляет расширенное представление этой серии. Экземпляры и исключения из повторяющейся основной реплики, которые попадают в параметры представления календаря, включаются в результирующий набор. С другой стороны, с помощью метода **FindItems** в УПРАВЛЯЕМОМ API EWS (или операции **FindItem** с элементом **индекседпажеитемвиев** или **фрактионалпажеитемвиев** в EWS) не вызывается процесс расширения, а экземпляры и исключения не включаются. Рассмотрим пример сравнения двух методов. 
  
**Таблица 3. Методы и операции для поиска встреч**

|**Метод управляемого API EWS**|**Операция EWS**|**Разворачивает ряды?**|**Элементы, включенные в результаты**|
|:-----|:-----|:-----|:-----|
|[ExchangeService. FindAppointments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Да  <br/> |Неповторяющиеся встречи, отдельные экземпляры повторяющихся рядов и исключения из повторяющихся рядов  <br/> |
|[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [Индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элементом [фрактионалпажеитемвиев](https://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Нет  <br/> |Неповторяющиеся встречи и повторяющиеся запланированные встречи  <br/> |
   
Ольга только что подписался на себя для группы свим. У группы есть упражнения каждую среду утром в 8:30 AM, начиная с 2 июля, с последней практикой из 6 августа. Не нужно забывать о практике, Ольга добавляет повторяющуюся встречу в свой календарь для напоминания.
  
**Таблица 4. Повторяющаяся встреча Ольга**

|**Поле "Встреча"**|**Значение**|
|:-----|:-----|
|Subject  <br/> |Практика группы свим  <br/> |
|Начало  <br/> |2 июля 2014 8:30 AM  <br/> |
|Конец  <br/> |2 июля 2014 10:00 AM  <br/> |
|Повторяется  <br/> |Каждую среду  <br/> |
|Последнее событие  <br/> |6 августа 2014 8:30 AM  <br/> |
   
Краткий обзор календаря показывает, что у команды будет всего шесть практических рекомендаций. Однако в календаре не существует шести отдельных элементов встречи. Вместо этого существует только одна повторяющаяся Главная встреча, представляющая ряд.
  
Теперь рассмотрим Поиск встреч в календаре Ольга, который встречается в июле. В следующем примере кода используется метод **FindItems** в управляемом API Exchange для создания нерасширенного представления календаря Ольга. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
#region FindItems + ItemView method
ItemView itemView = new ItemView(100);
itemView.PropertySet = propSet;
List<SearchFilter> filterList = new List<SearchFilter>();
// Find appointments that start after midnight on July 1, 2014.
SearchFilter.IsGreaterThan startFilter = new SearchFilter.IsGreaterThan(AppointmentSchema.Start,
    new DateTime(2014, 7, 1));
// Find appointments that end before midnight on July 31, 2014
SearchFilter.IsLessThan endFilter = new SearchFilter.IsLessThan(AppointmentSchema.End,
    new DateTime(2014, 7, 31));
filterList.Add(startFilter);
filterList.Add(endFilter);
SearchFilter.SearchFilterCollection calendarFilter = new SearchFilter.SearchFilterCollection(LogicalOperator.And, filterList);
// This results in a call to EWS.
FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Calendar, calendarFilter, itemView);
foreach(Item appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Этот код приводит к следующему запросу [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="100" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:IsGreaterThan>
            <t:FieldURI FieldURI="calendar:Start" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-01T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsGreaterThan>
          <t:IsLessThan>
            <t:FieldURI FieldURI="calendar:End" />
            <t:FieldURIOrConstant>
              <t:Constant Value="2014-07-31T07:00:00.000Z" />
            </t:FieldURIOrConstant>
          </t:IsLessThan>
        </t:And>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Ответ сервера включает в себя только один элемент — шаблон повторения, указанный значением элемента [календаритемтипе](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) в **рекуррингмастер**. Значение элемента [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) было сокращено для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA5..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>RecurringMaster</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

Теперь выполним сравнение с расширенным представлением. В следующем примере кода используется метод **FindAppointments** в УПРАВЛЯЕМОМ API EWS для создания расширенного представления календаря Ольга. 
  
```cs
PropertySet propSet = new PropertySet(AppointmentSchema.Subject,
                                      AppointmentSchema.Location,
                                      AppointmentSchema.Start, 
                                      AppointmentSchema.End,
                                      AppointmentSchema.AppointmentType);
CalendarView calView = new CalendarView(new DateTime(2014, 7, 1),
    new DateTime(2014, 7, 31));
calView.PropertySet = propSet;
FindItemsResults<Appointment> results = service.FindAppointments(WellKnownFolderName.Calendar, calView);
foreach(Appointment appt in results.Items)
{
    Console.WriteLine(appt.Subject);
}
```

Этот код приводит к следующему запросу [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [CalendarView](https://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="calendar:Location" />
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
          <t:FieldURI FieldURI="calendar:CalendarItemType" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView StartDate="2014-07-01T07:00:00.000Z" EndDate="2014-07-31T07:00:00.000Z" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

В этот раз ответ сервера включает пять повторений, по одному для каждой среды в июле. Элементы [календаритемтипе](https://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) для этих элементов имеют значение " **экземпляр**". Обратите внимание, что в отклике отсутствует шаблон повторения. Значения элементов [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) были сокращены для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder TotalItemsInView="5" IncludesLastItemInRange="true">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA6..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-02T15:30:00Z</t:Start>
                <t:End>2014-07-02T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA7..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-09T15:30:00Z</t:Start>
                <t:End>2014-07-09T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA8..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-16T15:30:00Z</t:Start>
                <t:End>2014-07-16T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADA9..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-23T15:30:00Z</t:Start>
                <t:End>2014-07-23T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
              <t:CalendarItem>
                <t:ItemId Id="AAMkADAA..." ChangeKey="DwAAABYA..." />
                <t:Subject>Swim Team Practice</t:Subject>
                <t:Start>2014-07-30T15:30:00Z</t:Start>
                <t:End>2014-07-30T17:00:00Z</t:End>
                <t:Location>Neighborhood Swimming Pool</t:Location>
                <t:CalendarItemType>Occurrence</t:CalendarItemType>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

После создания повторяющегося образца, вхождения или исключения всегда можно [получить другие связанные элементы](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Получив исключение, вы можете извлечь шаблон повторения и наоборот.
  
## <a name="working-with-recurring-calendar-items"></a>Работа с повторяющимися элементами календаря

Для работы с повторяющимися элементами календаря используются те же методы и операции, что и при работе с неповторяющимися элементами календаря. Разница заключается в том, что в зависимости от элемента, используемого для вызова этих методов или операций, выполняемые действия можно применить ко всей серии или только к одному экземпляру. [Действия, выполняемые на повторяющейся основной реплике](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) , будут применяться ко всем вхождениям в ряду, в то время как [действия, выполненные с одним экземпляром или исключением](how-to-update-a-recurring-series-by-using-ews.md) , будут применяться только к этому экземпляру или исключению. 
  
## <a name="in-this-section"></a>В этой статье

- [Доступ к повторяющимся сериям с помощью EWS в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание серии повторяющихся данных с помощью EWS в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Удаление встреч из серии повторяющихся данных с помощью EWS в Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся данных с помощью EWS](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление серии повторяющихся данных с помощью EWS в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Получение встреч и собраний с помощью EWS в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

