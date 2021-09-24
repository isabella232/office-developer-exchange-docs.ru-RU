---
title: SubscriptionId (GetEvents)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: Элемент SubscriptionId представляет идентификатор подписки.
ms.openlocfilehash: c24ae8dc61fa98716efc38d7a2500cab503760b2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522588"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (GetEvents)

Элемент **SubscriptionId** представляет идентификатор подписки. 
  
```xml
<SubscriptionId/>
```

 **SubscriptionIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |Представляет операцию, используемую клиентами для запроса уведомлений с сервера.  <br/> |
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
|[SubscribeResponseMessage](subscriberesponsemessage.md) <br/> |Содержит состояние и результат запроса подписки.  <br/> |
|[Отмена подписки](unsubscribe.md) <br/> |Содержит свойства, используемые для отписки из подписки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение — GUID.
  
## <a name="remarks"></a>Заметки

GUID, который представляет идентификатор подписки, создается сервером клиентского доступа после создания подписки.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)

