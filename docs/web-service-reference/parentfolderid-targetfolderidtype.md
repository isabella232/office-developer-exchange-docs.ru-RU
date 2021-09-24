---
title: ParentFolderId (TargetFolderIdType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ParentFolderId
api_type:
- schema
ms.assetid: 0e3e6e5f-06d0-499b-8ca4-d36036521658
description: Элемент ParentFolderId определяет папку, в которой создается новая папка, или папку для поиска операции FindConversation.
ms.openlocfilehash: 53a5721b2c20c211a61b7e71b2e4f636700456b4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524625"
---
# <a name="parentfolderid-targetfolderidtype"></a>ParentFolderId (TargetFolderIdType)

Элемент **ParentFolderId** определяет папку, в которой создается новая папка, или папку для поиска операции [FindConversation.](findconversation-operation.md)
  
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

**TargetFolderIdType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

Элемент **ParentFolderId содержит** два детских элемента. Детские элементы являются взаимоисключающими в схеме. 
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит необходимый идентификатор и необязательный ключ изменения папки, в которой создается новая папка, или папку, которая будет искать для операции [FindConversation.](findconversation-operation.md) Использование этого элемента исключает использование элемента [DistinguishedFolderId.](distinguishedfolderid.md)  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Определяет папки Microsoft Exchange Server 2007 года. Использование этого элемента исключает использование элемента [FolderId.](folderid.md)  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в Exchange базе данных.  <br/> Ниже приводится выражение XPath к этому элементу:  `/CreateFolder` <br/> |
|[FindConversation](findconversation.md) <br/> |Определяет запрос на поиск бесед в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Два детских элемента используются для определения папки, которая будет содержать новую папку. Чтобы определить родительную папку новой папки, необходимо выбрать элемент [FolderId](folderid.md) или [Элемент DistinguishedFolderId.](distinguishedfolderid.md) Вы не можете использовать оба элемента одновременно. Этот элемент необходим для создания папок. 
  
Элемент [ParentFolderId](parentfolderid.md) описывает расположение существующих элементов и папок. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|Имя схемы  <br/> |Схема сообщения  <br/> |
|Файл проверки  <br/> |Messages.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция CreateFolder](createfolder-operation.md)
- [Операция FindConversation](findconversation-operation.md)
- [Создание папок (Exchange веб-служб)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

