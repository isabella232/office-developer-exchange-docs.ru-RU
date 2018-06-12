---
title: MeetingRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingRequest
api_type:
- schema
ms.assetid: c44f8804-a355-473d-a837-48cc91617251
description: Элемент MeetingRequest представляет приглашения на собрание в хранилище Exchange.
ms.openlocfilehash: 3e290613293cb6ad1563912e5015742ffc503d08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834450"
---
# <a name="meetingrequest"></a>MeetingRequest

Элемент **MeetingRequest** представляет приглашения на собрание в хранилище Exchange. 
  
```xml
<MeetingRequest>
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
   <Importance/>
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
   <Sender/>
   <ToRecipients/>
   <CcRecipients/>
   <BccRecipients/>
   <IsReadReceiptRequested/>
   <IsDeliveryReceiptRequested/>
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <IsResponseRequested/>
   <References/>
   <ReplyTo/>
   <AssociatedCalendarItemId/>
   <IsDelegated/>
   <IsOutOfDate/>
   <HasBeenProcessed/>
   <ResponseType/>
   <MeetingRequestType/>
   <IntendedFreeBusyStatus/>
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
</MeetingRequest>
```

 **MeetingRequestMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит собственный поток Multipurpose Internet Mail Extensions (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Subject](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объекты ответа. Тема ограничена 255 символов.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Указывает уровень конфиденциальности для элемента.  <br/> |
|[Body](body.md) <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах элемента. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет набор строк, чтобы указать, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, к которому этот элемент является ее в ответ.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, является ли элемент был отправлен исходящие папке по умолчанию.  <br/> |
|[IsDraft](isdraft.md) <br/> |Указывает, является ли элемент еще не были отправлены.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Показывает пользователя отправить элемент на себя.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, является ли элемент ранее еще был отправлен.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, были ли изменены элемента.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, содержащиеся внутри элемента в почтовом ящике.  <br/> |
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
|[Отправитель](sender.md) <br/> |Идентифицирует отправителя элемента.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит список получателей сообщения.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые будут получать копии сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей скрытой копии (СК) сообщения электронной почты.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Указывает, будет ли отправителя элемента о прочтении.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Указывает, требует ли отправитель элемента уведомление о доставке.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет получателя, у которого было отправлено сообщение.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения Интернета элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, имеет ли чтение сообщения.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Указывает, запрашивается ли ответ на сообщение электронной почты.  <br/> |
|[Справочные материалы](references.md) <br/> |Представляет заголовок групп, используемый для сопоставления ответов с исходными сообщениями.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет набор адресов, к которым будут отправляться ответы.  <br/> |
|[AssociatedCalendarItemId](associatedcalendaritemid.md) <br/> |Представляет элемент календаря, связанного с [MeetingMessage](meetingmessage.md).  <br/> |
|[IsDelegated](isdelegated.md) <br/> |Указывает, обработано ли собрания с помощью учетной записи с доступом к делегата.  <br/> |
|[IsOutOfDate](isoutofdate.md) <br/> |Указывает, является ли устаревший сообщения о собрании.  <br/> |
|[HasBeenProcessed](hasbeenprocessed.md) <br/> |Указывает ли сообщение собрания элемент обработки.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип получателя ответа, полученные на собрание.  <br/> |
|[MeetingRequestType](meetingrequesttype.md) <br/> |Описывает тип приглашения на собрание.  <br/> |
|[IntendedFreeBusyStatus](intendedfreebusystatus.md) <br/> |Представляет предполагаемая состояния для элемента календаря, который связан с приглашения на собрание.  <br/> |
|[Start](start.md) <br/> |Представляет начало элемента календаря. Этот элемент применяется только для одного экземпляра элемента календаря.  <br/> |
|[End](end-ex15websvcsotherref.md) <br/> |Представляет конец длительность. Этот элемент применяется только для одного экземпляра элемента календаря.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Представляет исходное время начала элемента календаря.  <br/> |
|[IsAllDayEvent](isalldayevent.md) <br/> |Указывает тип календаря элемента или приглашения на собрание событием на целый день.  <br/> |
|[LegacyFreeBusyStatus](legacyfreebusystatus.md) <br/> |Представляет состояния занятости элемента календаря.  <br/> |
|[Location](location.md) <br/> |Представляет место собрания или встречи.  <br/> |
|[Когда](when.md) <br/> |Представлено описание при возникновении собрания.  <br/> |
|[IsMeeting](ismeeting.md) <br/> |Указывает, является ли элемент календаря собрания или встречи.  <br/> |
|[IsCancelled](iscancelled.md) <br/> |Указывает, была ли отменена встречи или собрания.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Указывает, является ли элемент календаря часть повторяющегося элемента. Этот элемент доступен только для чтения.  <br/> |
|[MeetingRequestWasSent](meetingrequestwassent.md) <br/> |Указывает, был ли отправлен приглашения на собрание запрошенные участникам.  <br/> |
|[CalendarItemType](calendaritemtype.md) <br/> |Представляет тип вхождение элемента календаря.  <br/> |
|[MyResponseType](myresponsetype.md) <br/> |Содержит состояние или ответа на элемент календаря.  <br/> |
|[Организатор](organizer.md) <br/> |Представляет организатора собрания.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые необходимы на участие в собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не требуется на участие в собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Ресурс запланированного собрания.  <br/> |
|[ConflictingMeetingCount](conflictingmeetingcount.md) <br/> |Представляет число собраний, конфликтующие с приглашения на собрание.  <br/> |
|[AdjacentMeetingCount](adjacentmeetingcount.md) <br/> |Представляет общее число элементов календаря, расположенных на время собрания.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
|[Продолжительность (элементы)](duration-items.md) <br/> |Представляет длительность элемента календаря.  <br/> |
|[Часовой пояс (элемент)](timezone-item.md) <br/> |Предоставляет текстовое описание часового пояса.  <br/> |
|[AppointmentReplyTime](appointmentreplytime.md) <br/> |Представляет дату и время, когда участник дан ответ на приглашения на собрание.  <br/> |
|[AppointmentSequenceNumber](appointmentsequencenumber.md) <br/> |Указывает порядковый номер версии встречи.  <br/> |
|[AppointmentState](appointmentstate.md) <br/> |Указывает состояние встречи.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашения на собрания.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первого появления повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнего вхождения повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Содержит массив повторяющихся вхождения элемента календаря, которые были изменены, отличного от элемента шаблона повторения.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[DeletedOccurrences](deletedoccurrences.md) <br/> |Содержит массив удаленных вхождения повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.  <br/> |
|[MeetingTimeZone](meetingtimezone.md) <br/> |Представляет часовой пояс расположение, где размещен собрания.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Представляет часовой пояс Пуск элемента календаря.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Представляет часовой пояс конечных элемента календаря.  <br/> |
|[ConferenceType](conferencetype.md) <br/> |Описывает тип конференц-связи, выполняемую с элементом календарь.  <br/> |
|[AllowNewTimeProposal](allownewtimeproposal.md) <br/> |Представляет ли собрание можно предложенное собрание.  <br/> |
|[IsOnlineMeeting](isonlinemeeting.md) <br/> |Указывает, является ли online собрания.  <br/> |
|[MeetingWorkspaceUrl](meetingworkspaceurl.md) <br/> |Содержит URL-адрес для рабочей области для собраний, которая связана с элемента календаря.  <br/> |
|[NetShowUrl](netshowurl.md) <br/> |Указывает URL-адрес для Microsoft Netshow собрание по сети.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит правами клиент, построенный на параметры разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, является ли элемент связан с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.  <br/> |
|[ИД ПОЛЬЗОВАТЕЛЯ](uid.md) <br/> |Идентифицирует элемент календаря.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Используется для идентификации определенный экземпляр повторяющегося элемента календаря.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Определяет все элементы календаря, расположенных на время собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[Создание (ItemSync)](create-itemsync.md) <br/> |Определяет один элемент для создания в локальном хранилище клиента.  <br/> |
|[Элементы](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет отдельное свойство элемента в [UpdateItem операции](updateitem-operation.md)обновления.  <br/> |
|[Обновление (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

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

