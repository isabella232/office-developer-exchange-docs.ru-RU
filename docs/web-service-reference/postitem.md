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
description: Элемент "i Item" представляет элемент POST в хранилище Exchange.
ms.openlocfilehash: 3fb6d6cfe334999c93ca0238547dd5aee8150a5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834866"
---
# <a name="postitem"></a>PostItem

Элемент "i **Item** " представляет элемент POST в хранилище Exchange. 
  
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

 **Неitemtype**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Сохранитьmimecontent](mimecontent.md) <br/> |Содержит собственный многоцелевой поток расширений почты в Интернете (MIME) объекта, представленного в формате base64Binary.  <br/> |
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange. Это свойство доступно только для чтения.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей элемент или папку. Это свойство доступно только для чтения.  <br/> |
|[ItemClass](itemclass.md) <br/> |Представляет класс сообщения для элемента.  <br/> |
|[Тема](subject.md) <br/> |Представляет тему для элементов хранилища Exchange и объектов ответа. Тема может иметь не более 255 символов.  <br/> |
|[Sensitivity](sensitivity.md) <br/> |Указывает уровень конфиденциальности элемента.  <br/> |
|[Основной текст](body.md) <br/> |Представляет реальное содержимое основного текста сообщения.  <br/> |
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
|[дисплайкк](displaycc.md) <br/> |Представляет отображаемую строку, используемую для содержимого поля "копия". Это объединенная строка всех отображаемых имен получателей копии.  <br/> |
|[дисплайто](displayto.md) <br/> |Представляет отображаемую строку, используемую для содержимого поля "Кому". Это объединенная строка для отображаемых имен получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое имеет значение **true** , если элемент имеет по крайней мере одно вложение. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок и элементов.  <br/> |
|[Culture](culture.md) <br/> |Представляет язык и региональные параметры для определенного элемента в почтовом ящике.  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.  <br/> |
|[ластмодифиеднаме](lastmodifiedname.md) <br/> |Содержит отображаемое имя последнего пользователя для изменения элемента.  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |Указывает время последнего изменения элемента.  <br/> |
|[Связанный](isassociated.md) <br/> |Указывает, связан ли элемент с папкой.  <br/> |
|[вебклиентреадформкуеристринг](webclientreadformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Microsoft Office Outlook Web App для чтения элемента в Outlook Web App.  <br/> |
|[вебклиентедитформкуеристринг](webclienteditformquerystring.md) <br/> |Представляет URL-адрес для сцепления с конечной точкой Outlook Web App для изменения элемента в Outlook Web App.  <br/> |
|[ConversationId](conversationid.md) <br/> |Содержит идентификатор элемента или беседы.  <br/> |
|[UniqueBody](uniquebody.md) <br/> |Представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.  <br/> |
|[ConversationIndex](conversationindex.md) <br/> |Содержит двоичный код, представляющий поток, к которому относится сообщение.  <br/> |
|[ConversationTopic](conversationtopic.md) <br/> |Представляет идентификатор беседы.  <br/> |
|[From](from.md) <br/> |Представляет адрес, с которого отправлен элемент POST. Элемент **from** можно задать только во время создания.  <br/> |
|[InternetMessageId](internetmessageid.md) <br/> |Представляет идентификатор сообщения Интернета для элемента.  <br/> |
|[IsRead](isread.md) <br/> |Указывает, было ли Прочитано сообщение.  <br/> |
|[постедтиме](postedtime.md) <br/> |Представляет время отправки почтового [элемента](postitem.md) .  <br/> |
|[References](references.md) <br/> |Представляет заголовок Usenet, используемый для связывания ответов с исходными сообщениями.  <br/> |
|[Sender](sender.md) <br/> |Определяет отправителя элемента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[сетитемфиелд](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции UpdateItem.  <br/> |
|[аппендтоитемфиелд](appendtoitemfield.md) <br/> |Определяет данные, добавляемые к одному свойству элемента или папки во время [операции UpdateItem](updateitem-operation.md).  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Create (Итемсинк)](create-itemsync.md) <br/> |Определяет один элемент, который необходимо создать в локальном хранилище клиента.  <br/> |
|[Обновление (Итемсинк)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном хранилище клиента.  <br/> |
|[реадфлагчанже](readflagchange.md) <br/> |Возвращается в ответах [SyncFolderItems](syncfolderitems.md) при чтении элемента. Это свойство доступно только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[конфликтингмитингс](conflictingmeetings.md) <br/> |Определяет все элементы, которые конфликтуют с временем собрания.  <br/> |
|[аджацентмитингс](adjacentmeetings.md) <br/> |Описывает все элементы календаря, смежные с временем собрания.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

