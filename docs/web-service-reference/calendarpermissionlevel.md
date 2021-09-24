---
title: CalendarPermissionLevel
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarPermissionLevel
api_type:
- schema
ms.assetid: 6ac2b792-4326-4a3f-b6cb-977bf523b5b2
description: Элемент CalendarPermissionLevel представляет уровень разрешений, который имеет пользователь в папке Calendar. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).
ms.openlocfilehash: e43b26f12fa65f47ca8377ecdd6c3abe2f6c5b71
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518836"
---
# <a name="calendarpermissionlevel"></a>CalendarPermissionLevel

Элемент **CalendarPermissionLevel** представляет уровень разрешений, который имеет пользователь в папке Calendar. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1). 
  
```xml
<CalendarPermissionLevel>None or Owner or PublishingEditor or Editor or PublishingAuthor or Author or NoneditingAuthor or Reviewer or Contributor or FreeBusyTimeOnly or FreeBusyTimeAndSubjectAndLocation or Custom</CalendarPermissionLevel>
```

 **CalendarPermissionLevelType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarPermission](calendarpermission.md) <br/> |Определяет доступ пользователя к папке календаря. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

В следующей таблице перечислены возможные значения элемента **CalendarPermissionLevel.** 
  
**Текстовые значения элемента CalendarPermissionLevel**

|**Значение**|**Описание**|
|:-----|:-----|
|Нет  <br/> |Указывает, что у пользователя нет разрешений на папку.  <br/> |
|Владелец  <br/> |Указывает, что пользователь может создавать, читать, изменять и удалять все элементы в папке и создавать подмостки. Пользователь является как владельцем папок, так и контактом папки.  <br/> |
|PublishingEditor  <br/> |Указывает, что пользователь может создавать, читать, изменять и удалять все элементы в папке и создавать подмостки.  <br/> |
|Редактор  <br/> |Указывает, что пользователь может создавать, читать, редактировать и удалять все элементы в папке.  <br/> |
|PublishingAuthor  <br/> |Указывает, что пользователь может создавать и читать все элементы в папке, редактировать и удалять только элементы, которые создает пользователь, и создавать подмостки.  <br/> |
|Автор  <br/> |Указывает, что пользователь может создавать и читать все элементы в папке, а также изменять и удалять только элементы, которые создает пользователь.  <br/> |
|NoneditingAuthor  <br/> |Указывает, что пользователь может создавать и читать все элементы в папке и удалять только элементы, которые создает пользователь.  <br/> |
|Reviewer  <br/> |Указывает, что пользователь может читать все элементы в папке.  <br/> |
|Участник  <br/> |Указывает, что пользователь может создавать элементы в папке. Содержимое папки не отображаются.  <br/> |
|FreeBusyTimeOnly  <br/> |Указывает, что пользователь может просматривать только свободное или занятое время в календаре.  <br/> |
|FreeBusyTimeAndSubjectAndLocation  <br/> |Указывает, что пользователь может просматривать свободное или занятое время в календаре, а также тему и расположение встреч.  <br/> |
|Пользовательский сервер  <br/> |Указывает, что пользователь имеет пользовательские разрешения доступа в папке.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
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

