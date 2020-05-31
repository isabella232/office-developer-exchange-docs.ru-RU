---
title: тофолдерид
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
description: Элемент Тофолдерид представляет папку назначения для скопированного или перемещенного элемента или папки.
ms.openlocfilehash: 9d2fd6c177711cfe3a5d3415320440259e2f5289
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353660"
---
# <a name="tofolderid"></a>тофолдерид

Элемент **тофолдерид** представляет папку назначения для скопированного или перемещенного элемента или папки. 
  
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

**таржетфолдеридтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор папки назначения для скопированного или перемещенного элемента или папки.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет именованную папку назначения для скопированного или перемещенного элемента или папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[MoveFolder](movefolder.md) <br/> |Определяет запрос на перемещение папки в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/MoveFolder` <br/> |
|[CopyFolder](copyfolder.md) <br/> |Определяет запрос на копирование папки в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CopyFolder` <br/> |
|[MoveItem](moveitem.md) <br/> |Определяет запрос на перемещение элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/MoveItem` <br/> |
|[CopyItem](copyitem.md) <br/> |Определяет запрос на копирование элемента в хранилище Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/CopyItem` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема Messages  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция MoveFolder](movefolder-operation.md)  
- [Операция CopyFolder](copyfolder-operation.md) 
- [Операция MoveItem](moveitem-operation.md) 
- [Операция CopyItem](copyitem-operation.md)

