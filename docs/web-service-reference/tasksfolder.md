---
title: TasksFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: Элемент TasksFolder представляет папку Tasks, которая содержится в почтовом ящике.
ms.openlocfilehash: 6c0225370dd4a4af700df9dd029c2e54154ad8e8
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543865"
---
# <a name="tasksfolder"></a>TasksFolder

Элемент **TasksFolder** представляет папку Tasks, которая содержится в почтовом ящике. 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

**TasksFolderType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки Задачи.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, которая содержит папку Задачи.  <br/> |
|[FolderClass](folderclass.md) <br/> |Представляет класс папки для папки Задачи.  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |Содержит имя отображения папки Задачи.  <br/> |
|[TotalCount](totalcount.md) <br/> |Представляет общее количество элементов в папке Задачи.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Представляет количество детских папок, содержащихся в папке Задачи. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства в папке Задачи.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемой папке.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Представляет количество непрочитанные элементы в папке Задачи.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент был представлен в Microsoft Exchange 2007 SP1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для приложения к свойству папки во время операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |Определяет одну папку, создаемую в локальном клиентской магазине.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление одного свойства в папке в операции [UpdateFolder.](updatefolder-operation.md)  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном клиентской магазине.  <br/> |
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, используемых в операциях папок.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

