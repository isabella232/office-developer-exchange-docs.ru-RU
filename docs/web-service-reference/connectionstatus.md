---
title: ConnectionStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConnectionStatus
api_type:
- schema
ms.assetid: 4300f9d6-8bf9-48c2-9f07-d80197864e17
description: Элемент ConnectionStatus предоставляет текстовое описание состояния попотоковой подписки.
ms.openlocfilehash: 928537201041950011ae06444e3c412228d252ea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462719"
---
# <a name="connectionstatus"></a>ConnectionStatus

Элемент **ConnectionStatus** предоставляет текстовое описание состояния попотоковой подписки. 
  
```xml
<ConnectionStatus>OK or Closed</ConnectionStatus>
```

 **коннектионстатустипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[жетстреаминжевентсреспонсемессаже](getstreamingeventsresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции GetStreamingEvents](getstreamingevents-operation.md) .  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Необходимо указать текстовое значение. Ниже приведены возможные текстовые значения для этого элемента:
  
- OK
    
- Закрыто
    
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



[Операция GetStreamingEvents](getstreamingevents-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

