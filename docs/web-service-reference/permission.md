---
title: Разрешение
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
description: Элемент permission определяет доступ пользователя к папке.
ms.openlocfilehash: 0f7515dbb06f8423f8d4d95e1391496e8ac73653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459260"
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

 **пермиссионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[канкреатеитемс](cancreateitems.md) <br/> |Указывает, имеет ли пользователь разрешение на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[канкреатесубфолдерс](cancreatesubfolders.md) <br/> |Указывает, имеет ли пользователь разрешение на создание вложенных папок в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[делетеитемс](deleteitems.md) <br/> |Указывает, имеет ли пользователь разрешение на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[едититемс](edititems.md) <br/> |Указывает, имеет ли пользователь разрешение на изменение элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдерконтакт](isfoldercontact.md) <br/> |Указывает, является ли пользователь контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдеровнер](isfolderowner.md) <br/> |Указывает, является ли пользователь владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдервисибле](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[пермиссионлевел](permissionlevel.md) <br/> |Представляет сочетание разрешений, которые пользователь имеет в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (Пермиссионтипе)](readitems-permissiontype.md) <br/> |Указывает, имеет ли пользователь разрешение на чтение элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UserId](userid.md) <br/> |Определяет делегата или пользователя с разрешениями на доступ к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешения](permissions.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
  
### <a name="version-differences"></a>Различия версий

Для приложений, предназначенных для Exchange Online, Exchange Online в составе Office 365, или локальной версии Exchange, начиная с Exchange 2013, разрешения для папки не возвращаются, если элемент [басешапе](baseshape.md) имеет значение **аллпропертиес** в запросе операции- [папки](getfolder-operation.md) . Чтобы получить разрешения для папки, добавьте элемент [PermissionSet (пермиссионсеттипе)](permissionset-permissionsettype.md) в элемент [аддитионалпропертиес](additionalproperties.md) в запросе на получение **папки** . 
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

