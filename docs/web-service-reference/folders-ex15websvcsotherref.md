---
title: Папки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Элемент папки содержит массив папки, которые используются в операциях папки.
ms.openlocfilehash: e1b9e337f633dbf6fda159c28725d3fb8dcd55a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762628"
---
# <a name="folders"></a>Папки

Элемент **папки** содержит массив папки, которые используются в операциях папки. 
  
```xml
<Folders>
   <Folder/>
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
|[Folder](folder.md) <br/> |Определяет папку для создания, получение, найти, синхронизировать или обновить.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, содержащую элементы календаря в первую очередь.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащихся в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задачи в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CopyFolder операции](copyfolder-operation.md) .  <br/> |
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в хранилище Exchange.  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CreateFolder операции](createfolder-operation.md) .  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [CreateManagedFolder операции](createmanagedfolder-operation.md) .  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |Содержит состояние и результат [операции GetFolder](getfolder-operation.md) запроса.  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |Содержит состояние и результат [операции MoveFolder](movefolder-operation.md) запроса.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |Указывает папку, где будет создана новая папка.  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [UpdateFolder операции](updatefolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Замечания

Этот элемент является обязательным дочерним элементом элемента [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) . 
  
Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server 2010 с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

