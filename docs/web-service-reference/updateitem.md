---
title: UpdateItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItem
api_type:
- schema
ms.assetid: 34643d58-2743-45b0-a08d-bff6dc1da61d
description: Элемент UpdateItem определяет запрос на обновление элемента в почтовом ящике.
ms.openlocfilehash: 7b9b5f1dcffb95eb127572cb91f92d961c05a77e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840357"
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
|**ConflictResolution** <br/> |Идентифицирует тип разрешения конфликтов попробовать во время обновления. Значение по умолчанию — автоматическое разрешение.  <br/> |
|**MessageDisposition** <br/> |Описывает, как будут обрабатываться элемента после обновления. Атрибут **MessageDisposition** является обязательным для элементов сообщения, включая сообщения собрания, такие как отмен собрания, приглашений на собрания и ответы на приглашения.  <br/> |
|**SendMeetingInvitationsOrCancellations** <br/> |Описывает, как собрание обновления передаются после обновления элемента календаря. Этот атрибут является обязательным для элементов календаря и вхождения элемента календаря.  <br/> |
|**SuppressReadReceipts** <br/> |Указывает, следует ли подавлять прочтении обновленного элемента. Текстовое значение **true,** указывает, что чтения, подавляются поступлений. Значение **false** указывает, что прочтении отправляются отправителю. Этот атрибут является необязательным.  <br/> Этот атрибут появился в Exchange Server 2013 с пакетом обновления 1.  <br/> |
   
#### <a name="conflictresolution-attribute"></a>Атрибут ConflictResolution

|**Значение**|**Описание**|
|:-----|:-----|
|NeverOverwrite  <br/> |Если происходит конфликт, происходит сбой операции обновления и возвращается сообщение об ошибке.  <br/> |
|Автоматическое разрешение  <br/> |Операции обновления автоматически конфликты любой.  <br/> |
|AlwaysOverwrite  <br/> |В случае конфликта операции обновления перезапишет данные.  <br/> |
   
#### <a name="messagedisposition-attribute"></a>Атрибут MessageDisposition

|**Значение**|**Описание**|
|:-----|:-----|
|SaveOnly  <br/> |Элемент обновлен и сохранения его текущей папки.  <br/> |
|SendOnly  <br/> |Элемент обновлен и отправляются, но копия не сохраняется.  <br/> |
|SendAndSaveCopy  <br/> |Элемент обновляется и копия сохраняется в папку, указанную в элементе [SavedItemFolderId](saveditemfolderid.md) .  <br/> |
   
#### <a name="sendmeetinginvitationsorcancellations-attribute"></a>Атрибут SendMeetingInvitationsOrCancellations

|**Значение**|**Описание**|
|:-----|:-----|
|SendToNone  <br/> |Обновление элемента календаря, но обновления не отправляются участникам.  <br/> |
|SendOnlyToAll  <br/> |Обновлены элемента календаря и обновление собрания отправляется всех участников, но не сохраняются в папке «Отправленные».  <br/> |
|SendOnlyToChanged  <br/> |Обновлены элемента календаря и обновление собрания отправляется только участникам, которые повлияет переход на собрании.  <br/> |
|SendToAllAndSaveCopy  <br/> |Обновления элемента календаря, сообщения о встрече всем участникам и копия сохраняется в папке «Отправленные».  <br/> |
|SendToChangedAndSaveCopy  <br/> |Обновлено элемента календаря, сообщения о встрече для всех участников, которые повлияет переход на собрании и копия сохраняется в папке «Отправленные».  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SavedItemFolderId](saveditemfolderid.md) <br/> |Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.  <br/> |
|[ItemChanges](itemchanges.md) <br/> |Содержит массив элементов [ItemChange](itemchange.md) , чтобы указать элементы и обновления, чтобы применить к элементам.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateItem Operation](updateitem-operation.md)

