---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: Элемент UpdateItem определяет запрос на обновление элемента в почтовом ящике.
ms.openlocfilehash: 544ccfb8c42b2a4d4f69ae04d383233203c235b8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59542793"
---
# <a name="updateitem"></a>UpdateItem

Элемент **UpdateItem** определяет запрос на обновление элемента в почтовом ящике. 
  
```XML
<UpdateItem ConflictResolution="" MessageDisposition="" SendMeetingInvitationsOrCancellations="" SuppressReadReceipts="">
   <SavedItemFolderId/>
   <ItemChanges/>
</UpdateItem>
```

 **UpdateItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ConflictResolution** <br/> |Определяет тип разрешения конфликтов, который необходимо попробовать во время обновления. По умолчанию значение AutoResolve.  <br/> |
|**MessageDisposition** <br/> |Описывает, как будет обрабатываться элемент после его обновления. Атрибут **MessageDisposition** необходим для элементов сообщений, включая сообщения собраний, такие как отмена собраний, запросы на собрания и ответы на собрания.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Описывает, как сообщается об обновлениях собраний после обновления элемента календаря. Этот атрибут необходим для элементов календаря и событий элементов календаря.  <br/> |
|**SuppressReadReceipts** <br/> |Указывает, следует ли подавлять квитанции для чтения обновленного элемента. Текстовое значение **true указывает** на то, что чтение квитанций должно быть подавлено. Значение false **указывает** на то, что чеки чтения будут отправлены отправителю. Этот атрибут является необязательным.  <br/> Этот атрибут был введен в Exchange Server 2013 sp1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Атрибут ConflictResolution

|**Значение**|**Описание**|
|:-----|:-----|
|NeverOverwrite  <br/> |Если произошел конфликт, операция обновления сбой и ошибка возвращается.  <br/> |
|AutoResolve  <br/> |Операция обновления автоматически устраняет любой конфликт.  <br/> |
|AlwaysOverwrite  <br/> |При конфликте операция обновления переопишет сведения.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Атрибут MessageDisposition

|**Значение**|**Описание**|
|:-----|:-----|
|SaveOnly  <br/> |Элемент обновляется и возвращается в текущую папку.  <br/> |
|SendOnly  <br/> |Элемент обновляется и отправляется, но копия не сохранена.  <br/> |
|SendAndSaveCopy  <br/> |Элемент обновляется, а копия сохранена в папке, идентифицированной элементом [SavedItemFolderId.](saveditemfolderid.md)  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Атрибут SendMeetingInvitationsOrCancellations

|**Значение**|**Описание**|
|:-----|:-----|
|SendToNone  <br/> |Элемент календаря обновляется, но обновления не отправляются участникам.  <br/> |
|SendOnlyToAll  <br/> |Элемент календаря обновляется, а обновление собрания отправляется всем участникам, но не сохранено в папке Отправленные элементы.  <br/> |
|SendOnlyToChanged  <br/> |Элемент календаря обновляется, а обновление собрания отправляется только участникам, на которых влияет изменение собрания.  <br/> |
|SendToAllAndSaveCopy  <br/> |Элемент календаря обновляется, обновление собрания отправляется всем участникам, а копия сохранена в папке Отправленные элементы.  <br/> |
|SendToChangedAndSaveCopy  <br/> |Элемент календаря обновляется, обновление собрания отправляется всем участникам, затронутым изменением собрания, а копия сохранена в папке Отправленные элементы.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Содержит массив элементов [ItemChange,](itemchange.md) определяющие элементы и обновления для применения к элементам.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция UpdateItem](updateitem-operation.md)

