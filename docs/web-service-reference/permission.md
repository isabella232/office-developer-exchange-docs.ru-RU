---
title: Permission
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permission
api_type:
- schema
ms.assetid: b8d0429a-0e58-4480-9847-4901970c7033
description: Элемент разрешений определяет доступ пользователя к папке.
ms.openlocfilehash: 600d60f481c4f1d407c3a39ab65d6ddcf46d04e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834735"
---
# <a name="permission"></a>Разрешение

Элемент **разрешений** определяет доступ пользователя к папке. 
  
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
|[CanCreateItems](cancreateitems.md) <br/> |Указывает, является ли пользователь имеет право на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[CanCreateSubFolders](cancreatesubfolders.md) <br/> |Указывает, является ли пользователь имеет право на создание вложенных папок в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[DeleteItems](deleteitems.md) <br/> |Указывает, является ли пользователь имеет разрешения на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[EditItems](edititems.md) <br/> |Указывает, является ли пользователь имеет разрешения на редактирование элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderContact](isfoldercontact.md) <br/> |Указывает, является ли пользователь является контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderOwner](isfolderowner.md) <br/> |Указывает, является ли пользователь является владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[IsFolderVisible](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[PermissionLevel](permissionlevel.md) <br/> |Представляет комбинации разрешений, которыми пользователь обладает на папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (PermissionType)](readitems-permissiontype.md) <br/> |Указывает, является ли пользователь имеет разрешение на чтение элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[Идентификатор пользователя](userid.md) <br/> |Идентифицирует пользователя делегатом или пользователь, имеющий права доступа к папкам. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешения](permissions.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
  
### <a name="version-differences"></a>Различия версий

Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365 или более в локальной версии Exchange, начиная с Exchange 2013 разрешения папок не возвращаются при [BaseShape](baseshape.md) элемент имеет значение **AllProperties** в запросе [GetFolder](getfolder-operation.md) операции. Для получения разрешений для папки, добавьте в элемент [AdditionalProperties](additionalproperties.md) в запросе **GetFolder** элемент [PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) . 
  
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

