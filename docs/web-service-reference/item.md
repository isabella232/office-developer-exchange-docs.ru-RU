---
title: Item
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Item
api_type:
- schema
ms.assetid: 4dfe8f48-e7b4-444d-bdf9-a34e180f598b
description: Элемент Item представляет универсальный элемент в Exchange магазине.
ms.openlocfilehash: bf634949d440b5c8223aeb90c04e63825e1198e9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540946"
---
# <a name="item"></a>Item

Элемент **Item** представляет универсальный элемент в Exchange магазине. 
  
```xml
<Item>
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
</Item>
```

 **ItemType**
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
|[Categories](categories-ex15websvcsotherref.md) <br/> |Представляет коллекцию строк, которые определяют, к какой категории относится элемент в почтовом ящике.  <br/> |
|[Importance](importance.md) <br/> |Описывает важность элемента.  <br/> |
|[InReplyTo](inreplyto.md) <br/> |Представляет идентификатор элемента, на который этот элемент является ответом.  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |Указывает, был ли элемент отправлен в папку по умолчанию "Избокс".  <br/> |
|[IsDraft](isdraft.md) <br/> |Представляет, был ли элемент еще не отправлен.  <br/> |
|[IsFromMe](isfromme.md) <br/> |Указывает, отправил ли пользователь элемент самому себе.  <br/> |
|[IsResend](isresend.md) <br/> |Указывает, был ли ранее отправлен элемент.  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |Указывает, был ли элемент изменен.  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |Представляет коллекцию всех заглавных сообщений в Интернете, содержащихся в элементе в почтовом ящике.  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |Представляет дату и время, когда был отправлен элемент в почтовом ящике.  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |Представляет дату и время создания данного элемента в почтовом ящике.  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |Представляет дату и время, когда происходит событие. Этот элемент используется [элементом ReminderMinutesBeforeStart](reminderminutesbeforestart.md) для определения времени отображения напоминания.  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Указывает, установлено ли напоминание для элемента в Exchange магазине.  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |Представляет количество минут до события, когда отображается напоминание.  <br/> |
|[DisplayCc](displaycc.md) <br/> |Представляет строку отображения, используемую для содержимого окна Cc. Это совмещенная строка всех имен отображения получателей Cc.  <br/> |
|[DisplayTo](displayto.md) <br/> |Представляет строку отображения, используемую для содержимого окна To. Это конкаентированная строка всех имен отображения получателей.  <br/> |
|[HasAttachments](hasattachments.md) <br/> |Представляет свойство, которое настроено на **верное,** если элемент имеет вложения по крайней мере одного видимого вложения. Это свойство доступно только для чтения.  <br/> |
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
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |Описывает все элементы календаря, которые примыкают к времени собрания.  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |Определяет данные для приложения к одному свойству элемента или папки во время операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |Определяет все элементы, конфликтуя со временем собрания.  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |Определяет один элемент, который необходимо создать в локальном клиентской магазине.  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Представляет элемент Exchange, присоединенный к другому элементу Exchange.  <br/> |
|[Items](items.md) <br/> |Содержит массив элементов.  <br/> |
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, идентифицированной элементом [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[SetItemField](setitemfield.md) <br/> |Представляет обновление одного свойства элемента в операции [UpdateItem.](updateitem-operation.md)  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |Определяет один элемент для обновления в локальном клиентской магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Важно отметить, что **ItemType** является базовым типом [задачи,](task.md) [CalendarItem,](calendaritem.md) [Contact,](contact.md) [DistributionList](distributionlist.md)и [Message](message-ex15websvcsotherref.md).
  
[Элементы](message-ex15websvcsotherref.md) сообщений представляют сообщения электронной почты и все другие элементы, которые не сильно впечатлены схемой Exchange веб-служб (EWS). Такие элементы, как IPM. Общий доступ и IPM.InfoPath возвращаются в качестве **элементов сообщения.** Microsoft Exchange Server 2010 не возвращает базовый элемент **Item** в ответах. 
  
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

