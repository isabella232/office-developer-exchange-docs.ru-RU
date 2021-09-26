---
title: StatusEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusEvent
api_type:
- schema
ms.assetid: d3901818-2640-4bed-aad8-21a61aee62a1
description: Элемент StatusEvent представляет уведомление о том, что в почтовом ящике не было никаких новых действий.
ms.openlocfilehash: 777d5cd22e47fea6e7bf7432e58e5d58d1ef67a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543977"
---
# <a name="statusevent"></a>StatusEvent

Элемент **StatusEvent** представляет уведомление о том, что в почтовом ящике не было никаких новых действий. 
  
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
|[Watermark](watermark.md) <br/> |Представляет последний допустимый водяной знак для подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Заметки

Элемент **StatusEvent** возвращается в уведомлении по одной из следующих причин: 
  
- Клиент pull выдает запрос GetEvents на подписку, которая не имеет действий.
    
- Клиент push не имеет событий в очереди, когда был достигнут [StatusFrequency.](statusfrequency.md) 
    
Водяной **знак StatusEvent**[](watermark.md) используется клиентом так же, как и другие водяные знаки типа событий. Однако водяной знак **statusEvent** не то же самое, что и водяные знаки, используемые для других событий. Например, в подписке есть события с водяными знаками 1, 2 и 3, и эти события успешно передается в уведомлении. Наступает период бездействия и отправляется запрос **GetEvents.** Сервер клиентского доступа (CAS) возвращает событие состояния и включает последний водяной знак, 3, как [и PreviousWatermark](previouswatermark.md) и текущий [водяной знак](watermark.md).
  
Водяной знак не будет оставаться одинаковым во всех случаях. Записи событий сохраняются в течение 30 дней. Чтобы поддерживать активную подписку, CAS периодически обновляет водяные знаки для очередей подписки. Обновленные водяные знаки отправляются клиентам для поддержания активной подписки.
  
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

