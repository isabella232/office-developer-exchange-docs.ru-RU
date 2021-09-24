---
title: PushSubscriptionRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PushSubscriptionRequest
api_type:
- schema
ms.assetid: 70caa0ca-40a1-421f-b4e6-0658f22d0b8e
description: Элемент PushSubscriptionRequest представляет подписку на подписку на push-уведомление о событиях.
ms.openlocfilehash: 6eb76bba92e78e048ae97dbec5fc6c4d698a815f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523729"
---
# <a name="pushsubscriptionrequest"></a>PushSubscriptionRequest

Элемент **PushSubscriptionRequest** представляет подписку на подписку на push-уведомление о событиях. 
  
[Subscribe](subscribe.md)
  
[PushSubscriptionRequest](pushsubscriptionrequest.md)
  
```XML
<PushSubscriptionRequest SubscribeToAllFolders="">
   <FolderIds/>
   <EventTypes/>
   <Watermark/>
   <StatusFrequency/>
   <URL/>
</PushSubscriptionRequest>
```

 **PushSubscriptionRequestType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**SubscribeToAllFolders** <br/> |Указывает, следует ли подписываться на все доступные папки. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, используемых для идентификации папок для мониторинга уведомлений о событиях.  <br/> |
|[EventTypes](eventtypes.md) <br/> |Содержит коллекцию уведомлений о событиях, используемых для создания подписки.  <br/> |
|[Watermark](watermark.md) <br/> |Представляет закладки событий в таблице событий почтового ящика. Это используется для создания подписки, начиная с события, представленного водяной знак. Если водяной знак из запроса Подписка не найден, клиенту будет возвращен ответ на ошибку. Это может произойти, если водяной знак старше 30 дней или если водяной знак никогда не присутствовал в почтовом ящике.  <br/> |
|[StatusFrequency](statusfrequency.md) <br/> |Представляет частоту, указанную в минутах, при которой сообщения уведомлений будут отправляться клиенту, если события не произошли.  <br/> |
|[URL-адрес ](url-ex15websvcsotherref.md) <br/> |Представляет расположение клиентской веб-службы для push-уведомлений.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Subscribe](subscribe.md) <br/> |Содержит свойства, используемые для создания подписок.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция Unsubscribe](unsubscribe-operation.md)

