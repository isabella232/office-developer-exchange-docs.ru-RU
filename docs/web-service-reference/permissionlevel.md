---
title: PermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermissionLevel
api_type:
- schema
ms.assetid: 87978600-3523-451e-a725-ef092c543e2a
description: Элемент PermissionLevel представляет уровень разрешений, который пользователь имеет на папку. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: 7cc734f5807fe039467065315c220341f47d3fb4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834730"
---
# <a name="permissionlevel"></a>PermissionLevel

Элемент **PermissionLevel** представляет уровень разрешений, который пользователь имеет на папку. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<PermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or Custom</PermissionLevel>
```

 **PermissionLevelType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Разрешение](permission.md) <br/> |Определяет доступ пользователя к папке. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице приведены возможные значения для элемента **PermissionLevel** . 
  
**PermissionLevel элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что пользователь не имеет разрешений на папку.  <br/> |
|Owner  <br/> |Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки. Пользователь является владельцем папки и папки контактов.  <br/> |
|PublishingEditor  <br/> |Указывает, что пользователя можно создавать, читать, изменить и удаление всех элементов в папке и создавать вложенные папки.  <br/> |
|Редактор  <br/> |Указывает, что пользователь создание, чтение, изменение и удаление всех элементов в папке.  <br/> |
|PublishingAuthor  <br/> |Указывает, что пользователя можно создавать и читать все элементы в папке, изменять и удалять только элементы, которые пользователь создает и создавать вложенные папки.  <br/> |
|Author  <br/> |Указывает, что пользователь создавать и читать все элементы в папке и редактировать и удалять только элементы, которые пользователь создает.  <br/> |
|NoneditingAuthor  <br/> |Указывает, что пользователь создавать и читать все элементы в папке и удалить только элементы, которые пользователь создает.  <br/> |
|Редактор  <br/> |Указывает, что пользователи могут читать все элементы в папке.  <br/> |
|Участник  <br/> |Указывает, что пользователь может создавать элементы в папке. Содержимое папки не отображаются.  <br/> |
|Пользовательский сервер  <br/> |Указывает, что пользователь имеет пользовательские разрешения доступа в общей папке.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
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
