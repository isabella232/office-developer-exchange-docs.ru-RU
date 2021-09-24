---
title: Watermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: Элемент Watermark представляет закладки событий в очереди событий почтового ящика.
ms.openlocfilehash: 959ae7369195a164d257b8805a8c985f1fdca53b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524401"
---
# <a name="watermark"></a>Watermark

Элемент **Watermark** представляет закладки событий в очереди событий почтового ящика. 
  
```xml
<Watermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Представляет подписку на подписку на уведомление о событиях на основе тяги.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписку на подписку на push-уведомление о событиях.  <br/> |
|[GetEvents](getevents.md) <br/> |Представляет операцию, используемую клиентами для запроса уведомлений с сервера.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, в котором создается элемент или папка.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, в котором элемент или папка удаляются.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, в котором элемент или папка изменены.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую родительную.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, инициированное новым элементом почты в почтовом ящике.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Представляет уведомление о том, что в почтовом ящике не было никаких новых действий.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат запроса подписки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение может быть обязательным или необязательным в зависимости от того, как этот элемент используется.
  
## <a name="remarks"></a>Заметки

Если запрос Подписка содержит водяной знак, подписка создается из водяного знака вперед. Если запрос Подписка содержит водяной знак, который не найден в таблице событий почтовых ящиков, ошибка возвращается  `ErrorInvalidWatermark` в клиентскую заявку. Это может произойти, если водяной знак слишком стар и удален из 30-дневного окна таблицы событий или если водяной знак никогда не присутствовал в таблице событий. Это может произойти, например, если водяной знак получен из другой подписки на почтовый ящик в другой базе данных. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)

