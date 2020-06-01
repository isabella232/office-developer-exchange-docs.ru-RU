---
title: фонекаллстате
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: Элемент Фонекаллстате указывает текущее состояние телефонного звонка.
ms.openlocfilehash: d2088b9b2811befe80684188d49c8034c577cc55
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468532"
---
# <a name="phonecallstate"></a>фонекаллстате

Элемент **фонекаллстате** указывает текущее состояние телефонного звонка. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **фонекаллстатетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фонекаллинформатион](phonecallinformation.md) <br/> |Задает сведения о состоянии для телефонного звонка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **фонекаллстате** . 
  
**Значения элементов Фонекаллстате**

|**Значение**|**Описание**|
|:-----|:-----|
|Простоя  <br/> |Начальное состояние вызова.  <br/> |
|Connecting  <br/> |Система набирает этот вызов.  <br/> |
|Предупрежден  <br/> |Вызов находится в состоянии оповещения (телефонный звонок).  <br/> |
|Подключено  <br/> |Вызов находится в подключенном состоянии.  <br/> |
|Отключено  <br/> |Вызов отключается.  <br/> |
|Входящее  <br/> |Вызов является входящим.  <br/> |
|Мещают  <br/> |Вызов передается в другой целевой объект.  <br/> |
|Сообщений  <br/> |Вызов перенаправляется в другую точку назначения.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в каталоге/ЕВС/компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

