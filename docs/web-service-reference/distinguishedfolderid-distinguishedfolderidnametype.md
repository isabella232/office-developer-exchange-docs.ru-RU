---
title: Дистингуишедфолдерид (Дистингуишедфолдериднаметипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 915b2ee9-8284-4bf6-8995-1fd0785e9e48
description: Элемент Дистингуишедфолдерид определяет папки, на которые можно ссылаться по имени.
ms.openlocfilehash: 1f5b97fc7ee7b93989762c26e4b979a8dfb884be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762190"
---
# <a name="distinguishedfolderid-distinguishedfolderidnametype"></a>Дистингуишедфолдерид (Дистингуишедфолдериднаметипе)

Элемент **дистингуишедфолдерид** определяет папки, на которые можно ссылаться по имени. 
  
```XML
<DistinguishedFolderId> calendar | contacts | deleteditems | drafts | inbox | journal | notes | outbox | sentitems | tasks | msgfolderroot | publicfoldersroot | root | junkemail | searchfolders | voicemail | recoverableitemsroot | recoverableitemsdeletions | recoverableitemsversions | recoverableitemspurges | archiveroot | archivemsgfolderroot | archivedeleteditems | archiverecoverableitemsroot | archiverecoverableitemsdeletions | archiverecoverableitemsversions | archiverecoverableitemspurges | syncissues | conflicts | localfailures | serverfailures | recipientcache | quickcontacts | conversationhistory | adminauditlogs | todosearch | mycontacts | directory | imcontactlist | peopleconnect</DistinguishedFolderId>
```

 **дистингуишедфолдериднаметипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

Нет
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Указывает общую папку.  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Указывает папку "Календарь".  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Указывает папку "Контакты".  <br/> |
   
## <a name="text-value"></a>Текстовое значение

**Текстовые значения элементов Дистингуишедфолдерид**

|**Значение**|**Описание**|
|:-----|:-----|
|calendar  <br/> |Указывает URL-адрес папки "Календарь".  <br/> |
|contacts  <br/> |Указывает URL-адрес папки контактов.  <br/> |
|deleteditems  <br/> |Указывает URL-адрес папки удаленных элементов.  <br/> |
|drafts  <br/> |Указывает URL-адрес папки "Черновики".  <br/> |
|inbox  <br/> |Указывает URL-адрес папки "Входящие".  <br/> |
|Фин  <br/> |Указывает URL-адрес папки журнала.  <br/> |
|notes  <br/> |Указывает URL-адрес папки заметок.  <br/> |
|outbox  <br/> |Указывает URL-адрес папки "Исходящие".  <br/> |
|sentitems  <br/> |Указывает URL-адрес папки "Отправленные".  <br/> |
|tasks  <br/> |Указывает URL-адрес папки Tasks.  <br/> |
|msgfolderroot  <br/> |Указывает URL-адрес корневой папки сообщения.  <br/> |
|публикфолдерсрут  <br/> |Указывает URL-адрес корневой папки общедоступных папок.  <br/> |
|root  <br/> |Указывает URL-адрес корневой папки.  <br/> |
|junkemail  <br/> |Указывает URL-адрес папки нежелательной почты.  <br/> |
|searchfolders  <br/> |Указывает URL-адрес папок поиска.  <br/> |
|voicemail  <br/> |Указывает URL-адрес папки голосовой почты.  <br/> |
|рековераблеитемсрут  <br/> |Указывает URL-адрес корневой папки "элементы с возможностью восстановления".  <br/> |
|recoverableitemsdeletions  <br/> |Указывает URL-адрес удаленной папки "элементы с возможностью восстановления".  <br/> |
|рековераблеитемсверсионс  <br/> |Указывает URL-адрес папки "версии элемента с возможностью восстановления".  <br/> |
|рековераблеитемспуржес  <br/> |Указывает URL-адрес очищенной папки "элементы с возможностью восстановления".  <br/> |
|арчиверут  <br/> |Указывает URL-адрес корневой папки архива.  <br/> |
|арчивемсгфолдеррут  <br/> |Указывает URL-адрес корневой папки с архивным сообщением.  <br/> |
|арчиведелетедитемс  <br/> |Указывает URL-адрес папки архивированных удаленных элементов.  <br/> |
|арчиверековераблеитемсрут  <br/> |Указывает URL-адрес корневой папки "архивные элементы с возможностью восстановления".  <br/> |
|арчиверековераблеитемсделетионс  <br/> |Указывает URL-адрес папки "архивные элементы с возможностью восстановления".  <br/> |
|арчиверековераблеитемсверсионс  <br/> |Указывает URL-адрес папки с архивными версиями элементов для восстановления.  <br/> |
|арчиверековераблеитемспуржес  <br/> |Указывает URL-адрес папки "архивная Очистка" элементов с возможностью восстановления.  <br/> |
|syncissues  <br/> |Указывает URL-адрес папки "ошибки синхронизации".  <br/> |
|conflicts  <br/> |Указывает URL-адрес папки конфликтов.  <br/> |
|localfailures  <br/> |Указывает URL-адрес папки "Локальные ошибки".  <br/> |
|serverfailures  <br/> |Указывает URL-адрес папки "ошибки сервера".  <br/> |
|реЦипиенткаче  <br/> |Указывает URL-адрес папки кэша получателей.  <br/> |
|куиккконтактс  <br/> |Указывает URL-адрес папки "Быстрые контакты".  <br/> |
|conversationhistory  <br/> |Указывает URL-адрес папки "Журнал бесед".  <br/> |
|админаудитлогс  <br/> |Указывает URL-адрес папки журнала административного аудита.  <br/> |
|тодосеарч  <br/> |Указывает URL-адрес папки поиска.  <br/> |
|Mycontacts  <br/> |Указывает URL-адрес папки "Мои контакты".  <br/> |
|каталога  <br/> |Указывает URL-адрес папки каталога.  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент появился в Exchange Server 2013.
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема типа  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> ||
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

