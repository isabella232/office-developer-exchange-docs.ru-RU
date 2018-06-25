---
title: Элемента календаря, имеющего
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarItem
api_type:
- schema
ms.assetid: b0c1fd27-b6da-46e5-88b8-88f00c71ba80
description: Элемент элемента календаря, имеющего представляет собой элемент календаря Exchange.
ms.openlocfilehash: c7b6d4930bc42fbe26d35264e2eae0c986cc8db7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761648"
---
# <a name="calendaritem"></a>Элемента календаря, имеющего

Элемент **элемента календаря, имеющего** представляет собой элемент календаря Exchange. 
  
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
|[MimeContent](mimecontent.md) <br/> |Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Subject](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объекты ответа.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Указывает уровень конфиденциальности для элемента.  <br/> |
|[Body](body.md) <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах элемента. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет набор строк, которые определяют категории, к которым принадлежит элемент в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, к которому этот элемент является ее в ответ.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, является ли элемент был отправлен исходящие папке по умолчанию.  <br/> |
|[IsDraft](isdraft.md) <br/> |Указывает, является ли элемент еще не были отправлены.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемента для его сами себя.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, является ли элемент ранее еще был отправлен.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, были ли изменены элемента.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, содержащихся в элемента в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, которые связаны с элемента в хранилище Exchange.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Используется в элементе [ReminderMinutesBeforeStart](reminderminutesbeforestart.md) определить, когда отображается оповещение.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлен ли напоминания для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет число минут и только потом событие, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Строка отображения, который используется для содержимого строку "Копия". Это составное строка всех получателей отображаемые имена «копия».  <br/> |
|[DisplayTo](displayto.md) <br/> |Строка отображения, который используется для содержимого строке. Это составное строка всех для получателей отображаемые имена.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере один видимым вложения. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Язык и региональные параметры](culture.md) <br/> |Представляет язык и региональные параметры для заданного элемента в почтовом ящике.  <br/> |
|[ИД ПОЛЬЗОВАТЕЛЯ](uid.md) <br/> |Идентифицирует элемент календаря.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Используется для идентификации определенный экземпляр повторяющегося элемента календаря.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
|[Start](start.md) <br/> |Представляет начало элемента календаря. Этот элемент применяется только для одного экземпляра элемента календаря.  <br/> |
|[End](end-ex15websvcsotherref.md) <br/> |Представляет конец длительность. Этот элемент применяется только для одного экземпляра элемента календаря.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Представляет исходное время начала элемента календаря.  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |Указывает тип календаря элемента или приглашения на собрание событием на целый день.  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |Представляет состояния занятости элемента календаря.  <br/> |
|[Location](location.md) <br/> |Представляет место собрания или встречи.  <br/> |
|[Когда](when.md) <br/> |Предоставляет сведения о при возникновении элемента календаря.  <br/> |
|[IsMeeting](ismeeting.md) <br/> |Указывает, является ли элемент календаря собрания или встречи.  <br/> |
|[IsCancelled](iscancelled.md) <br/> |Указывает, была ли отменена встречи или собрания.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Указывает, является ли элемент календаря часть повторяющегося элемента. Этот элемент доступен только для чтения.  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |Указывает, был ли отправлен приглашения на собрание запрошенные участникам.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Указывает, требуется ли ответа на элемент.  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |Представляет тип вхождение элемента календаря.  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |Содержит состояние или ответа на элемент календаря.  <br/> |
|[Организатор](organizer.md) <br/> |Представляет организатора собрания.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые необходимы на участие в собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не требуется на участие в собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Ресурс запланированного собрания.  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |Представляет число собраний, конфликтующие с элемента календаря.  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |Представляет общее число элементов календаря, расположенных на время собрания.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
|[Продолжительность (элементы)](duration-items.md) <br/> |Представляет длительность элемента календаря.  <br/> |
|[Часовой пояс (элемент)](timezone-item.md) <br/> |Предоставляет текстовое описание часового пояса.  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |Представляет дату и время, когда участник дан ответ на приглашения на собрание.  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |Указывает порядковый номер версии встречи.  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |Указывает состояние встречи.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашения на собрания.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первого появления повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнего вхождения повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Содержит массив повторяющихся вхождения элемента календаря, которые были изменены, чтобы они отличаются от элемента шаблона повторения.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Содержит массив удаленных вхождения повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |Представляет часовой пояс расположение, где размещен собрания.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Представляет часовой пояс Пуск элемента календаря.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Представляет часовой пояс конечных элемента календаря.  <br/> |
|[ConferenceType](conferencetype.md) <br/> |Описывает тип конференц-связи, выполняемую с элементом календарь.  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |Указывает, можно ли участником предлагаться собрание для собрания.  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |Указывает, является ли online собрания.  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |Содержит URL-адрес для рабочей области для собраний, которая связана с элемента календаря.  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Указывает URL-адрес для Microsoft NetShow собрание по сети.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, является ли элемент связан с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[Создание (ItemSync)](create-itemsync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[Элементы](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, указанной с помощью элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[Обновление (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

При обновлении элемента одного календаря стать повторяющегося элемента календаря главной [MeetingTimeZone](meetingtimezone.md) элемент должен быть указан для сохранения часового пояса исходного элемента календаря. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
  
[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

