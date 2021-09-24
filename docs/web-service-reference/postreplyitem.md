---
title: PostReplyItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PostReplyItem
api_type:
- schema
ms.assetid: e5d93d63-0a3b-470f-9a94-2d57284c6745
description: Элемент PostReplyItem содержит ответ на сообщение элемента. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 657173e19d5dc1bb6a8126b62c5977d5afc1c17c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527909"
---
# <a name="postreplyitem"></a>PostReplyItem

Элемент **PostReplyItem** содержит ответ на сообщение элемента. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<PostReplyItem>
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
   <EffectiveRights/>
   <ReceivedBy/>
   <ReceivedRepresenting/>
   <NewBodyContent/>
</PostReplyItem>
```

 **PostReplyItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит родной многоцелевой поток расширения интернет-почты (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в Exchange магазине. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет субъект для Exchange элементов и объектов отклика. Субъект ограничен 255 символами.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень чувствительности элемента.  <br/> |
|[Основной текст](body.md) <br/> |Представляет фактическое содержимое тела сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, присоединенные к элементу в Exchange магазине.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время, когда элемент в почтовом ящике был получен.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в bytes элемента. Это свойство доступно только для чтения.  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, которые определяют категории, к которым относится элемент в почтовом ящике.  <br/> |
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
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Представляет строку отображения, используемую для содержимого строки Cc. Это совмещенная строка всех имен отображения получателей Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Представляет строку отображения, используемую для содержимого окна To. Это конкаентированная строка всех имен отображения получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое настроено на **верное,** если элемент имеет вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет культуру для данного элемента в почтовом ящике.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправитель элемента.  <br/> |
|[ToRecipients](torecipients.md) <br/> |Содержит набор получателей сообщения.  <br/> |
|[CcRecipients](ccrecipients.md) <br/> |Представляет коллекцию получателей, которые получат копию сообщения.  <br/> |
|[BccRecipients](bccrecipients.md) <br/> |Представляет коллекцию получателей для получения слепой копии (BCC) электронной почты.  <br/> |
|[IsReadReceiptRequested](isreadreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента квитанцию для чтения.  <br/> |
|[IsDeliveryReceiptRequested](isdeliveryreceiptrequested.md) <br/> |Указывает, запрашивает ли отправитель элемента квитанцию доставки.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичный ID, который представляет поток, к которому принадлежит это сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет адрес, с которого было отправлено сообщение.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения в Интернете элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли прочитано сообщение.  <br/> |
|[IsResponseRequested](isresponserequested.md) <br/> |Указывает, запрашивается ли ответ на сообщение электронной почты.  <br/> |
|[Ссылки](references.md) <br/> |Представляет заглавную ссылку Usenet, которая используется для связывать ответы с их исходными сообщениями.  <br/> |
|[ReplyTo](replyto.md) <br/> |Определяет набор адресов, на которые должны быть отправлены ответы.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReceivedBy](receivedby.md) <br/> |Определяет делегата в сценарии доступа делегата. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReceivedRepresenting](receivedrepresenting.md) <br/> |Определяет главного в сценарии доступа к делегатам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[NewBodyContent](newbodycontent.md) <br/> |Представляет новое содержимое тела элемента post.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описывает все элементы, примыкающие к времени собрания.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Описывает все элементы, которые конфликтуют со временем собрания.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, идентифицированной элементом [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

