---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: Элемент FolderId содержит идентификатор и ключ изменения папки.
ms.openlocfilehash: 7aa5070fa7a2c51303c7159de04fe277f909a874
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461389"
---
# <a name="folderid"></a>FolderId

Элемент **FolderId** содержит идентификатор и ключ изменения папки. 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **фолдеридтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Содержит строку, определяющую папку в хранилище Exchange. Этот атрибут является обязательным.  <br/> |
|чанжекэй  <br/> |Содержит строку, определяющую версию папки, определяемую атрибутом ID. Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[контекстфолдерид](contextfolderid.md) <br/> |Указывает папку, предназначенную для действий, в которых используются папки.  <br/> |
|[копиедевент](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[дестинатионфолдерид](destinationfolderid.md) <br/> |Указывает целевую папку для действий по копированию и перемещению.  <br/> |
|[ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) <br/> | Определяет папку, в которой создается новая папка или элемент.  <br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[басефолдеридс](basefolderids.md) <br/> |Представляет коллекцию папок, которые будут mined для определения содержимого папки поиска.  <br/> |
|[Delete (Фолдерсинк)](delete-foldersync.md) <br/> |Определяет одну папку для удаления в локальном хранилище клиента.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку "Календарь" в почтовом ящике.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений, выполняемых над одной папкой.  <br/> Ниже приведено выражение XPath для этого элемента:`/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[тофолдерид](tofolderid.md) <br/> | Представляет папку назначения для скопированного или перемещенного элемента или папки. <br/> <br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[саведитемфолдерид](saveditemfolderid.md) <br/> | Определяет целевую папку для операций обновления, отправки и создания элементов в хранилище Exchange.  <br/><br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[синкфолдерид](syncfolderid.md) <br/> |Представляет папку, содержащую синхронизируемые элементы.  <br/> |
|[усерконфигуратионнаме](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Все элементы **FolderId** имеют тип **фолдеридтипе** . Элемент **FolderId** является обязательным для каждого случая, за исключением элементов, тип которых расширяет **басефолдертипе** или где элемент **FolderId** является частью выбора. Просмотрите схему, чтобы получить дополнительные сведения. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание папок (веб-службы Exchange)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

