---
title: арчиветаг
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c4cb0718-37cd-41aa-86e7-b492c4bb86aa
description: Элемент Арчиветаг указывает идентификатор хранения набора тегов архива для элемента или папки.
ms.openlocfilehash: 23167f3c96a6756fe4c6d915a4de91e815e620d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464765"
---
# <a name="archivetag"></a>арчиветаг

Элемент **арчиветаг** указывает идентификатор хранения набора тегов архива для элемента или папки. 
  
```XML
<ArchiveTag IsExplicit=""></ArchiveTag>
```

 **ретентионтагтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Явный** <br/> |Указывает, будет ли политика хранения явно задана для элемента или папки, а также от того, унаследована ли она от родительской папки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку, в которой в основном содержатся элементы календаря.  <br/> |
|[календаритем](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[контакт](contact.md); <br/> |Представляет элемент контакта в хранилище Exchange.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку "Контакты", содержащуюся в почтовом ящике.  <br/> |
|[дистрибутионлист](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Folder](folder.md) <br/> |Определяет папку для создания, получения, поиска, синхронизации или обновления.  <br/> |
|[Ресурс](item.md) <br/> |Представляет общий элемент в хранилище Exchange.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Microsoft Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент POST в хранилище Exchange.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащуюся в почтовом ящике.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку Tasks, содержащуюся в почтовом ящике.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **арчиветаг** — идентификатор GUID, определяющий политику хранения. 
  
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

