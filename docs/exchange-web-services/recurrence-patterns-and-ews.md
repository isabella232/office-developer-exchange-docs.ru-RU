---
title: Шаблоны повторения и веб-служб Exchange
manager: luken
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: fd9ef706-1e01-49fa-af6f-2f6d3e173c16
description: Сведения о шаблоны повторения и ряд повторяющейся в Exchange.
ms.openlocfilehash: ac10e9b9a347abb5907b77f0e0e7315e4e86d97a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761244"
---
# <a name="recurrence-patterns-and-ews"></a>Шаблоны повторения и веб-служб Exchange

Сведения о шаблоны повторения и ряд повторяющейся в Exchange.
  
Серии повторяющихся — встречи или собрания, повторяет согласно заданному шаблону. Серии повторяющихся либо может иметь определенного количества экземпляров или можно повторить неопределенное время. Кроме того, серии повторяющихся может иметь исключения, которые не отвечают шаблону остальную часть вхождений и может иметь вхождения, которые были удалены из шаблона. Для работы с серии повторяющихся и их элементы связанного календаря можно использовать управляемый API EWS и веб-служб Exchange.
  
## <a name="recurring-calendar-items"></a>Повторяющихся элементов календаря

Все элементы календаря попадают в одну из следующих четырех категорий:
  
- Неповторяющихся элементов календаря
    
- Повторяющееся образцов
    
- Вхождения в цикле
    
- Измененные вхождений в серии, известных как исключения
    
В этой статье мы рассмотрим трех типов элементов календаря, являющихся частью серии повторяющихся.
  
Будет полезно понять, как повторяющееся реализован на сервере Exchange. Вместо создания элемент уникальных для каждого повтора в ряду, сервер создает только один элемент фактические в календаре, известных как образца повторения. Формат образца повторения очень похоже на неповторяющейся встречи с добавлением информации шаблон повторения. Сервер создает на основе шаблона повторения в ответ на запросы клиентов для данные о встрече, используя процесс с именем расширения вхождений. Эти созданный вхождений не сохраняются на сервере без возможности восстановления. Это важно понимать, как поиск элементов календаря определяет, какие сведения о получении и ли расширение происходит.
  
## <a name="recurrence-patterns"></a>Расписания повторения

Основной блок в повторяющееся, который делает возможным расширения — это шаблон повторения. Шаблон повторения найдено в образце повторяющихся и описание набор критериев для расчета вхождений на основе даты и времени образца повторения.
  
**В таблице 1. Шаблоны повторения недоступны**

|**Управляемый API EWS класс**|**Элемент веб-служб Exchange**|**�������**|
|:-----|:-----|:-----|
|[Recurrence.DailyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.dailypattern%28v=exchg.80%29.aspx) <br/> |[DailyRecurrence](http://msdn.microsoft.com/library/0aaf265d-b723-49c6-8e9c-9ba60141e9ab%28Office.15%29.aspx) <br/> |Повторите каждый день.  <br/> Повторите каждый второй день.  <br/> |
|[Recurrence.MonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.monthlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteMonthlyRecurrence](http://msdn.microsoft.com/library/178fa0ae-9dfc-417f-933c-d657d31c2161%28Office.15%29.aspx) <br/> |Повторите ежемесячно в 10 день месяца.  <br/> Повторите каждые два месяца двадцати первый день месяца.  <br/> |
|[Recurrence.RelativeMonthlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativemonthlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeMonthlyRecurrence](http://msdn.microsoft.com/library/a76595db-7460-44ac-ac2a-53241caa33a7%28Office.15%29.aspx) <br/> |Повторите во второй вторник каждого месяца.  <br/> Повторите в третий четверг каждые три месяца.  <br/> |
|[Recurrence.RelativeYearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.relativeyearlypattern%28v=exchg.80%29.aspx) <br/> |[RelativeYearlyRecurrence](http://msdn.microsoft.com/library/25b67876-9979-4a30-a637-357ea10a93b8%28Office.15%29.aspx) <br/> |Повторите в первый понедельник августа каждый год.  <br/> |
|[Recurrence.WeeklyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.weeklypattern%28v=exchg.80%29.aspx) <br/> |[WeeklyRecurrence](http://msdn.microsoft.com/library/69c41dd5-597c-45bc-be3f-e2f2b5615aa3%28Office.15%29.aspx) <br/> |Повторите каждый понедельник.  <br/> Повторите вторникам и четверг каждые две недели.  <br/> |
|[Recurrence.YearlyPattern](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.yearlypattern%28v=exchg.80%29.aspx) <br/> |[AbsoluteYearlyRecurrence](http://msdn.microsoft.com/library/96f53e2c-3893-4f6e-a78a-ac179f45c5db%28Office.15%29.aspx) <br/> |Повторите на 1-го сентября каждый год.  <br/> |
   
Другие важную информацию для шаблона повторения — при завершении повторения. Это может быть выражено как заданное количество вхождений, Дата завершения или необходимости нет конца.
  
**В таблице 2. Параметры для окончания встречи**

|**Управляемый API EWS метод или свойство**|**Элемент веб-служб Exchange**|**Описание**|
|:-----|:-----|:-----|
|[Recurrence.NumberOfOccurrences](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.numberofoccurrences%28v=exchg.80%29.aspx) <br/> |[NumberedRecurrence](http://msdn.microsoft.com/library/53746909-ef21-4764-8715-a7769b943cca%28Office.15%29.aspx) <br/> |Значение этого свойства или элемент указывает число вхождений.  <br/> |
|[Recurrence.EndDate](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.enddate%28v=exchg.80%29.aspx) <br/> |[EndDateRecurrence](http://msdn.microsoft.com/library/a5ee2504-db84-49ee-870c-cca9269f2e26%28Office.15%29.aspx) <br/> |Последнее вхождение в серии попадает на или до даты, указанного идентификатором этого свойства или элемента.  <br/> |
|[Recurrence.HasEnd](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.hasend%28v=exchg.80%29.aspx) <br/> [Recurrence.NeverEnds](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.recurrence.neverends%28v=exchg.80%29.aspx) <br/> |[NoEndRecurrence](http://msdn.microsoft.com/library/ab2ebd9c-388e-45f1-abf9-56e293ef123b%28Office.15%29.aspx) <br/> |Серия имеет нет конца.  <br/> |
   
## <a name="expanded-vs-non-expanded-views"></a>Расширенное и не были развернуты представлений

С помощью метода **FindAppointments** в управляемый API веб-служб Exchange (или операции **FindItem** с элементом **представления календаря** в веб-служб Exchange) вызывает процесса расширения. Это скрывает повторяющихся встреч главных в наборе результатов и вместо этого представляет расширенное представление этого повторяющегося ряда. Вхождения и исключения повторяющихся образец, попадающие в параметры представления календаря включены в наборе результатов. С другой стороны, с помощью метода **FindItems** в управляемый API веб-служб Exchange (или операции **FindItem** с **IndexedPageItemView** или **FractionalPageItemView** элемент в веб-служб Exchange), не вызывает процесса расширения и вхождений и исключения, не включаются. Давайте рассмотрим пример сравнения двух методов. 
  
**В таблице 3. Методы и операций поиска встреч**

|**Метод управляемого API EWS**|**Операция служб EWS**|**При развертывании серии?**|**Компоненты, входящие в результаты**|
|:-----|:-----|:-----|:-----|
|[ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) <br/> |[Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [представления календаря](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx)  <br/> |Да  <br/> |Неповторяющихся встреч, отдельных экземпляров повторяющегося ряда и исключений из серии повторяющихся  <br/> |
|[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) <br/> |[Операция FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) элемент или элемент [FractionalPageItemView](http://msdn.microsoft.com/library/4111afec-35e7-4c6f-b291-9bbba603f633%28Office.15%29.aspx)  <br/> |Нет  <br/> |Неповторяющихся встреч и повторяющихся встреч главной  <br/> |
   
Sadie выполнил установил сын для swim группы. Группа имеет practice каждый день в 8:30:00 утра среда запуск 2 июля с последней, прием на 6 августа. Желающие не забудьте о practice, Sadie добавляет повторяющейся встречи в свой календарь, чтобы напомнить ему.
  
**В таблице 4. Sadie's повторяющейся встречи**

|**Поле встречи**|**Значение**|
|:-----|:-----|
|Subject  <br/> |Swim Practice группы  <br/> |
|Начало  <br/> |2 июля 2014 г. 8:30:00  <br/> |
|End  <br/> |2 июля 2014 г. 10:00 по  <br/> |
|Повторяется  <br/> |Каждую среду  <br/> |
|Последнее вхождение  <br/> |6 августа 2014 г. 8:30:00  <br/> |
   
Краткий обзор календаря показывает, что команда будет иметь всего шесть рекомендациям. Тем не менее не существует шесть элементов различных встречи в календаре. Вместо этого существует только один повторяющейся встречи главной, представляющее серии.
  
Теперь давайте взглянем на поиск встреч в календаре пользователя Sadie, которые происходят в рамках июля. В следующем примере кода метод **FindItems** в управляемый API Exchange для создания представления не были развернуты Sadie элемента календаря. 
  
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

Этот код приводит к следующей запрос [FindItem операции](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) с элементом [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Ответ сервера включает в себя только один элемент, хозяином повторяющихся указанный в параметре значение элемента [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) **RecurringMaster**. Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

Теперь давайте сравнить с расширенное представление. В следующем примере кода метод **FindAppointments** в управляемый API веб-служб Exchange для создания развернутого представления календаря в Sadie. 
  
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

Этот код приводит к следующей [операции FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) запроса с элемент [представления календаря](http://msdn.microsoft.com/library/a4a953b8-0710-416c-95ef-59e51eba9982%28Office.15%29.aspx) . 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Настоящее время отклика сервера включает в себя пять вхождений, другая — для каждого среда июля. Элементы [CalendarItemType](http://msdn.microsoft.com/library/1feb0788-adf7-4a7c-830c-005214ad930f%28Office.15%29.aspx) на все эти элементы имеют значение **экземпляра**. Обратите внимание, что повторяющиеся главных не указан в ответе. Значения элементов [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) URL-были сокращены для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="939" MinorBuildNumber="16" Version="V2_11" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

После того как образцом повторения, вхождения или исключение всегда можно [извлечь связанные элементы](how-to-access-a-recurring-series-by-using-ews-in-exchange.md). Учитывая вхождение или исключение, вы можете получить повторяющихся основной и наоборот.
  
## <a name="working-with-recurring-calendar-items"></a>Работа с повторяющихся элементов календаря

Можно использовать те же операций и методы для работы с серии повторяющихся как для работы с элементами календаря неповторяющейся. Отличие заключается, что в зависимости от того, элемент, который можно использовать для вызова этих методов или операции, выполняемые действия можно применять для всего ряда или только одно вхождение. [Действия, предпринимаемые в образце повторяющихся](how-to-update-a-recurring-series-by-using-ews-in-exchange.md) будут применяться ко все вхождения серии, во время [действия, предпринимаемые для одного экземпляра или исключение](how-to-update-a-recurring-series-by-using-ews.md) применяется только к этому вхождение или исключение. 
  
## <a name="in-this-section"></a>В этом разделе

- [Доступ к ряду с помощью веб-служб Exchange в Exchange](how-to-access-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Создание встречи с помощью веб-служб Exchange в Exchange](how-to-create-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Удаление встреч в серии повторяющихся с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-in-a-recurring-series-by-using-ews-in-exchange.md)
    
- [Обновление серии повторяющихся с помощью веб-служб Exchange](how-to-update-a-recurring-series-by-using-ews.md)
    
- [Обновление серии повторяющихся с помощью веб-служб Exchange в Exchange](how-to-update-a-recurring-series-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    
- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Получение встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md)
    

