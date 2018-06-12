---
title: PhoneCallState
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
description: Элемент PhoneCallState указывает текущее состояние телефонного звонка.
ms.openlocfilehash: 184a7400810711442e565d1ef37094bd63b00914
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834761"
---
# <a name="phonecallstate"></a>PhoneCallState

Элемент **PhoneCallState** указывает текущее состояние телефонного звонка. 
  
```xml
<PhoneCallState>Idle or Connecting or Alerted or Connected or Disconnected or Incoming or Transferring or Forwarding</PhoneCallState>
```

 **PhoneCallStateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PhoneCallInformation](phonecallinformation.md) <br/> |Задает сведения о состоянии для телефонного звонка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **PhoneCallState** . 
  
**Значения элементов PhoneCallState**

|**Значение**|**Описание**|
|:-----|:-----|
|Простоя  <br/> |Состояние первого вызова.  <br/> |
|Подключение  <br/> |Система — это набору номера, этот вызов.  <br/> |
|Оповещения  <br/> |Вызов выполнен в элемент интерфейса, предупреждающий состояние (телефонных звонков).  <br/> |
|Подключено  <br/> |Вызов выполнен в состояние подключения.  <br/> |
|Отключено  <br/> |Вызов разъединен.  <br/> |
|Входящая  <br/> |Входящий звонок.  <br/> |
|Передача  <br/> |Звонок переводится другому получателю.  <br/> |
|Переадресация  <br/> |Переадресация звонка другому получателю.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в каталоге /ews/ компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

