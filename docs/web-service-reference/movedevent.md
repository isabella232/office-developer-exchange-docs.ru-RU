---
title: MovedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MovedEvent
api_type:
- schema
ms.assetid: 572f8b40-dfa8-47bc-b0c1-e1a7138506fd
description: MovedEvent элемент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую.
ms.openlocfilehash: a375f421ca9159103e47b515729316b21149c68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834479"
---
# <a name="movedevent"></a>MovedEvent

**MovedEvent** элемент представляет событие, в котором элемент или папка перемещаются из одной родительской папки в другую. 
  
```xml
<MovedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldItemId/>
   <OldParentFolderId/>
</MovedEvent>
```

 **MovedCopiedEventType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Водяной знак](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика.  <br/> |
|[Метка времени](timestamp.md) <br/> |Представляет метка времени события перемещения элемента или временная папка почтового ящика.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор перемещенной папки.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Представляет идентификатор перемещаемый элемент.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор папка, содержащая перемещенный элемент или папку.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Содержит идентификатор папки исходной папки, прежде чем он был перемещен или скопирован.  <br/> |
|[OldItemId](olditemid.md) <br/> |Содержит уникальный идентификатор исходного элемента, прежде чем был перемещен.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Содержит идентификатор исходной родительской папки, элемента или папки, который был перемещен.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Уведомление](notification-ex15websvcsotherref.md) <br/> |Содержит сведения о подписке и события, произошедшие с момента последнего уведомления.  <br/> |
   
## <a name="remarks"></a>Замечания

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

