---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: Элемент ArchiveTag указывает идентификатор хранения тега архива, заданного на элементе или папке.
ms.openlocfilehash: c3545b505dc0596d7465154e0be7d6c758b24ec9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59525241"
---
# <a name="archivetag"></a>ArchiveTag

Элемент **ArchiveTag** указывает идентификатор хранения тега архива, заданного на элементе или папке. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IsExplicit** <br/> |Указывает, установлена ли политика хранения явно на элементе или папке или наследуется ли она из родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, которая в основном содержит элементы календаря.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Contact](contact.md) <br/> |Представляет элемент контакта в Exchange магазине.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов, которая содержится в почтовом ящике.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Определяет папку для создания, получения, поиска, синхронизации или обновления.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент в Exchange магазине.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange Майкрософт.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, которая содержится в почтовом ящике.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач, которая содержится в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **ArchiveTag** — это GUID, определяющие политику хранения. 
  
## <a name="remarks"></a>Заметки

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

