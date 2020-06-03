---
title: SubscriptionId (Events)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscriptionId
api_type:
- schema
ms.assetid: 77c0abab-69e8-428e-8c20-22258e4ef71b
description: Элемент SubscriptionId представляет идентификатор для подписки.
ms.openlocfilehash: e103386f466d65717878b4a6c811f3c3ad6e7c7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465354"
---
# <a name="subscriptionid-getevents"></a>SubscriptionId (Events)

Элемент **SubscriptionId** представляет идентификатор для подписки. 
  
```xml
<SubscriptionId/>
```

 **субскриптионидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GetEvents](getevents.md) <br/> |Представляет операцию, используемую клиентами опрашивающей репликации для запроса уведомлений с сервера.  <br/> |
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
|[субскрибереспонсемессаже](subscriberesponsemessage.md) <br/> |Содержит состояние и результат запроса на подписку.  <br/> |
|[Отмена подписки](unsubscribe.md) <br/> |Содержит свойства, используемые для отмены подписки на подписку.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Текстовое значение — GUID.
  
## <a name="remarks"></a>Примечания

Идентификатор GUID, представляющий идентификатор подписки, создается сервером клиентского доступа при создании подписки.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |схема сообщений  <br/> |
|Файл проверки  <br/> |messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

