---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: Элемент FolderId содержит идентификатор и ключ изменения папки.
ms.openlocfilehash: 7348fb7342bf33d487591a9daf93a9570f7552f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513684"
---
# <a name="folderid"></a>FolderId

Элемент **FolderId** содержит идентификатор и ключ изменения папки. 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|Id  <br/> |Содержит строку, которая идентифицирует папку в Exchange магазине. Этот атрибут является обязательным.  <br/> |
|ChangeKey  <br/> |Содержит строку, определяемую версией папки, идентифицируемой атрибутом Id. Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, которая ориентирована на действия, которые используют папки.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копируется элемент или папка.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Указывает папку назначения для копирования и перемещения действий.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Определяет папку, в которой создается новая папка или элемент.  <br/><br/>  Ниже приводится выражение XPath к этому элементу:<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Представляет коллекцию папок, которые будут заминированы для определения содержимого папки поиска.  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |Определяет одну папку, удаляемую в локальном клиентном магазине.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку календаря в почтовом ящике.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений, выполняемых в одной папке.  <br/> Ниже приводится выражение XPath к этому элементу:  `/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[ToFolderId](tofolderid.md) <br/> | Представляет папку назначения для скопированного или перемещенного элемента или папки. <br/> <br/>  Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.  <br/><br/>  Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, которая содержит элементы для синхронизации.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определяет идентификатор папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определяет идентификатор папки, в которую будут перемещены элементы электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Все **элементы FolderId** имеют тип **FolderIdType.** Элемент **FolderId** требуется в каждом случае, за исключением элементов, тип которых расширяет **BaseFolderType** или где элемент **FolderId** является частью выбора. Просмотрите схему для получения дополнительных сведений. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание папок (Exchange веб-служб)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

