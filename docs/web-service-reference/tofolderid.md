---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: Элемент ToFolderId представляет конечной папки для копируемые или перемещения элемента или папки.
ms.openlocfilehash: a48309f0b7f5c9bf667fc2eb653a0502832bc996
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840198"
---
# <a name="tofolderid"></a>ToFolderId

Элемент **ToFolderId** представляет конечной папки для копируемые или перемещения элемента или папки. 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

 **TargetFolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор конечной папки для копируемые или перемещения элемента или папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет именованный конечной папки для копируемые или перемещения элемента или папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение в папку в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос для копирования в папку в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элемента в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос для копирования элемента в хранилище Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция MoveFolder](movefolder-operation.md)
  
[Операция CopyFolder](copyfolder-operation.md)
  
[MoveItem Operation](moveitem-operation.md)
  
[CopyItem Operation](copyitem-operation.md)

