---
title: CopiedEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopiedEvent
api_type:
- schema
ms.assetid: 82f2fcac-deaa-4ff8-801f-4fe28d8a19f5
description: CopiedEvent элемент представляет событие, в котором копирование элемента или папки.
ms.openlocfilehash: 7ebfbb744a80e3a2d14ee9e0e1b952d2269dbf94
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353170"
---
# <a name="copiedevent"></a>CopiedEvent

**CopiedEvent** элемент представляет событие, в котором копирование элемента или папки. 
  
```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <FolderId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

```xml
<CopiedEvent>
   <Watermark/>
   <TimeStamp/>
   <ItemId/>
   <ParentFolderId/>
   <OldFolderId/>
   <OldParentFolderId/>
</CopiedEvent>
```

**MovedCopiedEventType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Watermark](watermark.md) <br/> |Представляет закладку события в таблице событий почтового ящика.  <br/> |
|[TimeStamp](timestamp.md) <br/> |Представляет метка времени события почтового ящика копии элемента или папки.  <br/> |
|[FolderId](folderid.md) <br/> |Представляет идентификатор папки.  <br/> |
|[Идентификатор элемента](itemid.md) <br/> |Представляет идентификатор элемента.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор папки, содержащей эту копию.  <br/> |
|[OldFolderId](oldfolderid.md) <br/> |Представляет идентификатор папки исходной папки, перед его скопирован.  <br/> |
|[OldItemId](olditemid.md) <br/> |Содержит уникальный идентификатор исходного элемента, прежде чем был скопирован.  <br/> |
|[OldParentFolderId](oldparentfolderid.md) <br/> |Содержит идентификатор исходной родительской папки, элемента или папки, который скопирован.  <br/> |
   
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

- [Операции подписки](subscribe-operation.md) 
- [Операция GetEvents](getevents-operation.md) 
- [Отписаться операции](unsubscribe-operation.md)
- [С помощью подписки по запросу](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx) 
- [Пример приложения для push-уведомлений](http://msdn.microsoft.com/library/db1f8523-fa44-483f-bdb6-ab5939b52eee%28Office.15%29.aspx)

