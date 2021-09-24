---
title: PullSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PullSubscriptionRequest
api_type:
- schema
ms.assetid: 145c5cc7-a894-4f0b-a6ea-358cddfb5c33
description: Элемент PullSubscriptionRequest представляет подписку на подписку на уведомление о событиях на основе тяги.
ms.openlocfilehash: f1a527dff0c81262cac01a905293af1155acbf1c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540603"
---
# <a name="pullsubscriptionrequest"></a>PullSubscriptionRequest

Элемент **PullSubscriptionRequest** представляет подписку на подписку на уведомление о событиях на основе тяги. 
  
[Subscribe](subscribe.md)
  
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
|**SubscribeToAllFolders** <br/> |Указывает, следует ли подписываться на все доступные папки. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, используемых для идентификации папок для мониторинга уведомлений о событиях.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Содержит коллекцию уведомлений о событиях, используемых для создания подписки.  <br/> |
|[Watermark](watermark.md) <br/> |Представляет закладки событий в таблице событий почтового ящика. Это используется для создания подписки, которая начинается с события, которое представлено водяной знак. Если водяной знак из запроса Подписка не найден, клиенту будет возвращен ответ на ошибку. Эта ошибка может возникнуть, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.  <br/> |
|[Timeout](timeout.md) <br/> |Представляет продолжительность, в течение нескольких минут, чтобы подписка не простаивала без запроса GetEvents от клиента.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Содержит свойства, используемые для создания подписок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

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



[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

