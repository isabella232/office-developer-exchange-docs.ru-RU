---
title: ParentFolderId (TargetFolderIdType)
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
description: Элемент ParentFolderId определяет папку, в которой будет создана новая папка или папки для поиска FindConversation операции.
ms.openlocfilehash: 61072e1dd3321beb5f3b76d9accf20530b443796
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834686"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

Элемент **ParentFolderId** определяет папку, в которой будет создана новая папка или папки для поиска [FindConversation операции](findconversation-operation.md).
  
```xml
<ParentFolderId>
   <DistinguishedFolderId/>
</ParentFolderId>
```

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

Элемент **ParentFolderId** содержит два дочерних элементов. Дочерние элементы являются взаимоисключающими в схеме. 
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит обязательного элемента identifier и ключ необязательно изменения папки, в которой будет создана новая папка или к папке, где выполняется поиск [FindConversation операции](findconversation-operation.md). С помощью этого элемента исключает использование элемента [DistinguishedFolderId](distinguishedfolderid.md) .  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует папок Microsoft Exchange Server 2007 по умолчанию. С помощью этого элемента исключает использование элемента [FolderId](folderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в базе данных Exchange.  <br/> Ниже приведен выражение XPath для этого элемента.`/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовый ящик.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Два дочерние элементы используются для определения папки, которая будет содержать новую папку. Необходимо выбрать [FolderId](folderid.md) или элемент [DistinguishedFolderId](distinguishedfolderid.md) для определения родительской папки новую папку. Нельзя использовать оба этих элемента в то же время. Этот элемент необходим для создания папки. 
  
Элемент [ParentFolderId](parentfolderid.md) описывает расположение существующих элементов и папок. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [CreateFolder Operation](createfolder-operation.md)
- [FindConversation Operation](findconversation-operation.md)
- [Создание папки (веб-служб Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

