---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: Элемент StatusFrequency представляет максимальное значение времени в минутах, в которых попытки повторного и повторного ирисовки будут пытаться на сервере.
ms.openlocfilehash: f0359bab58167bbe7be5cce8c250240bebc7cc08
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525535"
---
# <a name="statusfrequency"></a>StatusFrequency

Элемент **StatusFrequency** представляет максимальное значение времени в минутах, в которых попытки повторного и повторного ирисовки будут пытаться на сервере. 
  
[Subscribe](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
[StatusFrequency](statusfrequency.md)
  
```XML
<StatusFrequency/>
```

 **SubscriptionStatusFrequencyType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписку на подписку на push-уведомление о событиях.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Если используется этот элемент, требуется текстовое значение, представляю которое представляет несколько элементов. Возможные значения для этого элемента : от 1 до 1440 включительно. Этот элемент является необязательным. Значение по умолчанию  30 минут.
  
## <a name="remarks"></a>Заметки

Значение **StatusFrequency** используется сервером для повторного запроса push-уведомления, если оно не получает ответа на push-уведомление или запрос состояния от клиента. Если сервер не получает ответа, он несколько раз отправляет уведомление, прежде чем перестать отправлять уведомление. В EWS интервал повторной работы по умолчанию составляет 30 секунд, а последующие ириски всегда удваив время последнего интервала повторной работы. Время повторной перезаверки не является точным, так как они могут быть отложены из-за других нагрузок на сервере. В следующей таблице показано, как происходят интервалы повторного исследования в 30 минутах, выделенных значением **StatusFrequency** по умолчанию (если предположить, что сервер не сталкивался с задержками). 
  
|**Повторить**|**Секунды**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Начальная синхронизация  <br/> |
|1   <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3   <br/> |120  <br/> |02:00  <br/> |
|4   <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6   <br/> |960  <br/> |16:00  <br/> |
|7   <br/> |1920  <br/> |32:00 - значение по умолчанию **StatusFrequency** превысило 30, повторное не отправлено  <br/> |
   
Если клиент не получает уведомления с сервера в течение периода времени, превышающего в два раза время, указанное **StatusFrequency,** клиент должен принять меры, такие как воссоздание подписки. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
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
  
[Watermark](watermark.md)

