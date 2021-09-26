---
title: PreviousWatermark
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PreviousWatermark
api_type:
- schema
ms.assetid: 474f4f7c-47da-47d4-8126-230012172fb5
description: Элемент PreviousWatermark представляет водяной знак последнего события, которое было успешно доведено до клиента для подписки.
ms.openlocfilehash: c46e18c7a58405fe2149666531cb2af773110816
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543025"
---
# <a name="previouswatermark"></a>PreviousWatermark

Элемент **PreviousWatermark** представляет водяной знак последнего события, которое было успешно доведено до клиента для подписки. 
  
```xml
<PreviousWatermark/>
```

 **WatermarkType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и событиях, произошедших с момента последнего уведомления.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Требуется текстовое значение. Текстовое значение представляет собой последний водяной знак. Текстовое значение не может быть пустой строкой.
  
## <a name="remarks"></a>Заметки

Свойство **PreviousWatermark** полезно клиенту при определении последнего успешного уведомления. Например, если подписка имеет три события с водяными знаками 1, 2 и 3, а следующее уведомление отправляется со значением **PreviousWatermark** 3, клиент может сравнить это значение со значением Водяной знак последнего полученного уведомления. Это позволяет клиенту обеспечить непрерывность событий. 
  
Для push-клиентов **previousWatermark** сравнивается с локальным последним известным водяном знаком на стороне клиента. Если значения отличаются, клиент пропустил уведомление о событии и должен восстановить подписку с помощью последнего локального водяного знака. Например, если клиент push получает три события для подписки с водяными знаками 1, 2 и 3, а следующее уведомление поставляется со значением **PreviousWatermark** 5, клиент пропустил по крайней мере одно уведомление и должен создать новую подписку, передав 3 в качестве водяного знака. 
  
В случае клиента с тягой значение **PreviousWatermark** будет [](watermark.md) таким же, как и водяной знак, включенный клиентом в вызов GetEvents. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
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

