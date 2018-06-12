---
title: Разрешения
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: Элемент Permissions содержит набор разрешений на папку.
ms.openlocfilehash: 08d015c3b1afb58fce0fb4b99466965cc5c29fc6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834727"
---
# <a name="permissions"></a>Разрешения

Элемент **Permissions** содержит набор разрешений на папку. 
  
```XML
<Permissions>
   <Permission/>
</Permissions>
```

 **PermissionType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешение](permission.md) <br/> |Определяет доступ делегата в папку. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все разрешения, которые настроены для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
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
