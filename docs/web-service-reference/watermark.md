---
title: Водяной знак
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Watermark
api_type:
- schema
ms.assetid: e1545046-94f9-4ac7-af1c-ea81dfb6822c
description: Элемент водяной знак — это закладка события в очереди событий почтового ящика.
ms.openlocfilehash: 1867aa781bc24f5eb3bdb4648fa494a2a7ea396a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840487"
---
# <a name="watermark"></a>Водяной знак

Элемент **водяной знак** — это закладка события в очереди событий почтового ящика. 
  
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
|[PullSubscriptionRequest](pullsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о событий на основе репликации по запросу.  <br/> |
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о принудительной события.  <br/> |
|[GetEvents](getevents.md) <br/> |Представляет операцию, используемую клиентами пула для запроса уведомлений с сервера.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, куда копируются элемента или папки.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, где создается элемент или папку.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, где удаления элемента или папки.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, где при изменении элемента или папки.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, где элемента или папки перемещаются из одной родительской папки в другую.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет события, вызванные нового элемента почты в почтовом ящике.  <br/> |
|[StatusEvent](statusevent.md) <br/> |Представляет уведомление о том, что не новые действия в почтовом ящике.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат запроса подписаться.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение может быть обязательный или необязательный в зависимости от того, как используется данный элемент.
  
## <a name="remarks"></a>Замечания

Если подписки на запрос содержит водяного знака, от переадресации водяного знака создается подписка. Если запрос подписки на содержит водяной знак, не найден в таблице событий почтового ящика `ErrorInvalidWatermark` клиентскому приложению возвращается ошибка. Это может произойти, если водяной знак устарел и был удален из окна 30-дневный таблицы событий или если водяной знак не требуется даже представления в таблице "events". Например, это может произойти, если водяной знак получен из другой подписки для почтового ящика в другую базу данных. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Отписаться операции](unsubscribe-operation.md)

