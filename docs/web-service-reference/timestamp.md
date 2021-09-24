---
title: TimeStamp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeStamp
api_type:
- schema
ms.assetid: 5eae859a-5a74-4bf6-b196-d1b2fd38501a
description: Элемент Timestamp представляет время события почтовых ящиков.
ms.openlocfilehash: 87264f25cb8902d7306e1c8c42bef600520175be
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531377"
---
# <a name="timestamp"></a>TimeStamp

Элемент **Timestamp** представляет время события почтовых ящиков. 
  
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
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[CreatedEvent](createdevent.md) <br/> |Представляет событие, в котором создается элемент или папка.  <br/> |
|[DeletedEvent](deletedevent.md) <br/> |Представляет событие, в котором элемент или папка удаляются.  <br/> |
|[ModifiedEvent](modifiedevent.md) <br/> |Представляет событие, в котором элемент или папка изменены.  <br/> |
|[MovedEvent](movedevent.md) <br/> |Представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую родительную.  <br/> |
|[NewMailEvent](newmailevent.md) <br/> |Представляет событие, инициированное новым элементом почты в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Это свойство доступно только для чтения.
  
## <a name="remarks"></a>Заметки

Этот элемент в первую очередь доступен для использования в определении клиентом частоты событий. Это не присутствует в [StatusEvent](statusevent.md).
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
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

