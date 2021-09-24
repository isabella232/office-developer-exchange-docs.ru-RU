---
title: DistinguishedFolderId (DistinguishedFolderIdNameType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: Элемент DistinguishedFolderId определяет папки, на которые можно ссылаться по имени.
ms.openlocfilehash: 23d1dead5a97fe8b2ceb29235f4b784f667d2ee1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59526442"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>DistinguishedFolderId (DistinguishedFolderIdNameType)

Элемент **DistinguishedFolderId** определяет папки, на которые можно ссылаться по имени. 
  
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
|[Folder](folder.md) <br/> |Указывает общую папку.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Указывает папку календаря.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Указывает папку контактов.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**Значения текста элемента DistinguishedFolderId**

|**Значение**|**Описание**|
|:-----|:-----|
|calendar  <br/> |Указывает URL-адрес папки календаря.  <br/> |
|contacts  <br/> |Указывает URL-адрес папки контактов.  <br/> |
|deleteditems  <br/> |Указывает URL-адрес папки удаленных элементов.  <br/> |
|drafts  <br/> |Указывает URL-адрес папки черновиков.  <br/> |
|inbox  <br/> |Указывает URL-адрес папки "Входящие".  <br/> |
|журнал  <br/> |Указывает URL-адрес папки журнала.  <br/> |
|notes  <br/> |Указывает URL-адрес папки примечаний.  <br/> |
|outbox  <br/> |Указывает URL-адрес папки "Избокс".  <br/> |
|sentitems  <br/> |Указывает URL-адрес папки отправленных элементов.  <br/> |
|tasks  <br/> |Указывает URL-адрес папки задач.  <br/> |
|msgfolderroot  <br/> |Указывает URL-адрес корневой папки сообщения.  <br/> |
|publicfoldersroot  <br/> |Указывает URL-адрес корневой папки общедоступных папок.  <br/> |
|root  <br/> |Указывает URL-адрес корневой папки.  <br/> |
|junkemail  <br/> |Указывает URL-адрес нежелательной папки электронной почты.  <br/> |
|searchfolders  <br/> |Указывает URL-адрес папки поиска.  <br/> |
|voicemail  <br/> |Указывает URL-адрес папки голосовой почты.  <br/> |
|recoverableitemsroot  <br/> |Указывает URL-адрес корневой папки восстанавливаемых элементов.  <br/> |
|recoverableitemsdeletions  <br/> |Указывает URL-адрес папки удаленных извлекаемых элементов.  <br/> |
|recoverableitemsversions  <br/> |Указывает URL-адрес папки версий извлекаемых элементов.  <br/> |
|recoverableitemspurges  <br/> |Указывает URL-адрес папки извлеченных извлекаемых элементов.  <br/> |
|archiveroot  <br/> |Указывает URL-адрес корневой папки архива.  <br/> |
|archivemsgfolderroot  <br/> |Указывает URL-адрес корневой папки архивной папки сообщений.  <br/> |
|archivedeleteditems  <br/> |Указывает URL-адрес архивной папки удаленных элементов.  <br/> |
|archiverecoverableitemsroot  <br/> |Указывает URL-адрес корневой папки архивируемых извлекаемых элементов.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Указывает URL-адрес архивной папки удаленных элементов, которые можно восстановить.  <br/> |
|archiverecoverableitemsversions  <br/> |Указывает URL-адрес папки версий архивируемых версий элементов.  <br/> |
|archiverecoverableitemspurges  <br/> |Указывает URL-адрес архивной папки извлекаемых извлекаемых элементов.  <br/> |
|syncissues  <br/> |Указывает URL-адрес папки проблем синхронизации.  <br/> |
|conflicts  <br/> |Указывает URL-адрес папки конфликтов.  <br/> |
|localfailures  <br/> |Указывает URL-адрес локальной папки отказов.  <br/> |
|serverfailures  <br/> |Указывает URL-адрес папки с ошибками сервера.  <br/> |
|recipientcache  <br/> |Указывает URL-адрес папки кэша получателя.  <br/> |
|quickcontacts  <br/> |Указывает URL-адрес папки быстрых контактов.  <br/> |
|conversationhistory  <br/> |Указывает URL-адрес папки истории беседы.  <br/> |
|adminauditlogs  <br/> |Указывает URL-адрес папки журнала административного аудита.  <br/> |
|todosearch  <br/> |Указывает URL-адрес папки поиска.  <br/> |
|mycontacts  <br/> |Указывает URL-адрес папки контактов.  <br/> |
|каталог  <br/> |Указывает URL-адрес папки каталога.  <br/> |
   
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

