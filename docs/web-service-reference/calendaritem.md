---
title: CalendarItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: Элемент CalendarItem представляет элемент Exchange календаря.
ms.openlocfilehash: b8493a54e42df2789be04b2a426c6aff414ec6f2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518864"
---
# <a name="calendaritem"></a>CalendarItem

Элемент **CalendarItem** представляет элемент Exchange календаря. 
  
```XML
<CalendarItem>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <Start/>
   <End/>
   <OriginalStart/>
   <IsAllDayEvent/>
   <LegacyFreeBusyStatus/>
   <Location/>
   <When/>
   <IsMeeting/>
   <IsCancelled/>
   <IsRecurring/>
   <MeetingRequestWasSent/>
   <IsResponseRequested/>
   <CalendarItemType/>
   <MyResponseType/>
   <Organizer/>
   <RequiredAttendees/>
   <OptionalAttendees/>
   <Resources/>
   <ConflictingMeetingCount/>
   <AdjacentMeetingCount/>
   <ConflictingMeetings/>
   <AdjacentMeetings/>
   <Duration/>
   <TimeZone/>
   <AppointmentReplyTime/>
   <AppointmentSequenceNumber/>
   <AppointmentState/>
   <Recurrence/>
   <FirstOccurrence/>
   <LastOccurrence/>
   <ModifiedOccurrences/>
   <DeletedOccurrences/>
   <MeetingTimeZone/>
   <StartTimeZone/>
   <EndTimeZone/>
   <ConferenceType/>
   <AllowNewTimeProposal/>
   <IsOnlineMeeting/>
   <MeetingWorkspaceUrl/>
   <NetShowUrl/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</CalendarItem>
```

 **CalendarItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит родной многоцелевой поток расширения интернет-почты (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет субъект для Exchange элементов и объектов отклика.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень чувствительности элемента.  <br/> |
|[Основной текст](body.md) <br/> |Представляет фактическое содержимое тела сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время, когда элемент в почтовом ящике был получен.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в bytes элемента. Это свойство доступно только для чтения.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, которые определяют категории, к которым относится элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, на который этот элемент является ответом.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку по умолчанию "Избокс".  <br/> |
|[IsDraft](isdraft.md) <br/> |Указывает, был ли элемент еще не отправлен.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемент ему или себе.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, был ли элемент изменен.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заглавных сообщений в Интернете, содержащихся в элементе в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время, когда был отправлен элемент в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Этот элемент используется [элементом ReminderMinutesBeforeStart](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлено ли напоминание для элемента в Exchange магазине.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Представляет строку отображения, используемую для содержимого строки Cc. Это совмещенная строка всех имен отображения получателей Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Представляет строку отображения, используемую для содержимого строки To. Это конкаентированная строка всех имен отображения получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое настроено на **верное,** если элемент имеет хотя бы одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет культуру для данного элемента в почтовом ящике.  <br/> |
|[UID](uid.md) <br/> |Определяет элемент календаря.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Используется для определения определенного экземпляра повторяющегося элемента календаря.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
|[Start](start.md) <br/> |Представляет начало элемента календаря. Этот элемент применяется только к одному появлению элемента календаря.  <br/> |
|[End ](end-ex15websvcsotherref.md) <br/> |Представляет собой конец продолжительности. Этот элемент применяется только к одному появлению элемента календаря.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Представляет исходное время начала элемента календаря.  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |Указывает, является ли элемент календаря или запрос собрания событием на весь день.  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |Представляет состояние свободного или занятого элемента календаря.  <br/> |
|[Location](location.md) <br/> |Представляет расположение собрания или встречи.  <br/> |
|[When](when.md) <br/> |Предоставляет сведения о том, когда происходит элемент календаря.  <br/> |
|[IsMeeting](ismeeting.md) <br/> |Указывает, является ли элемент календаря собранием или встречей.  <br/> |
|[IsCancelled](iscancelled.md) <br/> |Указывает, отменена ли встреча или собрание.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Указывает, является ли элемент календаря частью повторяющегося элемента. Этот элемент доступен только для чтения.  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |Указывает, был ли отправлен запрос на собрание запрашиваемой участникам.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Указывает, требуется ли ответ на элемент.  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |Представляет тип возникновения элемента календаря.  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |Содержит состояние или ответ на элемент календаря.  <br/> |
|[Organizer](organizer.md) <br/> |Представляет организатор собрания.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые должны присутствовать на собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не обязаны присутствовать на собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Представляет запланированный ресурс для собрания.  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |Представляет количество собраний, которые конфликтуют с элементом календаря.  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |Представляет общее число элементов календаря, примыкающих к времени собрания.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтуя со временем собрания.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описывает все элементы календаря, которые примыкают к времени собрания.  <br/> |
|[Duration (Items)](duration-items.md) <br/> |Представляет продолжительность элемента календаря.  <br/> |
|[TimeZone (Item)](timezone-item.md) <br/> |Предоставляет текстовое описание часового пояса.  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |Представляет дату и время, когда участник ответил на запрос собрания.  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |Указывает номер последовательности версии встречи.  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |Указывает состояние встречи.  <br/> |
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и запросов на собрания.  <br/> Этот элемент действителен, [если значение CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первое появление повторяющегося элемента календаря.  <br/> Этот элемент действителен, [если значение CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнее появление повторяющегося элемента календаря.  <br/> Этот элемент действителен, [если значение CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Содержит массив повторяющихся событий элементов календаря, которые были изменены таким образом, чтобы они отличались от элемента master повторения.  <br/> Этот элемент действителен, [если значение CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Содержит массив удаленных случаев повторяющегося элемента календаря.  <br/> Этот элемент действителен, [если значение CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |Представляет часовой пояс расположения, где проходит собрание.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Представляет часовой пояс начала элемента календаря.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Представляет конечный часовой пояс элемента календаря.  <br/> |
|[ConferenceType](conferencetype.md) <br/> |Описывает тип conferencing, выполняемый с элементом календаря.  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |Указывает, может ли участник использовать новое время собрания для собрания.  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |Указывает, является ли собрание интерактивным.  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |Содержит URL-адрес рабочей области собрания, связанной с элементом календаря.  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Указывает URL-адрес собрания Microsoft NetShow в Интернете.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит имя отображения последнего пользователя, который должен изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает, когда элемент был изменен в последний раз.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для одновременного Microsoft Office Outlook конечной точки веб-приложения для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для одновременного Microsoft Office Outlook конечной точки веб-приложения для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или простой текст, который представляет уникальное тело этого разговора.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описывает все элементы календаря, которые примыкают к времени собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Определяет данные для приложения к одному свойству элемента или папки во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтуя со временем собрания.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Определяет одну папку, создаемую в локальном клиентской магазине.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, идентифицированной элементом [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном клиентской магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом календаря, элемент [MeetingTimeZone](meetingtimezone.md) необходимо указать, чтобы сохранить исходный часовой пояс элемента календаря. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
  
[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

