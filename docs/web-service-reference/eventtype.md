---
title: EventType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EventType
api_type:
- schema
ms.assetid: 04b70f9e-c226-4130-958e-0db0275cf58b
description: Элемент EventType используется для создания подписки и определяет тип события, который должен быть указан в уведомлении.
ms.openlocfilehash: 58c7ce571434b6fb8ac0b1dc2a3f8cd4fd56ff17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526174"
---
# <a name="eventtype"></a>EventType

Элемент **EventType** используется для создания подписки и определяет тип события, который должен быть указан в уведомлении. 
  
```xml
<EventType/>
```

 **нотификатионевенттипетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[евенттипес](eventtypes.md) <br/> |Содержит коллекцию типов событий уведомления о событиях, которые используются для создания подписки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже перечислены возможные значения.
  
- копиедевент
    
- креатедевент
    
- делетедевент
    
- модифиедевент
    
- моведевент
    
- невмаилевент
    
- фрибусичанжедевент
    
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

