---
title: ArchiveTag
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: Элемент ArchiveTag указывает идентификатор хранения архива тега для элемента или папки.
ms.openlocfilehash: ae9c7d512981af3bf564bcb73a9a27c5c78217fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761493"
---
# <a name="archivetag"></a>ArchiveTag

Элемент **ArchiveTag** указывает идентификатор хранения архива тега для элемента или папки. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **RetentionTagType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**IsExplicit** <br/> |Указывает ли политика хранения явно задать для элемента или папки или ли наследуется от родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, содержащую элементы календаря в первую очередь.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет контакт в хранилище Exchange.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку Контакты, содержащихся в почтовом ящике.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Определяет папку для создания, получение, найти, синхронизировать или обновить.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент post в хранилище Exchange.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащихся в почтовом ящике.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задачи, содержащихся в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **ArchiveTag** — это идентификатор GUID, определяющий политику хранения. 
  
## <a name="remarks"></a>Замечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

