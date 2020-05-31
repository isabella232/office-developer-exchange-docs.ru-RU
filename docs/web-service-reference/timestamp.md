---
title: Метка времени
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: Элемент timestamp представляет метку времени события почтового ящика.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840231"
---
# <a name="timestamp"></a>Метка времени

Элемент **timestamp** представляет метку времени события почтового ящика. 
  
```xml
<TimeStamp/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[копиедевент](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[креатедевент](createdevent.md) <br/> |Представляет событие, в котором создается элемент или папка.  <br/> |
|[делетедевент](deletedevent.md) <br/> |Представляет событие, в котором удаляется элемент или папка.  <br/> |
|[модифиедевент](modifiedevent.md) <br/> |Представляет событие, в котором изменяется элемент или папка.  <br/> |
|[моведевент](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.  <br/> |
|[невмаилевент](newmailevent.md) <br/> |Представляет событие, инициированное новым почтовым элементом в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Примечания

Этот элемент в основном доступен для использования в определении клиента частоты событий. Отсутствует в [статусевент](statusevent.md).
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операции подписки](subscribe-operation.md)
  
[Операция GetEvents](getevents-operation.md)
  
[Операция по отмене подписки](unsubscribe-operation.md)

