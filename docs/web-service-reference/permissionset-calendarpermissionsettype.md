---
title: PermissionSet (CalendarPermissionSetType)
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
ms.assetid: 75f20033-85eb-4627-b4f8-be85e4889e96
description: Элемент PermissionSet содержит все разрешения, настроенные для папки календаря.
ms.openlocfilehash: 26351be8fd9fbe56ea5abb2dd346cb9c9458c463
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59539157"
---
# <a name="permissionset-calendarpermissionsettype"></a>PermissionSet (CalendarPermissionSetType)

Элемент **PermissionSet** содержит все разрешения, настроенные для папки календаря. 
  
```XML
<PermissionSet>
   <CalendarPermissions/>
   <UnknownEntries/>
</PermissionSet>
```

 **CalendarPermissonSetType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarPermissions](calendarpermissions.md) <br/> |Содержит массив разрешений календаря для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
|[UnknownEntries](unknownentries.md) <br/> |Содержит массив неизвестных записей, которые невозможно разрешить в службе каталогов Active Directory. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, которая в основном содержит элементы календаря.  <br/> |
   
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

