---
title: PermissionSet (PermissionSetType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- PermissionSet
api_type:
- schema
ms.assetid: 6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d
description: Элемент PermissionSet содержит все разрешения, настроенные для папки.
ms.openlocfilehash: b18fef33d3be6cb8c525f731a264860c3a83afdc
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543144"
---
# <a name="permissionset-permissionsettype"></a>PermissionSet (PermissionSetType)

Элемент **PermissionSet** содержит все разрешения, настроенные для папки. 
  
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
|[Разрешения](permissions.md) <br/> |Содержит коллекцию разрешений для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Содержит массив неизвестных записей, которые невозможно разрешить в службе каталогов Active Directory. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Определяет папку для создания, получения, поиска, синхронизации или обновления.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, которая содержится в почтовом ящике.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов, которая содержится в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач, которая содержится в почтовом ящике.  <br/> |
   
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

