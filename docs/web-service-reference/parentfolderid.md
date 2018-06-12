---
title: ParentFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 258f4b1f-367e-4c7d-9c29-eb775a2398c7
description: Элемент ParentFolderId представляет идентификатор родительской папки, содержащей элемент или папку.
ms.openlocfilehash: 3f60e8adb62fbf464a58af4169fbcd83910877cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834687"
---
# <a name="parentfolderid"></a>ParentFolderId

Элемент **ParentFolderId** представляет идентификатор родительской папки, содержащей элемент или папку. 
  
```XML
<ParentFolderId Id="" ChangeKey=""/>
```

**FolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Содержит строку, которая определяет папке в хранилище Exchange. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Содержит строку, которая определяет к папке, которая определена в атрибуте **Id** версии. Этот атрибут является необязательным. Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку Календарь в почтовом ящике.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря в почтовом ящике.  <br/> |
|[Контакт](contact.md) <br/> |Представляет контакт в почтовом ящике.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копирование элемента или папки.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, в котором создается элемента или папки.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, в котором удаляется элемент или папку.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки закрытый в почтовом ящике.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange.  <br/> |
|[Элемент (UploadItemType)](item-uploaditemtype.md) <br/> |Представляет один элемент для передачи в почтовый ящик.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмены собрания в почтовом ящике.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания в почтовом ящике.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашения на собрание в почтовом ящике.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение в почтовом ящике.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты в почтовом ящике.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, в котором изменения элемента или папки.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, которое инициируется нового элемента почты в почтовом ящике.  <br/> |
|[AcceptItem](acceptitem.md) <br/> |Представляет ответ на принять приглашение на собрание.  <br/> |
|[TentativelyAcceptItem](tentativelyacceptitem.md) <br/> |Представляет под вопросом ответ на приглашения на собрание.  <br/> |
|[DeclineItem](declineitem.md) <br/> |Представляет отклонить ответ на приглашения на собрание.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет элемент задачи в почтовом ящике.  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |Содержит ответ создателем элемента в хранилище Exchange.  <br/> |
|[ReplyAllToItem](replyalltoitem.md) <br/> |Содержит ответить всем получателям определенного элемента в хранилище Exchange.  <br/> |
|[ForwardItem](forwarditem.md) <br/> |Содержит элемент хранилища Exchange переадресация получателям.  <br/> |
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |Представляет объект ответа, которая используется для отмены собрания.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

