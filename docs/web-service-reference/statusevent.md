---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: Элемент StatusEvent представляет уведомление о том, что не новые действия в почтовом ящике.
ms.openlocfilehash: e214918f9795e9e29061d4aac72ab144d2b24267
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835592"
---
# <a name="statusevent"></a>StatusEvent

Элемент **StatusEvent** представляет уведомление о том, что не новые действия в почтовом ящике. 
  
```xml
<StatusEvent>
   <Watermark/>
</StatusEvent>
```

 **BaseNotificationEventType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Водяной знак](watermark.md) <br/> |Представляет последний допустимый водяного знака для подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Замечания

Элемент **StatusEvent** возвращается в уведомлении по одной из следующих причин: 
  
- Клиент извлечением отправляет запрос GetEvents на подписку, имеющей не выполняет никаких действий.
    
- Клиент push не имеет событий в очереди при достижении [StatusFrequency](statusfrequency.md) . 
    
**StatusEvent**[водяного знака](watermark.md) используется клиентским приложением в так же, как другие водяных знаков типа событий. Тем не менее водяного знака для **StatusEvent** не совпадает с водяные знаки, используемые для другие события. Например Подписка содержит события с подложки 1, 2 и 3 и эти события успешно отправлены в уведомлении. Период бездействия и отправить запрос **GetEvents** . Сервер клиентского доступа (CAS) возвращает состояние события и включает в себя водяного знака последней версии 3, как [PreviousWatermark](previouswatermark.md) и текущей [водяного знака](watermark.md).
  
Водяной знак будет остаются неизменными во всех случаях. Записи событий, сохраняются в течение 30 дней. Для поддержки активной подписки, сервер клиентского доступа периодически обновляет водяных знаков для очередей подписки. Обновленные подложки отправляются клиентов на обслуживание активной подписки.
  
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

