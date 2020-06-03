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
description: Элемент Фолдерчанже представляет коллекцию изменений, которые необходимо выполнить для одной папки.
ms.openlocfilehash: e4a025bef100fdd478be545b6448b15886e47c60
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530241"
---
# <a name="folderchange"></a>FolderChange

Элемент **фолдерчанже** представляет коллекцию изменений, которые необходимо выполнить для одной папки. 
  
- [UpdateFolder](updatefolder.md) 
- [фолдерчанжес](folderchanges.md) 
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

**фолдерчанжетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки, которую требуется обновить.  <br/> |
|[дистингуишедфолдерид](distinguishedfolderid.md) <br/> |Определяет Майкрософт Exchange Server 2007 папок, на которые можно ссылаться по имени.  <br/> |
|[Обновления (папка)](updates-folder.md) <br/> |Определяет тип обновления, выполняемого для папки, которая идентифицируется с помощью элемента [FolderId](folderid.md) или [дистингуишедфолдерид](distinguishedfolderid.md) .  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[фолдерчанжес](folderchanges.md) <br/> |Представляет коллекцию изменений для папки.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/UpdateFolder/FolderChanges` <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server 2007 с ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateFolder](updatefolder-operation.md)

