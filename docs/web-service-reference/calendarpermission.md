---
title: календарпермиссион
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
description: Элемент Календарпермиссион определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: c43f75e6cf5abc2dce9af6c04122ec9a589dcd58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529478"
---
# <a name="calendarpermission"></a>календарпермиссион

Элемент **календарпермиссион** определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
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

 **календарпермиссионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарпермиссионлевел](calendarpermissionlevel.md) <br/> |Представляет уровень разрешений, который пользователь имеет в папке "Календарь". Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[канкреатеитемс](cancreateitems.md) <br/> |Указывает, имеет ли пользователь разрешение на создание элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[канкреатесубфолдерс](cancreatesubfolders.md) <br/> |Указывает, имеет ли пользователь разрешение на создание вложенных папок в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[делетеитемс](deleteitems.md) <br/> |Указывает, имеет ли пользователь разрешение на удаление элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[едититемс](edititems.md) <br/> |Указывает, имеет ли пользователь разрешение на изменение элементов в папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдерконтакт](isfoldercontact.md) <br/> |Указывает, является ли пользователь контактом для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдеровнер](isfolderowner.md) <br/> |Указывает, является ли пользователь владельцем папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[исфолдервисибле](isfoldervisible.md) <br/> |Указывает, может ли пользователь просматривать папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[ReadItems (Календарпермиссионтипе)](readitems-calendarpermissiontype.md) <br/> |Указывает, имеет ли пользователь разрешение на чтение элементов в папке "Календарь". Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UserId](userid.md) <br/> |Определяет делегата или пользователя с разрешениями на доступ к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарпермиссионс](calendarpermissions.md) <br/> |Содержит массив разрешений календаря для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
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

