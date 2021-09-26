---
title: Папки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Элемент Folders содержит массив папок, используемых в операциях папок.
ms.openlocfilehash: 77442965c9d372a2895404cf1c919be38e98abb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546436"
---
# <a name="folders"></a>Folders

Элемент **Folders** содержит массив папок, используемых в операциях папок. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

**ArrayOfFoldersType** или **NonEmptyArrayOfFoldersType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Определяет папку для создания, получения, поиска, синхронизации или обновления.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, которая в основном содержит элементы календаря.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку Контакты в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку Поиска, содержаную в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку Задачи в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CopyFolder.](copyfolder-operation.md)  <br/> |
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в Exchange магазине.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateFolder.](createfolder-operation.md)  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateManagedFolder.](createmanagedfolder-operation.md)  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [GetFolder.](getfolder-operation.md)  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат запроса на операцию [MoveFolder.](movefolder-operation.md)  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Определяет папку, в которой создается новая папка.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Содержит результаты поиска одной корневой папки во время операции [FindFolder.](findfolder-operation.md)  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции UpdateFolder.](updatefolder-operation.md)  <br/> |
   
## <a name="remarks"></a>Заметки

Этот элемент является обязательной детской частью элемента [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2010, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

