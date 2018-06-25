---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: Элемент PermissionSet содержит все разрешения, которые настроены для папки.
ms.openlocfilehash: 0fa0ac78a0db2bf382ad413cbb8bd072aa88c6fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834732"
---
# <a name="permissionset-permissionsettype"></a>PermissionSet (PermissionSetType)

Элемент **PermissionSet** содержит все разрешения, которые настроены для папки. 
  
```XML
<PermissionSet>
   <Permissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **PermissionSetType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешения](permissions.md) <br/> |Содержит набор разрешений на папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Содержит массив Неизвестный записей, которые не удалось разрешить от службы каталогов Active Directory. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Определяет папку для создания, получение, найти, синхронизировать или обновить.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащихся в почтовом ящике.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку Контакты, содержащихся в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задачи, содержащихся в почтовом ящике.  <br/> |
   
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

