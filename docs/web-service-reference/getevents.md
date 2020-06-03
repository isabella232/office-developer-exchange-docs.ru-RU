---
title: GetEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEvents
api_type:
- schema
ms.assetid: 22d4da6b-d8a8-484f-82c4-3e4b8f5431cd
description: Элемент Events представляет операцию, используемую клиентами, запрашивающими уведомления от сервера.
ms.openlocfilehash: 004f782ccd32b3c5e501080bfc59419a6e7d9ce4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462502"
---
# <a name="getevents"></a>GetEvents

Элемент **Events** представляет операцию, используемую клиентами, запрашивающими уведомления от сервера. 
  
[GetEvents](getevents.md)
  
```xml
<GetEvents>
   <SubscriptionId/>
   <Watermark/>
</GetEvents>
```

 **жетевентстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[SubscriptionId (Events)](subscriptionid-getevents.md) <br/> |Представляет идентификатор подписки, запрашиваемой для событий.  <br/> |
|[Watermark](watermark.md) <br/> |Представляет последний водяной знак, возвращенный клиенту. Если для этой подписки не вызывались события для этой подписки, клиент использует водяной знак, возвращенный из запроса Subscribe. В противном случае используется водяной знак из последнего события в последнем ответе на событие.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |false  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

