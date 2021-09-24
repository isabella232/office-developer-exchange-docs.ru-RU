---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: Элемент DistinguishedFolderId определяет папки, на которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент FolderId для идентификации папки.
ms.openlocfilehash: 309db925bb783c435320aeb283915ece39da2271
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521999"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

Элемент **DistinguishedFolderId** определяет папки, на которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент [FolderId](folderid.md) для идентификации папки. 
  
```XML
<DistinguishedFolderId Id="" ChangeKey="">
   <Mailbox/>
</DistinguishedFolderId>
```

 **DistinguishedFolderIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**Id** <br/> |Содержит строку, которая идентифицирует папку по умолчанию. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Содержит строку, определяемую версией папки, идентифицируемой **атрибутом Id.** Этот атрибут является необязательным. Используйте этот атрибут, чтобы убедиться, что используется правильная версия папки.  <br/> |
   
#### <a name="id-attribute-values"></a>Значения атрибута Id

|**Значение**|**Описание**|
|:-----|:-----|
|calendar  <br/> |Представляет папку Calendar.  <br/> |
|contacts  <br/> |Представляет папку Контакты.  <br/> |
|deleteditems  <br/> |Представляет папку "Удаленные элементы".  <br/> |
|drafts  <br/> |Представляет папку Черновики.  <br/> |
|inbox  <br/> |Представляет папку Входящие.  <br/> |
|журнал  <br/> |Представляет папку Журнал.  <br/> |
|notes  <br/> |Представляет папку Заметки.  <br/> |
|outbox  <br/> |Представляет папку "Избокс".  <br/> |
|sentitems  <br/> |Представляет папку Отправленные элементы.  <br/> |
|tasks  <br/> |Представляет папку Задачи.  <br/> |
|msgfolderroot  <br/> |Представляет корень папки сообщений.  <br/> |
|root  <br/> |Представляет корень почтового ящика.  <br/> |
|junkemail  <br/> |Представляет папку нежелательной почты.  <br/> |
|searchfolders  <br/> |Представляет папку папки поиска.  <br/> |
|voicemail  <br/> |Представляет папку голосовой почты.  <br/> |
|recoverableitemsroot  <br/> |Представляет корневую папку контейнера.  <br/> |
|recoverableitemsdeletions  <br/> |Представляет папку удаления контейнера.  <br/> |
|recoverableitemsversions  <br/> |Представляет папку версий контейнера.  <br/> |
|recoverableitemspurges  <br/> |Представляет папку очистки контейнера.  <br/> |
|archiveroot  <br/> |Представляет папку корневого архива.  <br/> |
|archivemsgfolderroot  <br/> |Представляет папку сообщений корневого архива.  <br/> |
|archivedeleteditems  <br/> |Представляет папку удаленных элементов архива.  <br/> |
|archiveinbox  <br/> |Представляет папку архивных почтовых ящиков. Версии Exchange со сборкой 15.00.0913.09 включают это значение.  <br/> |
|archiverecoverableitemsroot  <br/> |Представляет корневую папку восстанавливаемых элементов архива.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Представляет папку удаления извлекаемых из архива элементов.  <br/> |
|archiverecoverableitemsversions  <br/> |Представляет папку версий архивных версий элементов.  <br/> |
|archiverecoverableitemspurges  <br/> |Представляет папку очистки извлекаемых из архива элементов.  <br/> |
|syncissues  <br/> |Представляет папку проблем синхронизации.  <br/> |
|conflicts  <br/> |Представляет папку конфликтов.  <br/> |
|localfailures  <br/> |Представляет локализованную папку отказов.  <br/> |
|serverfailures  <br/> |Представляет папку с ошибками сервера.  <br/> |
|recipientcache  <br/> |Представляет папку кэша получателя.  <br/> |
|quickcontacts  <br/> |Представляет папку быстрых контактов.  <br/> |
|conversationhistory  <br/> |Представляет папку истории беседы.  <br/> |
|adminauditlogs  <br/> |Представляет папку журналов аудита администратора.  <br/> |
|todosearch  <br/> |Представляет папку поиска todo.  <br/> |
|mycontacts  <br/> |Представляет папку Мои контакты.  <br/> |
|каталог  <br/> |Представляет папку каталога.  <br/> |
|imcontactlist  <br/> |Представляет папку списка контактов в чате.  <br/> |
|peopleconnect  <br/> |Представляет папку подключения людей.  <br/> |
|избранное  <br/> |Представляет папку Избранное.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет основной smTP-адрес. Прокси-адреса не допускаются.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, которая ориентирована на действия разговоров, которые используют папки.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Указывает папку назначения для копирования и перемещения действий беседы.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Определяет папку, в которой создается новая папка или элемент.  <br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Определяет папки для поиска операции [FindItem](finditem-operation.md) и [операции FindFolder.](findfolder-operation.md)  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Представляет коллекцию папок, которые будут искать для определения содержимого папки поиска.  <br/> |
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, используемых для идентификации папок для копирования, перемещения, получения, удаления или мониторинга уведомлений о событиях.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений, выполняемых в одной папке.  <br/> <br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Представляет папку назначения для скопированного или перемещенного элемента или папки.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Определяет целевую папку для операций, которые обновляют, отправляют и создают элементы в Exchange магазине.<br/><br/>Ниже приводится выражение XPath к этому элементу:<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, которая содержит элементы для синхронизации.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Представляет ID папки, в которую будут скопированы элементы электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Представляет ID папки, в которую будут перемещены элементы электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

**DistinguishedFolderId** решается на **папку**. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание папок (Exchange веб-служб)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

