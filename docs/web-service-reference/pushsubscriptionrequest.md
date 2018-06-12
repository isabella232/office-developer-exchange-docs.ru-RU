---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: Элемент PushSubscriptionRequest — подписка на подписку на уведомления о принудительной события.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834929"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

Элемент **PushSubscriptionRequest** — подписка на подписку на уведомления о принудительной события. 
  
[Подписка](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **PushSubscriptionRequestType**
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
|[Водяной знак](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика. Используется для создания подписки, начиная с события, представленного водяного знака. Если водяного знака из подписки на запрос не найден, возврату ошибки будут возвращены клиенту. Это может произойти, если водяной знак старше 30 дней или если водяного знака никогда не был указан в почтовом ящике.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Представляет частоту, в минутах, в какой уведомлении сообщения будут отправляться клиенту возникновения события не.  <br/> |
|[URL-адрес](url-ex15websvcsotherref.md) <br/> |Представляет расположение клиента веб-службы push-уведомлений.  <br/> |
   
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



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)

