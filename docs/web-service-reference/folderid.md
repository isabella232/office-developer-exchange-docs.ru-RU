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
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762625"
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
|Id  <br/> |Содержит строку, которая определяет папке в хранилище Exchange. Этот атрибут является обязательным.  <br/> |
|ChangeKey  <br/> |Содержит строку, которая определяет к папке, которая определена в атрибуте Id версии. Этот атрибут является необязательным. Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, предназначенное для действий, использующих папок.  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |Представляет событие, в котором копирование элемента или папки.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Определяет папку назначения для копирования и перемещения действия.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Определяет папку, где создается на новую папку или элемент.  <br/><br/>  Ниже приведены выражения XPath для этого элемента.<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Представляет коллекцию папок, которые будут получены для определения содержимого папки поиска.  <br/> |
|[Удаление (FolderSync)](delete-foldersync.md) <br/> |Определяет одну папку для удаления в локальном хранилище клиента.  <br/> |
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку Календарь в почтовом ящике.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений выполняется на одной папке.  <br/> Ниже приведен выражение XPath для этого элемента.`/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папке контактов в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[ToFolderId](tofolderid.md) <br/> | Представляет конечной папки для копируемые или перемещения элемента или папки. <br/> <br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.  <br/><br/>  Ниже приведены выражения XPath для этого элемента. <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, содержащую элементы для синхронизации.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Определение идентификатора к папке, где будет скопировано элементов электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Определение идентификатора к папке, где планируется переместить сообщения электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Все элементы **FolderId** , типа **FolderIdType** . Элемент **FolderId** является обязательным во всех случаях, за исключением в элементах, тип которого расширяет **BaseFolderType** или где **FolderId** элемент является частью выбор. Просмотрите схемы для получения дополнительных сведений. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание папки (веб-служб Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

