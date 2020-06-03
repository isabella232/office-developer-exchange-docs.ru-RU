---
title: стреамингсубскриптионрекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StreamingSubscriptionRequest
api_type:
- schema
ms.assetid: d18f3b60-ebb6-4133-b895-a6ec8942d039
description: Элемент Стреамингсубскриптионрекуест представляет подписку на подписку на уведомление о событии потоковой передачи.
ms.openlocfilehash: b469ba7598420189c1db0e2fe676a279390eb6bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468231"
---
# <a name="streamingsubscriptionrequest"></a>стреамингсубскриптионрекуест

Элемент **стреамингсубскриптионрекуест** представляет подписку на подписку на уведомление о событии потоковой передачи. 
  
[Подписаться](subscribe.md)
  
[стреамингсубскриптионрекуест](streamingsubscriptionrequest.md)
  
```xml
<StreamingSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
</StreamingSubscriptionRequest>
```

 **стреамингсубскриптионрекуест**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**субскрибетоаллфолдерс** <br/> |Указывает, будет ли сервер подписываться на все папки в почтовом ящике пользователя. Значение **true** указывает на то, что сервер будет подписываться.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдеридс](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для определения папок, которые необходимо отслеживать для получения уведомлений о событиях.  <br/> |
|[евенттипес](eventtypes.md) <br/> |Содержит коллекцию уведомлений о событиях, которые используются для создания подписки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Подписаться](subscribe.md) <br/> |Содержит свойства, используемые для создания подписок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция GetStreamingEvents](getstreamingevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

