---
title: Часовые пояса и веб-службах Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 0e0a666c-0541-414b-a7fb-297d94f692e6
description: Узнайте, как часовые пояса работают с управляемый API EWS и веб-служб Exchange в Exchange.
ms.openlocfilehash: fcc8b00acf2b63de04718e13b82191de95bbf2b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761253"
---
# <a name="time-zones-and-ews-in-exchange"></a>Часовые пояса и веб-службах Exchange

Узнайте, как часовые пояса работают с управляемый API EWS и веб-служб Exchange в Exchange.
  
Часовые пояса не то, что большинство пользователей предоставить намного определиться. Тем не менее они важные концепции при указании даты и времени с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange. Неправильным часовые пояса в управляемый API EWS или веб-служб Exchange приложение может привести к непредсказуемым последствиям. Обработка часовых поясах должным образом, можно легко до тех пор, пока вы знаете, как.
  
## <a name="handling-time-zones-in-the-ews-managed-api"></a>Обработка часовые пояса в управляемый API веб-служб Exchange

Если вы используете управляемый API веб-служб Exchange, часовые пояса в большинстве случаев обрабатываются для вас автоматически. Без каких-либо явных действий со стороны пользователя API использует локальный часовой пояс клиентского компьютера и все необходимые преобразование в фоновом режиме. Это очень полезно при нужную влияние, но у вас есть другие параметры.
  
Один из вариантов — это задание для свойства [ExchangeService.TimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) . Это свойство определяет часовой пояс для всех запросов, выполняемых с управляемый API веб-служб Exchange. Это свойство доступно только для чтения; Единственный способ его настройка — через конструктор класса. Если вы используете [ExchangeService(System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd635875%28v=exchg.80%29.aspx) или конструктор [ExchangeService (ExchangeVersion, System.TimeZoneInfo)](http://msdn.microsoft.com/en-us/library/dd636248%28v=exchg.80%29.aspx) , как объект [System.TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx) можно указать конкретного часового пояса. Если вы используете один из других конструкторов, не вступят в качестве параметра объекта **TimeZoneInfo** , класс **ExchangeService** задает свойство **часового пояса** для текущего часового пояса на клиентском компьютере. 
  
Ли задание конкретного часового пояса, или оставьте его как часовой пояс клиентского компьютера, все даты и время выражаются в часовом поясе, представленный свойством **часового пояса** . Управляемый API веб-служб Exchange предоставляет все свойства даты и времени как [System.DateTime](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx) структуры. Поэтому если выбрать все свойства даты и времени быть нельзя, что времени, заданного обрабатывается в соответствии со значением свойства [DateTime.Kind](http://msdn.microsoft.com/en-us/library/system.datetime.kind%28v=vs.110%29.aspx) объекта **даты и времени** . Если значение свойства **Тип** **не определен**, значение **даты и времени** интерпретируется как в часовом поясе, указанном свойством **часового пояса** . Если вы читаете свойства даты и времени, все свойства **даты и времени** выраженная в этого часового пояса. 
  
При [создании новой встречи или собрания](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md) или [обновлении существующей встречи или собрания](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md), у вас есть возможность переопределить часовой пояс, указанных в **часовой пояс** для новых объектов [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) . Тем не менее именно то, что можно переопределить зависит от [версии схемы веб-служб Exchange](ews-schema-versions-in-exchange.md) , вы используете. Для всех значения свойства [ExchangeService.RequestedServerVersion](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.requestedserverversion%28v=exchg.80%29.aspx) можно задать [Appointment.StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) для использования конкретного часового пояса для встречи или собрания. Если вы используете значение для свойства **ExchangeService.RequestedServerVersion** , больше, чем **Exchange2007_SP1**, можно также свойство [Appointment.EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) , что позволяет указать часовой пояс для [ Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) свойство. Тем не менее иметь в виду, что эти свойства только влияет на интерпретацию даты и времени для создания запроса. Если получить встречу, время начала и окончания по-прежнему быть выражены в часовом поясе, указанном свойством **часового пояса** . 
  
При обновлении существующей встречи или собрания, можно изменить часовой пояс для объекта **встречи** , задав свойство **StartTimeZone** и/или свойство **EndTimeZone** . Это приведет к применимых раз перенести соответствующим образом. Если выбрать **ExchangeService.RequestedServerVersion** для **Exchange2007_SP1**не удается задать свойство **EndTimeZone** ; Вместо него будет использоваться значение свойства **StartTimeZone** . 
  
**В таблице 1. Свойства часового пояса в управляемый API веб-служб Exchange**

|**Свойства часового пояса**|**Версия минимальные сервера запросов**|**Описание**|
|:-----|:-----|:-----|
|[Часовой пояс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.timezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Если не установить их при помощи конструктор класса **ExchangeService** этому свойству присвоено часовой пояс клиентского компьютера. Все свойства **даты и времени** , при создании элементов и при получении существующих элементов выражаются в данном часовом поясе. Зона может быть переопределен в этот раз создания запросов для встречи и собрания по **Appointment.StartTimeZone** и/или свойство **Appointment.EndTimeZone** . Если не переопределено свойство **Appointment.StartTimeZone** , этот часовой пояс считается создания часовой пояс для собраний и встреч.  <br/> |
|[StartTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.starttimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2007_SP1** <br/> |Если задать новые объекты **встречи** , этот часовой пояс используется для интерпретации свойства [Appointment.Start](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.start%28v=exchg.80%29.aspx) и [Appointment.ReminderDueBy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.reminderdueby%28v=exchg.80%29.aspx) . Этот часовой пояс рассматривается создание часовой пояс для объекта **встречи** .  <br/> При получении существующих элементов, это свойство является информационным только. Значения свойств **даты и времени** в существующую встречу всегда отображаются в часовом поясе, указанном свойством **ExchangeService.TimeZone** .  <br/> |
|[EndTimeZone](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.endtimezone%28v=exchg.80%29.aspx) <br/> |**Exchange2010** <br/> |Если задать новые объекты **встречи** , этот часовой пояс используется для интерпретации свойство [Appointment.End](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.end%28v=exchg.80%29.aspx) .  <br/> При получении существующих элементов, это свойство является информационным только. Значения свойств **даты и времени** в существующую встречу всегда отображаются в часовом поясе, указанном свойством **ExchangeService.TimeZone** .  <br/> |
   
## <a name="handling-time-zones-in-ews"></a>Обработка часовые пояса в веб-служб Exchange

Если вы используете веб-служб Exchange, часовые пояса не обрабатывается для вас автоматически и обстоятельства немного сложнее. Как часовые пояса повысить EWS запросы и ответы зависит от нескольких факторов:
  
- Версия Exchange, заданная в элементе [RequestServerVersion](http://msdn.microsoft.com/library/af4032d5-42b3-463e-9d0a-8236d78e5b75%28Office.15%29.aspx) 
    
- Часовой пояс, заданная в элементе [TimeZoneContext](http://msdn.microsoft.com/library/573c462b-aa1d-4ba0-8852-e3f48b26873b%28Office.15%29.aspx) (если имеется) 
    
- Часовой пояс, указанный в [MeetingTimeZone](http://msdn.microsoft.com/library/413b47d9-8126-462c-9a4f-4e771a5e8889%28Office.15%29.aspx), [StartTimeZone](http://msdn.microsoft.com/library/d38c4dc1-4ecb-42a1-8d57-a451b16a2de2%28Office.15%29.aspx)или [EndTimeZone](http://msdn.microsoft.com/library/6c53c337-be60-4d22-9e9e-a0c140c5e913%28Office.15%29.aspx) элементы (если есть на встречи или собрания) 
    
- Часовой пояс, указанного в XML-элементы **даты и времени** (при его наличии) 
    
Часовой пояс, указанных в значение **даты и времени** элементов может иметь три формы. Могут читать все сведения в [схему XML, часть 2: типы данных Second Edition](http://www.w3.org/TR/xmlschema-2/#dateTime), но Перефразируя:
  
- **Скоординированному времени (UTC):** Заданный параметром «Z». Например`2014-06-06T19:00:00.000Z`
    
- **Конкретного часового пояса:** Определяется «+» или "-" следуют часов и минут. Например`2014-06-06T19:00:00.000-08:00`
    
- **Без часового пояса:** Указанной отсутствия любого часового пояса. Например`2014-06-06T19:00:00.000`
    
Если часовой пояс присутствует в значение **даты и времени** (UTC или конкретного часового пояса), это значение всегда считается этого часового пояса. При наличии без часового пояса Интерпретация значение зависит от конкретный набор другие элементы связанных с ними часового пояса. 
  
**В таблице 2. Часовой пояс элементов в веб-служб Exchange и их эффекты**

|**RequestServerVersion**|**Этот параметр указан TimeZoneContext?**|**MeetingTimeZone, StartTimeZone или EndTimeZone представить (элемента календаря, имеющего и только MeetingRequest)?**|**даты и времени в формате UTC**|**даты и времени в конкретного часового пояса**|**даты и времени без часового пояса**|**Часовой пояс создания встречи и собрания**|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|**Exchange2007_SP1** <br/> |Да  <br/> |Да ( **MeetingTimeZone** )  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Элементы внутри [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) элемента, который содержит элемент **MeetingTimeZone** обрабатываются как часовой пояс в элементе **MeetingTimeZone** , все остальные как UTC  <br/> |Часовой пояс в элементе **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Да  <br/> |Нет  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Как UTC  <br/> |UTC  <br/> |
|**Exchange2007_SP1** <br/> |Нет  <br/> |Да ( **MeetingTimeZone** )  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Элементы внутри [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) элемента, который содержит элемент **MeetingTimeZone** обрабатываются как часовой пояс в элементе **MeetingTimeZone** , все остальные как UTC  <br/> |Часовой пояс в элементе **MeetingTimeZone**  <br/> |
|**Exchange2007_SP1** <br/> |Нет  <br/> |Нет  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Как UTC  <br/> |UTC  <br/> |
|**Файл Exchange2010** и более поздних версий  <br/> |Да  <br/> |Да ( **StartTimeZone** и/или **EndTimeZone** )  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |При наличии элемент **StartTimeZone** значение [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и элементы [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) интерпретируются как часовой пояс в элементе **StartTimeZone** . В противном случае — значение этих элементов интерпретируются как часовой пояс в элементе **TimeZoneContext** .  <br/> При наличии элемент **EndTimeZone** значение элемента [запустите](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) интерпретируется как часовой пояс в элементе **EndTimeZone** . В противном случае — значение **конечного** элемента считается часовой пояс в элементе **TimeZoneContext** .  <br/> Элементы за пределами [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) интерпретируются как часовой пояс в элементе **TimeZoneContext** .  <br/> |Часовой пояс в элементе **StartTimeZone** , если этот параметр указан, часового пояса в элементе **TimeZoneContext** , если это не так  <br/> |
|**Файл Exchange2010** и более поздних версий  <br/> |Да  <br/> |Нет  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Как часовой пояс в элементе **TimeZoneContext**  <br/> |Часовой пояс в элементе **TimeZoneContext**  <br/> |
|**Файл Exchange2010** и более поздних версий  <br/> |Нет  <br/> |Да ( **StartTimeZone** и/или **EndTimeZone** )  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |При наличии элемент **StartTimeZone** значение [Start](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) и элементы [ReminderDueBy](http://msdn.microsoft.com/library/e28a0485-86af-4a4e-a2ba-3ad2d4ebff6f%28Office.15%29.aspx) интерпретируются как часовой пояс в элементе **StartTimeZone** . В противном случае — значение этих элементов интерпретируются как UTC.  <br/> При наличии элемент **EndTimeZone** значение элемента [запустите](http://msdn.microsoft.com/library/7cfe9979-c893-4f9b-b3a1-8f9e17515a4b%28Office.15%29.aspx) интерпретируется как часовой пояс в элементе **EndTimeZone** . В противном случае — значение **конечного** элемента считается UTC.  <br/> Элементы за пределами [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) или [MeetingRequest](http://msdn.microsoft.com/library/c44f8804-a355-473d-a837-48cc91617251%28Office.15%29.aspx) интерпретируются как UTC.  <br/> |Часовой пояс в элементе **StartTimeZone** , если этот параметр указан, UTC, если это не так  <br/> |
|**Файл Exchange2010** и более поздних версий  <br/> |Нет  <br/> |Нет  <br/> |Как UTC  <br/> |Как часовой пояс, указанные в значение  <br/> |Как UTC  <br/> |UTC  <br/> |
   
При интерпретации ответов с сервера, следует всегда проверять значение каждого элемента и интерпретации значения соответствующим образом. Exchange в значение всегда будут включены часового пояса (UTC или конкретного часового пояса).
  
## <a name="additional-time-zone-considerations-when-creating-appointments-and-meetings"></a>Сведения о выполнении дополнительных часовой пояс при создании встречи и собрания

При создании встречи или собрания, часовой пояс, который применяется к времени начала считается создания часовой пояс для встречи. Помимо Интерпретация date/times при создании встречи или собрания, часовой пояс создания имеет следующие эффекты для элемента:
  
- Если элемент является событием на целый день, он может показывать каким-либо образом при просмотре из клиента, с помощью различных часовой пояс, чем создания часового пояса. Это, так как [при создании событием на целый день](how-to-create-all-day-events-by-using-ews-in-exchange.md), время начала и окончания целый день событий настроены на полночь создания часового пояса. Это время будет показывать в качестве времени, отличный от полуночи в часовом поясе, поэтому элемент может отображаться охватывать дополнительных дней. Таким образом мы рекомендуем использовать часовой пояс, настроенных для основного календаря клиент пользователя для создания событий на целый день, когда это возможно.
    
- Если элемент собрания, часовой пояс создания отображается в панель информации Outlook на приглашения на собрания, получаемые участников, если этот часовой пояс отличается от часового пояса их клиента.
    
## <a name="in-this-section"></a>В этом разделе

- [Создание встречи в конкретного часового пояса с помощью веб-служб Exchange в Exchange](how-to-create-appointments-in-a-specific-time-zone-by-using-ews-in-exchange.md)
    
- [Обновление часового пояса для встречи с помощью веб-служб Exchange в Exchange](how-to-update-the-time-zone-for-an-appointment-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также


- [Разработка клиентов веб-служб для Exchange](develop-web-service-clients-for-exchange.md)
    
- [Версии схемы веб-служб Exchange в Exchange](ews-schema-versions-in-exchange.md)
    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)
    
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)
    
- [Создание событий на целый день с помощью веб-служб Exchange в Exchange](how-to-create-all-day-events-by-using-ews-in-exchange.md)
    
- [Структура даты и времени](http://msdn.microsoft.com/en-us/library/system.datetime%28v=vs.110%29.aspx)
    
- [Класс TimeZoneInfo](http://msdn.microsoft.com/en-us/library/system.timezoneinfo%28v=vs.110%29.aspx)
    

