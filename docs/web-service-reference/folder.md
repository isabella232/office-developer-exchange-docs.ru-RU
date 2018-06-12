---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Элемент Folder определяет папку для создания, получение, найти, синхронизировать или обновить.
ms.openlocfilehash: ecfea52d2105599372a22b78778ac0d0d066bc60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762622"
---
# <a name="folder"></a>Folder

Элемент **Folder** определяет папку для создания, получение, найти, синхронизировать или обновить. 
  
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
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей папку.  <br/> |
|[FolderClass](folderclass.md) <br/> |Представляет класс папки для данной папки.  <br/> |
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Содержит отображаемое имя папки.  <br/> |
|[TotalCount](totalcount.md) <br/> |Представляет общее число элементов в указанной папке.  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Представляет число дочерних папок, содержащихся в папке. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства папки.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемых папок.  <br/> |
|[UnreadCount](unreadcount.md) <br/> |Представляет количество непрочитанных элементов в указанной папке.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[Создание (FolderSync)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[Обновление (FolderSync)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Папки](folders-ex15websvcsotherref.md) <br/> |Содержит набор папок, используемых в операциях папки.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает с установленной ролью сервера клиентского доступа Exchange 2007.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

