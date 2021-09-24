---
title: CalendarPermission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarPermission
api_type:
- schema
ms.assetid: 3aafb221-a04b-41f6-804e-eda810f1ba28
description: Элемент CalendarPermission определяет доступ пользователя к папке Calendar. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7794cab261653f8cb6421d4e0633d496ba347a5f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514804"
---
# <a name="calendarpermission"></a>CalendarPermission

Элемент **CalendarPermission** определяет доступ пользователя к папке Calendar. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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
|[CalendarPermissionLevel](calendarpermissionlevel.md) <br/> |Представляет уровень разрешений, который имеет пользователь в папке Calendar. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateItems](cancreateitems.md) <br/> |Указывает, имеет ли пользователь разрешение на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Указывает, имеет ли пользователь разрешение на создание подмостков в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Указывает, имеет ли пользователь разрешение на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[EditItems](edititems.md) <br/> |Указывает, имеет ли пользователь разрешение на редактирование элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Указывает, является ли пользователь контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Указывает, является ли пользователь владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (CalendarPermissionType)](readitems-calendarpermissiontype.md) <br/> |Указывает, имеет ли пользователь разрешение на чтение элементов в папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UserId](userid.md) <br/> |Определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Содержит массив разрешений календаря для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

