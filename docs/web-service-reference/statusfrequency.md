---
title: StatusFrequency
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StatusFrequency
api_type:
- schema
ms.assetid: 917474e2-a426-4166-b825-53783a41dad4
description: Элемент StatusFrequency представляет максимальное время ожидания в минутах, в которых повторных попыток на сервере.
ms.openlocfilehash: 402f8978c0ec6b377dfa020f23595c8954509a07
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835589"
---
# <a name="statusfrequency"></a>StatusFrequency

Элемент **StatusFrequency** представляет максимальное время ожидания в минутах, в которых повторных попыток на сервере. 
  
[Подписка](subscribe.md)
  
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
|[PushSubscriptionRequest](pushsubscriptionrequest.md) <br/> |Представляет подписка на подписку на уведомления о принудительной события.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение, представляющее целое число является обязательным, если данный элемент используется. Возможные значения для этого элемента: 1 до 1440 включительно. Этот элемент является необязательным. Значение по умолчанию — 30 минут.
  
## <a name="remarks"></a>Замечания

Значение **StatusFrequency** используется сервером-Повтор push-уведомления, когда не получает ответ push-уведомлений или состояние ping от клиента. Если сервер не получает ответ, повторов отправки уведомления несколько раз до остановки его отправки. В веб-служб Exchange интервал повтора по умолчанию — 30 секунд и последующих попыток, всегда double времени последнего интервал повтора. Время повтора не точное, как их можно отложить из-за другие нагрузки на сервере. В следующей таблице показаны как интервалы повтора возникают в 30 минут, выделенной значением по умолчанию **StatusFrequency** (предполагается, что сервер не обнаружил любой задержки). 
  
|**Число повторов**|**Секунд**|**Time**|
|:-----|:-----|:-----|
|0  <br/> |0  <br/> |Начальной синхронизации  <br/> |
|1  <br/> |30  <br/> |00:30  <br/> |
|2  <br/> |60  <br/> |01:00  <br/> |
|3  <br/> |120  <br/> |02:00  <br/> |
|4  <br/> |240  <br/> |04:00  <br/> |
|5  <br/> |480  <br/> |08:00  <br/> |
|6  <br/> |960  <br/> |16:00  <br/> |
|7  <br/> |1920  <br/> |32:00 - **StatusFrequency** значение по умолчанию 30 превышено, не отправляются число повторов  <br/> |
   
Если клиент не получает уведомления с сервера на определенный период времени, превышающее дважды времени, заданного параметром **StatusFrequency**, клиент должен выполнять действий, например повторного создания подписки. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
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
  
[Водяной знак](watermark.md)

