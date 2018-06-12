---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: Элемент CalendarPermission определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7f6ceb6895add3fdd82cdd595463b3a80db822e5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761649"
---
# <a name="calendarpermission"></a>CalendarPermission

Элемент **CalendarPermission** определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<Permission>
   <CalendarPermissionLevel/>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **CalendarPermissionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |Представляет уровень разрешений, который пользователь имеет папки календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |Указывает, является ли пользователь имеет право на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Указывает, является ли пользователь имеет право на создание вложенных папок в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Указывает, является ли пользователь имеет разрешения на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[EditItems](edititems.md) <br/> |Указывает, является ли пользователь имеет разрешения на редактирование элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Указывает, является ли пользователь является контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Указывает, является ли пользователь является владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |Указывает, является ли пользователь имеет разрешение на чтение элементов внутри папки календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[Идентификатор пользователя](userid.md) <br/> |Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Содержит набор разрешений на папку календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

