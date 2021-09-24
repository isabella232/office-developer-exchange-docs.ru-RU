---
title: Разрешение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: Элемент Permission определяет доступ пользователя к папке.
ms.openlocfilehash: bc3e140aaf7bd9ea7f1a4993c9bea1dcad8d39fa
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512669"
---
# <a name="permission"></a>Разрешение

Элемент **Permission** определяет доступ пользователя к папке. 
  
```XML
<Permission>
   <CanCreateItems/>
   <CanCreateSubfolders/>
   <IsFolderOwner/>
   <IsFolderVisible/>
   <IsFolderContact/>
   <EditItems/>
   <DeleteItems/>
   <PermissionLevel/>
   <ReadItems/>
   <UserId/>
</Permission>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CanCreateItems](cancreateitems.md) <br/> |Указывает, имеет ли пользователь разрешение на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Указывает, имеет ли пользователь разрешение на создание подмостков в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Указывает, имеет ли пользователь разрешение на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[EditItems](edititems.md) <br/> |Указывает, имеет ли пользователь разрешение на редактирование элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Указывает, является ли пользователь контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Указывает, является ли пользователь владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |Представляет комбинацию разрешений, которые есть у пользователя в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |Указывает, имеет ли пользователь разрешение на чтение элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UserId](userid.md) <br/> |Определяет пользователя-делегата или пользователя, у которого есть разрешения на доступ к папкам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешения](permissions.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент был представлен в Exchange Server 2007 Пакет обновления 1 (SP1).
  
### <a name="version-differences"></a>Различия версий

Для приложений, Exchange Online, Exchange Online в составе Office 365 или локальной версии Exchange начиная с Exchange 2013 г., разрешения папок не возвращаются, если элемент [BaseShape](baseshape.md) имеет значение **AllProperties** в [GetFolder](getfolder-operation.md) запрос на операцию. Чтобы получить разрешения папок, добавьте элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) в элемент [AdditionalProperties](additionalproperties.md) в **запросе GetFolder.** 
  
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

