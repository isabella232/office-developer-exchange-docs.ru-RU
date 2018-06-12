---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: Элемент PullSubscriptionRequest — подписка на подписку на уведомления о событий на основе репликации по запросу.
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834932"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

Элемент **PullSubscriptionRequest** — подписка на подписку на уведомления о событий на основе репликации по запросу. 
  
[Подписка](subscribe.md)
  
[PullSubscriptionRequest](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 **PullSubscriptionRequestType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Указывает, следует ли подписка на всех доступных папок. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для определения папок для наблюдения за уведомления о событиях.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.  <br/> |
|[Водяной знак](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика. Используется для создания подписки, начинающимся на события, представленного водяного знака. Если водяного знака из подписки на запрос не найден, возврату ошибки будут возвращены клиенту. Эта ошибка может возникнуть, если водяной знак старше 30 дней или если водяного знака никогда не был указан в почтовом ящике.  <br/> |
|[Timeout](timeout.md) <br/> |Представляет продолжительность в минутах, подписки может простаивать без запроса GetEvents от клиента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Подписка](subscribe.md) <br/> |Содержит свойства, используемые для создания подписок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

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



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

