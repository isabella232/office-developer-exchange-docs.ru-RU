---
title: календаритем
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
description: Элемент Календаритем представляет элемент календаря Exchange.
ms.openlocfilehash: b29141470d157ef5bd67be06a1e1fa1c9536b042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529485"
---
# <a name="calendaritem"></a>календаритем

Элемент **календаритем** представляет элемент календаря Exchange. 
  
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

 **календаритемтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сохранитьmimecontent](mimecontent.md) <br/> |Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения для элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объектов ответа.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень конфиденциальности элемента.  <br/> |
|[Body](body.md) <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, вложенные в элемент в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер элемента в байтах. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[инреплито](inreplyto.md) <br/> |Представляет идентификатор элемента, который является ответом на этот элемент.  <br/> |
|[Отправлено](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку "Исходящие" по умолчанию.  <br/> |
|[Черновик](isdraft.md) <br/> |Указывает, был ли элемент еще не отправлен.  <br/> |
|[исфромме](isfromme.md) <br/> |Указывает, отправляет ли пользователь элемент.  <br/> |
|[исресенд](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[исунмодифиед](isunmodified.md) <br/> |Указывает, был ли изменен элемент.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заголовков сообщений Интернета, которые находятся в элементе почтового ящика.  <br/> |
|[датетимесент](datetimesent.md) <br/> |Представляет дату и время отправки элемента в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания определенного элемента в почтовом ящике.  <br/> |
|[респонсеобжектс](responseobjects.md) <br/> |Содержит коллекцию всех объектов ответа, связанных с элементом в хранилище Exchange.  <br/> |
|[реминдердуеби](reminderdueby.md) <br/> |Представляет дату и время возникновения события. Он используется элементом [реминдерминутесбефорестарт](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[реминдериссет](reminderisset.md) <br/> |Указывает, задано ли напоминание для элемента в хранилище Exchange.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события при отображении напоминания.  <br/> |
|[дисплайкк](displaycc.md) <br/> |Представляет отображаемую строку, используемую для содержимого строки "копия". Это объединенная строка всех отображаемых имен получателей копии.  <br/> |
|[дисплайто](displayto.md) <br/> |Представляет отображаемую строку, используемую для содержимого строки "Кому". Это объединенная строка для отображаемых имен получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, для которого задано значение **true** , если элемент имеет по крайней мере одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет язык и региональные параметры для определенного элемента в почтовом ящике.  <br/> |
|[UID](uid.md) <br/> |Определяет элемент календаря.  <br/> |
|[рекурренцеид](recurrenceid.md) <br/> |Используется для идентификации определенного экземпляра повторяющегося элемента календаря.  <br/> |
|[датетиместамп](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
|[Начало](start.md) <br/> |Представляет начало элемента календаря. Этот элемент применяется только к одному экземпляру элемента календаря.  <br/> |
|[Оканчиваться](end-ex15websvcsotherref.md) <br/> |Представляет конец длительности. Этот элемент применяется только к одному экземпляру элемента календаря.  <br/> |
|[оригиналстарт](originalstart.md) <br/> |Представляет исходное время начала элемента календаря.  <br/> |
|[исаллдайевент](isalldayevent.md) <br/> |Указывает, представляет ли элемент календаря или приглашение на собрание событие на целый день.  <br/> |
|[легацифрибусистатус](legacyfreebusystatus.md) <br/> |Представляет состояние занятости элемента календаря.  <br/> |
|[Location](location.md) <br/> |Представляет место собрания или встречи.  <br/> |
|[Когда](when.md) <br/> |Предоставляет сведения о том, когда встречается элемент календаря.  <br/> |
|["Собрание"](ismeeting.md) <br/> |Указывает, является ли элемент календаря собранием или встречей.  <br/> |
|[С отменой](iscancelled.md) <br/> |Указывает, отменена ли встреча или собрание.  <br/> |
|[IsRecurring](isrecurring.md) <br/> |Указывает, является ли элемент календаря частью повторяющегося элемента. Этот элемент доступен только для чтения.  <br/> |
|[митингрекуествассент](meetingrequestwassent.md) <br/> |Указывает, было ли приглашение на собрание отправлено запрошенным участникам.  <br/> |
|[исреспонсерекуестед](isresponserequested.md) <br/> |Указывает, требуется ли ответ на элемент.  <br/> |
|[календаритемтипе](calendaritemtype.md) <br/> |Представляет тип вхождения элемента календаря.  <br/> |
|[миреспонсетипе](myresponsetype.md) <br/> |Содержит состояние или ответ на элемент календаря.  <br/> |
|[Organizer](organizer.md) <br/> |Представляет организатор собрания.  <br/> |
|[RequiredAttendees](requiredattendees.md) <br/> |Представляет участников, которые необходимы для участия в собрании.  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |Представляет участников, которые не являются обязательными для участия в собрании.  <br/> |
|[Ресурсы](resources.md) <br/> |Представляет запланированный ресурс для собрания.  <br/> |
|[конфликтингмитингкаунт](conflictingmeetingcount.md) <br/> |Представляет количество собраний, которые конфликтуют с элементом календаря.  <br/> |
|[аджацентмитингкаунт](adjacentmeetingcount.md) <br/> |Представляет общее число элементов календаря, смежных с временем собрания.  <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуют с временем собрания.  <br/> |
|[аджацентмитингс](adjacentmeetings.md) <br/> |Описывает все элементы календаря, смежные с временем собрания.  <br/> |
|[Длительность (элементы)](duration-items.md) <br/> |Представляет продолжительность элемента календаря.  <br/> |
|[Часовой пояс (элемент)](timezone-item.md) <br/> |Содержит текст описания часового пояса.  <br/> |
|[аппоинтментреплитиме](appointmentreplytime.md) <br/> |Представляет дату и время, когда участник ответил на приглашение на собрание.  <br/> |
|[аппоинтментсекуенценумбер](appointmentsequencenumber.md) <br/> |Задает порядковый номер версии встречи.  <br/> |
|[аппоинтментстате](appointmentstate.md) <br/> |Указывает состояние встречи.  <br/> |
|[Повторение (RecurrenceType)](recurrence-recurrencetype.md) <br/> |Содержит шаблон повторения для элементов календаря и приглашений на собрание.  <br/> Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.  <br/> |
|[фирстоккурренце](firstoccurrence.md) <br/> |Представляет первое вхождение повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.  <br/> |
|[ластоккурренце](lastoccurrence.md) <br/> |Представляет последнее вхождение повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.  <br/> |
|[модифиедоккурренцес](modifiedoccurrences.md) <br/> |Содержит массив повторяющихся экземпляров повторяющихся элементов календаря, которые были изменены таким образом, что они отличаются от элемента шаблона повторения.  <br/> Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.  <br/> |
|[делетедоккурренцес](deletedoccurrences.md) <br/> |Содержит массив удаленных экземпляров повторяющегося элемента календаря.  <br/> Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.  <br/> |
|[митингтимезоне](meetingtimezone.md) <br/> |Представляет часовой пояс для расположения, в котором размещается собрание.  <br/> |
|[StartTimeZone](starttimezone.md) <br/> |Представляет часовой пояс элемента календаря.  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |Представляет конечный часовой пояс элемента календаря.  <br/> |
|[конференцетипе](conferencetype.md) <br/> |Описывает тип конференций, который выполняется с элементом календаря.  <br/> |
|[алловневтимепропосал](allownewtimeproposal.md) <br/> |Указывает, может ли новое время проведения собрания предлагаться участнику.  <br/> |
|[исонлинемитинг](isonlinemeeting.md) <br/> |Указывает, находится ли собрание в сети.  <br/> |
|[митингворкспацеурл](meetingworkspaceurl.md) <br/> |Содержит URL-адрес рабочей области для собраний, связанной с элементом календаря.  <br/> |
|[нетшовурл](netshowurl.md) <br/> |Указывает URL-адрес собрания Microsoft NetShow.  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[ластмодифиеднаме](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя для изменения элемента.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[Связанный](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[вебклиентреадформкуеристринг](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[вебклиентедитформкуеристринг](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для изменения элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аджацентмитингс](adjacentmeetings.md) <br/> |Описывает все элементы календаря, смежные с временем собрания.  <br/> |
|[аппендтоитемфиелд](appendtoitemfield.md) <br/> |Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуют с временем собрания.  <br/> |
|[Create (Итемсинк)](create-itemsync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Элементы (Нонемптяррайофаллитемстипе)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания в папке, определяемой элементом [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) .  <br/> |
|[сетитемфиелд](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в [операции UpdateItem](updateitem-operation.md).  <br/> |
|[Обновление (Итемсинк)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Когда один элемент календаря обновляется, чтобы стать повторяющимся элементом основного календаря, необходимо указать элемент [митингтимезоне](meetingtimezone.md) , чтобы сохранить исходный часовой пояс элемента календаря. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
  
[Справка по веб-служб Exchange для Exchange](ews-reference-for-exchange.md)

