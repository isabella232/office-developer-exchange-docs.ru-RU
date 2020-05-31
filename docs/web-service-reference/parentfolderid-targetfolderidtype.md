---
title: ParentFolderId (Таржетфолдеридтипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: Элемент ParentFolderId определяет папку, в которой создается новая папка, или папку для поиска операции FindConversation.
ms.openlocfilehash: 8e80b9b342274a8b2004838ebd16f8425a2d3fa3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353828"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (Таржетфолдеридтипе)

Элемент **ParentFolderId** определяет папку, в которой создается новая папка, или папку для поиска [операции FindConversation](findconversation-operation.md).
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

```xml
<ParentFolderId>
   <FolderId/> 
</ParentFolderId>
```

**таржетфолдеридтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

Элемент **ParentFolderId** содержит два дочерних элемента. Дочерние элементы в схеме являются взаимоисключающими. 
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит обязательный идентификатор и необязательный ключ изменения папки, в которой создается новая папка, или папки, в которой выполняется поиск [операции FindConversation](findconversation-operation.md). Использование этого элемента исключает использование элемента [дистингуишедфолдерид](distinguishedfolderid.md) .  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет стандартные папки Microsoft Exchange Server 2007. Использование этого элемента исключает использование элемента [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в базе данных Exchange.  <br/> Ниже приведено выражение XPath для этого элемента:`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Два дочерних элемента используются для определения папки, которая будет содержать новую папку. Чтобы определить родительскую папку для новой папки, необходимо выбрать элемент [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) . Одновременное использование обоих элементов невозможно. Этот элемент необходим для создания папок. 
  
Элемент [ParentFolderId](parentfolderid.md) описывает расположение существующих элементов и папок. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateFolder](createfolder-operation.md)
- [Операция FindConversation](findconversation-operation.md)
- [Создание папок (веб-службы Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

