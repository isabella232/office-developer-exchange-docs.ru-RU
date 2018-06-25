---
title: PostItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PostItem
api_type:
- schema
ms.assetid: 7727ed84-9591-4a1c-bb04-12129926499b
description: PostItem элемент представляет элемент post в хранилище Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834866"
---
# <a name="postitem"></a>PostItem

Элемент **PostItem** представляет элемент post в хранилище Exchange. 
  
```xml
<PostItem>
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
   <ConversationIndex/>
   <ConversationTopic/>
   <From/>
   <InternetMessageId/>
   <IsRead/>
   <PostedTime/>
   <References/>
   <Sender/>
</PostItem>
```

 **PostItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Содержит собственный поток Multipurpose Internet Mail Extensions (MIME), представленного в формате base64Binary объекта.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения элемента.  <br/> |
|[Subject](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объекты ответа. Тема ограничена 255 символов.  <br/> |
|[Уровень конфиденциальности сообщения](sensitivity.md) <br/> |Указывает уровень конфиденциальности для элемента.  <br/> |
|[Body](body.md) <br/> |Представляет фактическое содержимое основного текста сообщения.  <br/> |
|[Вложения](attachments-ex15websvcsotherref.md) <br/> |Содержит элементы или файлы, подключенные к элементу в хранилище Exchange.  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |Представляет дату и время получения элемента в почтовом ящике.  <br/> |
|[Размер](size.md) <br/> |Представляет размер в байтах элемента. Это свойство доступно только для чтения.  <br/> |
|[Категории](categories-ex15websvcsotherref.md) <br/> |Представляет набор строк, которые определяют категории, к которым принадлежит элемент в почтовом ящике.  <br/> |
|[Важность](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, к которому этот элемент является ее в ответ.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, является ли элемент был отправлен исходящие папке по умолчанию.  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет ли элемент еще не были отправлены.  <br/> |
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
|[DisplayCc](displaycc.md) <br/> |Строка отображения, который используется для содержимого в поле "Копия". Это составное строка всех получателей отображаемые имена «копия».  <br/> |
|[DisplayTo](displayto.md) <br/> |Строка отображения, который используется для содержимого в поле «Кому». Это составное строка всех для получателей отображаемые имена.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое задано значение **true,** Если у элемента есть по крайней мере одного вложения. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Язык и региональные параметры](culture.md) <br/> |Представляет язык и региональные параметры для заданного элемента в почтовом ящике.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя, чтобы изменить элемент.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[IsAssociated](isassociated.md) <br/> |Указывает, является ли элемент связан с папкой.  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для присоединения к конечной точке Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для объединения в конечную точку Outlook Web App для редактирования элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичные идентификатор, представляющий поток, к которой принадлежит это сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет адрес, с которого было отправлено элемента записи. Элемент **из** могут быть установлены только во время создания.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения Интернета элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, имеет ли чтение сообщения.  <br/> |
|[PostedTime](postedtime.md) <br/> |Представляет время, добавившего [PostItem](postitem.md) .  <br/> |
|[Справочные материалы](references.md) <br/> |Представляет заголовок групп, используемый для связи ответов с исходного сообщения.  <br/> |
|[Отправитель](sender.md) <br/> |Идентифицирует отправителя элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SetItemField](setitemfield.md) <br/> |Представляет обновление для одного свойства элемента в рамках одной операции UpdateItem.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Указывает данные для добавления во время [операции UpdateItem](updateitem-operation.md)отдельное свойство элемента или папки.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет собой элемент Exchange, подключенный к другой элемент Exchange.  <br/> |
|[Создание (ItemSync)](create-itemsync.md) <br/> |Определяет один элемент для создания в локальном хранилище клиента.  <br/> |
|[Обновление (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
|[ReadFlagChange](readflagchange.md) <br/> |Возвращаются в ответы [SyncFolderItems](syncfolderitems.md) прочтении элемента. Это свойство доступно только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[Элементы](items.md) <br/> |Содержит массив элементов.  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтующие с время собрания.  <br/> |
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описание всех элементов календаря, расположенных на время собрания.  <br/> |
   
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

