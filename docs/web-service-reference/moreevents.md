---
title: MoreEvents
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoreEvents
api_type:
- schema
ms.assetid: 76a7ea58-a44f-49b8-baba-d21302d742ad
description: Элемент MoreEvents определяет, есть ли дополнительные события в очереди доставки для клиента.
ms.openlocfilehash: cc3f7ed3b4b5f5ce27a9d45d508506bfa62e5086
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834489"
---
# <a name="moreevents"></a>MoreEvents

Элемент **MoreEvents** определяет, есть ли дополнительные события в очереди доставки для клиента. 
  
```xml
<MoreEvents/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение представляет значение типа Boolean. Значение **true** указывает, что другие события в очереди. Значение **false** указывает, что не другие события в очереди. Это свойство доступно только для чтения. 
  
## <a name="remarks"></a>Замечания

В случае оповещения о репликации по запросу значение **true** в этот элемент указывает клиенту, что другой запрос GetEvents должно быть выдано для получения оставшихся событий. При условии, что спецификации клиента требуют минимальные задержки уведомлений о событиях, пока не будет возвращено **значение false,** **MoreEvents** значение GetEvents запросы должны продолжать в непрерывной последовательности. 
  
В случае Push-уведомлений значение **true** для **MoreEvents** указывает клиенту, что другой запрос уведомления будут отправляться клиенту для доставки оставшихся событий. Как и уведомления по запросу, эти запросы по обработке результатов будет продолжаться в непрерывной последовательности до пуст очередь событий на сервере клиентского доступа. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
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

