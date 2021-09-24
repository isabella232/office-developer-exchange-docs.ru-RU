---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Элемент Folder определяет папку для создания, получения, поиска, синхронизации или обновления.
ms.openlocfilehash: 5b6b8eb1d53c84bc3d0484d1c868470137db492d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530383"
---
# <a name="folder"></a>Folder

Элемент **Folder** определяет папку для создания, получения, поиска, синхронизации или обновления. 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 **FolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит папку.  <br/> |
|[FolderClass](folderclass.md) <br/> |Представляет класс папки для данной папки.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Содержит отображаемую папку.  <br/> |
|[TotalCount](totalcount.md) <br/> |Представляет общее количество элементов в данной папке.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Представляет количество детских папок, содержащихся в папке. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства в папках.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемой папке.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Представляет количество непрочитанные элементы в данной папке.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для приложения к свойству папки во время операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |Определяет одну папку, создаемую в локальном клиентской магазине.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление одного свойства в папке в операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном клиентской магазине.  <br/> |
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, используемых в операциях папок.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описываемая этим элементом, расположена в виртуальном каталоге компьютера EWS, который работает Exchange 2007 г., где установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

