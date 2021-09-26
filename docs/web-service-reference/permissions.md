---
title: Разрешения
manager: sethgros
ms.date: 09/17/2015
ms.audience: ITPro
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Permissions
api_type:
- schema
ms.assetid: 2ba50bd9-819f-4e5f-a3bb-85a0a87d8a86
description: Элемент Permissions содержит коллекцию разрешений для папки.
ms.openlocfilehash: 079bd74def1d768b3c8406d8949dcaa3ac0a0baf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544831"
---
# <a name="permissions"></a>Permissions

Элемент **Permissions** содержит коллекцию разрешений для папки. 
  
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
|[Разрешение](permission.md) <br/> |Определяет доступ делегата к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |Содержит все разрешения, настроенные для папки. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
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

