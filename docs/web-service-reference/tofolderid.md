---
title: ToFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ToFolderId
api_type:
- schema
ms.assetid: bd6a4265-ad40-43f6-bcc4-0bf5df4e984c
description: Элемент ToFolderId представляет папку назначения для скопированного или перемещенного элемента или папки.
ms.openlocfilehash: b58192aa4d1ffe609da78dfdf1b5c86522fc45c8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515168"
---
# <a name="tofolderid"></a>ToFolderId

Элемент **ToFolderId** представляет папку назначения для скопированного или перемещенного элемента или папки. 
  
```xml
<ToFolderId>
   <FolderId/>
</ToFolderId>
```

```xml
<ToFolderId>
   <DistinguishedFolderId/>
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
|[FolderId](folderid.md) <br/> |Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет именоваемую папку назначения для скопированного или перемещенного элемента или папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение папки в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос на копирование папки в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элемента в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элемента в Exchange магазине.  <br/> Ниже приводится выражение XPath к этому элементу:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция MoveFolder](movefolder-operation.md)  
- [Операция CopyFolder](copyfolder-operation.md) 
- [Операция MoveItem](moveitem-operation.md) 
- [Операция CopyItem](copyitem-operation.md)

