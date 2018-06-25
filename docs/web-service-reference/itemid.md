---
title: Идентификатор элемента
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemId
api_type:
- schema
ms.assetid: 3350b597-57a0-4961-8f44-8624946719b4
description: Элемент ItemId содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange.
ms.openlocfilehash: 9c5d71a23e1e4b77d2a50016aa4d765d872d04cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834157"
---
# <a name="itemid"></a>Идентификатор элемента

Элемент **ItemId** содержит уникальный идентификатор и меняет ключ элемента в хранилище Exchange. 
  
```XML
<ItemId Id="" ChangeKey="" />
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|
  **Id** <br/> |Идентифицирует определенного элемента в хранилище Exchange. **ID** учитывается регистр; Таким образом сравнение **идентификаторы** должен быть с учетом регистра или двоичный.  <br/> |
|**ChangeKey** <br/> | Идентифицирует определенной версии элемента. <br/><br/>**ChangeKey** является обязательным для следующих сценариев: <br/> <br/>- [UpdateItem](updateitem.md) , которого требует элемент **ChangeKey** Если атрибут **ConflictResolution** имеет значение автоматического разрешения конфликтов. Автоматическое разрешение — это значение по умолчанию. Если атрибут **ChangeKey** не указан, ответ вернет значение [ResponseCode](responsecode.md) равно **ErrorChangeKeyRequired**.  <br/><br/>-Элемент [SendItem](senditem.md) требует **ChangeKey** для проверки, является ли операцию будет действовать после последней версии элемента. Если атрибут **ChangeKey** не включен в **ItemId** или **ChangeKey** пуст, ответ вернет значение [ResponseCode](responsecode.md) равно **ErrorStaleObject**.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, при копировании элемента или папки.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, при создании элемента или папки.  <br/> |
|[Удаление (ItemSync)](delete-itemsync.md) <br/> |Определяет один элемент для удаления в локальном хранилище клиента.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, при удалении элемента или папки.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[ExportItemsResponseMessage](exportitemsresponsemessage.md) <br/> |Содержит состояние и результаты запроса на экспорт элемента одного почтового ящика.  <br/> |
|[FirstOccurrence](firstoccurrence.md) <br/> |Представляет первого появления повторяющегося элемента календаря.  <br/> |
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
|[Пропуск](ignore.md) <br/> |Определяет элементы, чтобы пропустить во время синхронизации.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange.  <br/> |
|[Элемент (UploadItemType)](item-uploaditemtype.md) <br/> |Представляет один элемент для передачи в почтовый ящик.  <br/> |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления для применения к элементу.  <br/><br/> Ниже приведен выражение XPath для этого элемента. <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[Что ItemID](itemids.md) <br/> | Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange. <br/> <br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
|[Что ItemID (NonEmptyArrayOfItemIdsType)](itemids-nonemptyarrayofitemidstype.md) <br/> |Содержит массив идентификаторов элементов, определите, какие элементы из почтового ящика.  <br/> |
|[LastOccurrence](lastoccurrence.md) <br/> |Представляет последнего вхождения повторяющегося элемента календаря.  <br/> |
|[Mailbox](mailbox.md) <br/> |Определяет объект службы каталогов с включенной поддержкой почты Active Directory.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, происходящее при изменении элемента.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, которое происходит, когда элемент перемещается из одной родительской папки в другую.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, которое инициируется нового элемента почты в почтовом ящике.  <br/> |
|[Вхождение](occurrence.md) <br/> |Представляет измененной вхождения повторяющегося элемента календаря.  <br/> |
|[PlayOnPhone (веб-служб Exchange)](playonphone-exchange-web-services.md) <br/> |Представляет запрос на его чтение на телефон.  <br/> |
|[RemoveItem](removeitem.md) <br/> |Удаляет элемент из хранилища Exchange.  <br/> |
|[RoomList](roomlist.md) <br/> |Представляет адрес электронной почты, который определяет список конференц-залы.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[UploadItemsResponseMessage](uploaditemsresponsemessage.md) <br/> |Содержит состояние и результаты запроса для отправки элемента одного почтового ящика.  <br/> |
|[UserConfiguration](userconfiguration.md) <br/> |Определяет объект конфигурации одного пользователя.  <br/> |
   
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

- [Операция ExportItems](exportitems-operation.md)
- [Операция UploadItems](uploaditems-operation.md) 
- [FindConversation Operation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

