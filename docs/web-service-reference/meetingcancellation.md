---
title: MeetingCancellation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MeetingCancellation
api_type:
- schema
ms.assetid: a9c61f7f-2ecd-4b21-9dce-24d9f61aeeea
description: Элемент MeetingCancellation представляет отмену собрания в Exchange магазине.
ms.openlocfilehash: 979db9af3092247fe09775fb2d7a43394a09925c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523974"
---
# <a name="meetingcancellation"></a>MeetingCancellation

Элемент **MeetingCancellation** представляет отмену собрания в Exchange магазине. 
  
```xml
<MeetingCancellation>
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
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
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
</MeetingCancellation>
```

 **MeetingCancellationMessageType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит родной поток MIME объекта, который представлен в формате base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет субъект для Exchange элементов и объектов отклика. Субъект ограничен 255 символами.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень чувствительности элемента.  <br/> |
|[Основной текст](body.md) <br/> |Представляет фактическое содержимое тела сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время, когда элемент в почтовом ящике был получен.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в bytes элемента. Это свойство доступно только для чтения.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, которые определяют, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, на который этот элемент является ответом.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку по умолчанию "Избокс".  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет, был ли элемент еще не отправлен.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемент ему или себе.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, был ли элемент изменен.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заглавных сообщений в Интернете, содержащихся в элементе в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время, когда был отправлен элемент в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Этот элемент используется [элементом ReminderMinutesBeforeStart](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлено ли напоминание для элемента в Exchange магазине.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события, на которое отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Представляет строку отображения, используемую для содержимого окна Cc. Это совмещенная строка всех имен отображения получателей Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Представляет строку отображения, используемую для содержимого окна To. Это конкаентированная строка всех имен отображения получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое настроено на **верное,** если элемент имеет хотя бы одно видимое вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет культуру для данного элемента в почтовом ящике.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит имя отображения последнего пользователя, который должен изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает, когда элемент был изменен в последний раз.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для одновременного Microsoft Office Outlook конечной точки веб-приложения для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для одновременного Outlook Web App конечной точки для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или простой текст, который представляет уникальное тело этого разговора.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправитель элемента.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит набор получателей сообщения.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые получат копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения слепой копии (BCC) электронной почты.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента квитанцию для чтения.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента квитанцию доставки.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичный ID, который представляет поток, к которому принадлежит это сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет адресата, от которого было отправлено сообщение.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения в Интернете элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли прочитано сообщение.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Указывает, запрашивается ли ответ на сообщение электронной почты.  <br/> |
|[Ссылки](references.md) <br/> |Представляет заглавную ссылку Usenet, которая используется для сопоставления ответов с их исходными сообщениями.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет набор адресов, на которые должны быть отправлены ответы.  <br/> |
|[AssociatedCalendarItemId](associatedcalendaritemid.md) <br/> |Представляет элемент календаря, связанный с [meetingMessage.](meetingmessage.md)  <br/> |
|[IsDelegated](isdelegated.md) <br/> |Указывает, была ли встреча обработана учетной записью с доступом делегата.  <br/> |
|[IsOutOfDate](isoutofdate.md) <br/> |Указывает, устарело ли сообщение собрания.  <br/> |
|[HasBeenProcessed](hasbeenprocessed.md) <br/> |Указывает, был ли обработан элемент сообщения собрания.  <br/> |
|[ResponseType](responsetype.md) <br/> |Представляет тип ответа получателя, полученного для собрания.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Определяет делегата в сценарии доступа делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Определяет главного в сценарии доступа к делегатам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UID](uid.md) <br/> |Определяет элемент календаря.  <br/> |
|[RecurrenceId](recurrenceid.md) <br/> |Используется для определения определенного экземпляра повторяющегося элемента календаря.  <br/> |
|[DateTimeStamp](datetimestamp.md) <br/> |Указывает дату и время создания экземпляра объекта iCalendar.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Определяет все элементы календаря, которые примыкают к времени собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Определяет данные для приложения к одному свойству элемента во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтуя со временем собрания.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Определяет один элемент, который необходимо создать в локальном клиентской магазине.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов для создания.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном клиентской магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

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

