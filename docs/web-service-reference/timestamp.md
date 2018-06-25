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
description: Метка времени элемент представляет метка времени события почтового ящика.
ms.openlocfilehash: d020d9a4cf3a128d26e0ff2b83be9f3deb024339
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840231"
---
# <a name="timestamp"></a>Метка времени

**Метка времени** элемент представляет метка времени события почтового ящика. 
  
```xml
<TimeStamp/>
```

 **DateTime**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, куда копируются элемента или папки.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, где создается элемент или папку.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, где удаления элемента или папки.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, где при изменении элемента или папки.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, где элемента или папки перемещаются из одной родительской папки в другую.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет события, вызванные нового элемента почты в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Замечания

Этот элемент в первую очередь доступна для использования в клиентских определения частоты событий. Это не указан в [StatusEvent](statusevent.md).
  
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

