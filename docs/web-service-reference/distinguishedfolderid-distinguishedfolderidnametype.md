---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: Элемент DistinguishedFolderId определяет папки, которые можно ссылаться по имени.
ms.openlocfilehash: 1f5b97fc7ee7b93989762c26e4b979a8dfb884be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762190"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

Элемент **DistinguishedFolderId** определяет папки, которые можно ссылаться по имени. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **DistinguishedFolderIdNameType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Указывает универсальный папки.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Путь к папке календаря.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Указывает папку Контакты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**DistinguishedFolderId элемент текстовые значения**

|**Значение**|**Описание**|
|:-----|:-----|
|календарь  <br/> |Указывает URL-адрес папки календаря.  <br/> |
|contacts  <br/> |Указывает URL-адрес папки «Контакты».  <br/> |
|deleteditems  <br/> |Указывает URL-адрес папки "Удаленные".  <br/> |
|черновики  <br/> |Указывает URL-адрес папке "Черновики".  <br/> |
|папки «Входящие»  <br/> |Указывает URL-адрес папки "Входящие".  <br/> |
|журнал  <br/> |Указывает URL-адрес папки журнала.  <br/> |
|notes  <br/> |Указывает URL-адрес папка «заметки».  <br/> |
|Исходящие  <br/> |Указывает URL-адрес папки "Исходящие".  <br/> |
|папки "Отправленные"  <br/> |Указывает URL-адрес папки «Отправленные».  <br/> |
|tasks  <br/> |Указывает URL-адрес папки задач.  <br/> |
|msgfolderroot  <br/> |Указывает URL-адрес в корневой папке сообщения.  <br/> |
|publicfoldersroot  <br/> |Указывает URL-адрес в корневой папке общих папок.  <br/> |
|root  <br/> |Указывает URL-адрес в корневой папке.  <br/> |
|junkemail  <br/> |Указывает URL-адрес в папку нежелательной почты.  <br/> |
|searchfolders  <br/> |Указывает URL-адрес папки поиска.  <br/> |
|Голосовая почта  <br/> |Указывает URL-адрес папки голосовой почты.  <br/> |
|recoverableitemsroot  <br/> |Указывает URL-адрес корневой папки элементов для восстановления.  <br/> |
|recoverableitemsdeletions  <br/> |Указывает URL-адрес папки папки "Удаленные".  <br/> |
|recoverableitemsversions  <br/> |Указывает URL-адрес папки версий восстанавливаемый элемент.  <br/> |
|recoverableitemspurges  <br/> |Указывает URL-адрес в папку удаленных элементов для восстановления.  <br/> |
|archiveroot  <br/> |Указывает URL-адрес в корневую папку архива.  <br/> |
|archivemsgfolderroot  <br/> |Указывает URL-адрес в корневой папке папки заархивированные сообщения.  <br/> |
|archivedeleteditems  <br/> |Указывает URL-адрес папки архива "Удаленные".  <br/> |
|archiverecoverableitemsroot  <br/> |Указывает URL-адрес в корневой папке архивных элементов для восстановления.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Указывает URL-адрес папки архива папки "Удаленные".  <br/> |
|archiverecoverableitemsversions  <br/> |Указывает URL-адрес папки версии архивных элементов для восстановления.  <br/> |
|archiverecoverableitemspurges  <br/> |Указывает URL-адрес папки архивных удаленных элементов для восстановления.  <br/> |
|syncissues  <br/> |Указывает URL-адрес папки проблемы синхронизации.  <br/> |
|конфликтов  <br/> |Указывает URL-адрес папки "конфликты".  <br/> |
|localfailures  <br/> |Указывает URL-адрес папки Локальные ошибки.  <br/> |
|serverfailures  <br/> |Указывает URL-адрес папки сбоев сервера.  <br/> |
|recipientcache  <br/> |Указывает URL-адрес папки кэш-памяти получателя.  <br/> |
|QuickContacts  <br/> |Указывает URL-адрес папки, экспресс-контакты.  <br/> |
|conversationhistory  <br/> |Указывает URL-адрес папки журнал бесед.  <br/> |
|adminauditlogs  <br/> |Указывает URL-адрес папки журнала административного аудита.  <br/> |
|todosearch  <br/> |Указывает URL-адрес папки поиска задачи.  <br/> |
|mycontacts  <br/> |Указывает URL-адрес Мои папки «Контакты».  <br/> |
|каталог  <br/> |Указывает URL-адрес папки каталога.  <br/> |
   
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

