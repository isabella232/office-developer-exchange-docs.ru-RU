---
title: PhoneCallState
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PhoneCallState
api_type:
- schema
ms.assetid: ac009eb3-6334-49ce-82be-48fe83577f9c
description: Элемент PhoneCallState указывает текущее состояние для телефонного звонка.
ms.openlocfilehash: 8c0b8357b58826f18f05eb0fedc0865be1623c2b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59528304"
---
# <a name="phonecallstate"></a>PhoneCallState

Элемент **PhoneCallState** указывает текущее состояние для телефонного звонка. 
  
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
|[PhoneCallInformation](phonecallinformation.md) <br/> |Указывает сведения о состоянии для телефонного звонка.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **PhoneCallState.** 
  
**Значения элементов PhoneCallState**

|**Значение**|**Описание**|
|:-----|:-----|
|Idle  <br/> |Начальное состояние вызова.  <br/> |
|Connecting  <br/> |Система набирает этот вызов.  <br/> |
|Оповещено  <br/> |Вызов находится в состоянии оповещений (звонит телефон).  <br/> |
|Подключение  <br/> |Вызов находится в подключенной состоянии.  <br/> |
|Отключено  <br/> |Вызов отключен.  <br/> |
|Входящие  <br/> |Вызов входящий.  <br/> |
|Перенос  <br/> |Вызов передается в другое место назначения.  <br/> |
|Переададка  <br/> |Вызов перенаправлен в другое место.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в каталоге /ews/directory компьютера, который работает Microsoft Exchange Server 2010 г., где установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

