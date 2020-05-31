---
title: Уведомления
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Notifications
api_type:
- schema
ms.assetid: 153cc420-d2fe-42f1-afb2-9a31ee09a750
description: Элемент Notifications содержит массив сведений о подписке и событиях, произошедших с момента последнего уведомления.
ms.openlocfilehash: f576bf579c91b77dcde8646a6af7fdc47145aef7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834550"
---
# <a name="notifications"></a>Уведомления

Элемент **Notifications** содержит массив сведений о подписке и событиях, произошедших с момента последнего уведомления. 
  
```xml
<Notifications>
   <Notification/>
</Notifications>
```

 **нонемптяррайофнотификатионстипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетстреаминжевентсреспонсемессаже](getstreamingeventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Namespace  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages и http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема сообщений; Схема Types  <br/> |
|Файл проверки  <br/> |Messages. xsd; Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция GetFolder](getfolder-operation.md)
  
[Операция DeleteFolder](deletefolder-operation.md)
  
[Операция MoveFolder](movefolder-operation.md)
  
[Операция CopyFolder](copyfolder-operation.md)
  
[Операции подписки](subscribe-operation.md)

