---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: Элемент ContactsFolder представляет папку Контакты, содержащихся в почтовом ящике.
ms.openlocfilehash: 01302f00d84cfff9713e3b188b7799c537fc0629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761739"
---
# <a name="contactsfolder"></a>ContactsFolder

Элемент **ContactsFolder** представляет папку Контакты, содержащихся в почтовом ящике. 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 **ContactsFolderType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки Контакты.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей папки «Контакты».  <br/> |
|[FolderClass](folderclass.md) <br/> |Представляет класс папки для папки контактов.  <br/> |
|[Отображаемое имя (строка)](displayname-string.md) <br/> |Содержит отображаемое имя папки Контакты.  <br/> |
|[TotalCount](totalcount.md) <br/> |Представляет общее число элементов в папке «Контакты».  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |Представляет число дочерних папок, содержащихся в папке «Контакты». Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства списка контактов пользователя.  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |Содержит сведения об управляемых папок.  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |Содержит права клиента на основании параметров разрешений для элемента или папки.  <br/> |
|[SharingEffectiveRights (PermissionReadAccessType)](sharingeffectiverights-permissionreadaccesstype.md) <br/> |Указывает разрешения, которые пользователь имеет для контактных данных, общий.  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |Указывает данные для добавления к папке свойство во время [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[Создание (FolderSync)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |Представляет обновление для одного свойства папки в рамках одной [операции UpdateFolder](updatefolder-operation.md).  <br/> |
|[Обновление (FolderSync)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Папки](folders-ex15websvcsotherref.md) <br/> |Содержит набор папок, используемых в операциях папки.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

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

