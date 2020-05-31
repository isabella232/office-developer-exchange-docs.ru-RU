---
title: пушсубскриптионрекуест
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
description: Элемент Пушсубскриптионрекуест представляет подписку на подписку на уведомления о событиях на основе push-уведомлений.
ms.openlocfilehash: 34717d37b8e5bb50c927e57088299fbcb18a2514
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834929"
---
# <a name="pushsubscriptionrequest"></a>пушсубскриптионрекуест

Элемент **пушсубскриптионрекуест** представляет подписку на подписку на уведомления о событиях на основе push-уведомлений. 
  
[Подписаться](subscribe.md)
  
[пушсубскриптионрекуест](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **пушсубскриптионрекуесттипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**субскрибетоаллфолдерс** <br/> |Указывает, следует ли подписываться на все доступные папки. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдеридс](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для определения папок, которые необходимо отслеживать для получения уведомлений о событиях.  <br/> |
|[евенттипес](eventtypes.md) <br/> |Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.  <br/> |
|[Watermark](watermark.md) <br/> |Представляет закладку события в таблице событий почтовых ящиков. Используется для создания подписки, начиная с события, представленного водяным знаком. Если водяной знак из запроса на подписку не найден, клиенту будет возвращен ответ об ошибке. Это может произойти, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Представляет частоту, заданную в минутах, с которой сообщения уведомлений будут отправляться клиенту при отсутствии событий.  <br/> |
|[Адрес](url-ex15websvcsotherref.md) <br/> |Представляет расположение клиентской веб-службы для push-уведомлений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Подписаться](subscribe.md) <br/> |Содержит свойства, используемые для создания подписок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

