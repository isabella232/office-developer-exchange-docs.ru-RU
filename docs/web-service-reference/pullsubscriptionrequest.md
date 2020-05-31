---
title: пуллсубскриптионрекуест
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
description: Элемент Пуллсубскриптионрекуест представляет подписку на подписку на уведомления о событиях по запросу.
ms.openlocfilehash: 5f757bf1f79f7e2a00fb886db50e6ea0eaed1a4a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834932"
---
# <a name="pullsubscriptionrequest"></a>пуллсубскриптионрекуест

Элемент **пуллсубскриптионрекуест** представляет подписку на подписку на уведомления о событиях по запросу. 
  
[Подписаться](subscribe.md)
  
[пуллсубскриптионрекуест](pullsubscriptionrequest.md)
  
```XML
<PullSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <Timeout/>
</PullSubscriptionRequest>
```

 **пуллсубскриптионрекуесттипе**
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
|[Watermark](watermark.md) <br/> |Представляет закладку события в таблице событий почтовых ящиков. Используется для создания подписки, которая начинается с события, представленного водяным знаком. Если водяной знак из запроса на подписку не найден, клиенту будет возвращен ответ об ошибке. Эта ошибка может возникать, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.  <br/> |
|[Timeout](timeout.md) <br/> |Представляет продолжительность в минутах, в течение которого подписка может быть бездействовать без запроса на получение событий от клиента.  <br/> |
   
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



[пушсубскриптионрекуест](pushsubscriptionrequest.md)
  
[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

