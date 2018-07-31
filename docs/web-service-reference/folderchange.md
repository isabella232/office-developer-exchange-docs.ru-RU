---
title: FolderChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderChange
api_type:
- schema
ms.assetid: 23279750-131b-4e1a-b7d1-be235c4e0891
description: Элемент FolderChange представляет коллекцию изменений выполняется на одной папке.
ms.openlocfilehash: f25defa9974f7b5dd0c683c7657983741890d45d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354332"
---
# <a name="folderchange"></a>FolderChange

Элемент **FolderChange** представляет коллекцию изменений выполняется на одной папке. 
  
- [UpdateFolder](updatefolder.md) 
- [FolderChanges](folderchanges.md) 
- [FolderChange](folderchange.md)
  
```xml
<FolderChange>
   <FolderId/>
   <Updates/>
</FolderChange>
```

```xml
<FolderChange>
   <DistinguishedFolderId/>
   <Updates/>
</FolderChange>
```

**FolderChangeType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки для обновления.  <br/> |
|[DistinguishedFolderId](distinguishedfolderid.md) <br/> |Идентифицирует MicrosoftExchange Server 2007 папок, которые можно ссылаться по имени.  <br/> |
|[Updates (Folder)](updates-folder.md) <br/> |Определяет тип обновления, который выполняется на папку, определяемую средством параметр [FolderId](folderid.md) или [DistinguishedFolderId](distinguishedfolderid.md) элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderChanges](folderchanges.md) <br/> |Представляет коллекцию изменений для папки.  <br/> Ниже приведен выражение XPath для этого элемента.  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server 2007 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateFolder](updatefolder-operation.md)

