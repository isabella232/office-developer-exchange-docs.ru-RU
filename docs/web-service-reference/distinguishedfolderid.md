---
title: DistinguishedFolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DistinguishedFolderId
api_type:
- schema
ms.assetid: 50018162-2941-4227-8a5b-d6b4686bb32f
description: Элемент DistinguishedFolderId определяет папки, которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент FolderId для идентификации в папку.
ms.openlocfilehash: 834166be3d882fa8c0533cfcc2999600430b82ce
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762192"
---
# <a name="distinguishedfolderid"></a>DistinguishedFolderId

Элемент **DistinguishedFolderId** определяет папки, которые можно ссылаться по имени. Если этот элемент не используется, необходимо использовать элемент [FolderId](folderid.md) для идентификации в папку. 
  
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
|
  **Id** <br/> |Содержит строку, которая определяет папки по умолчанию. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Содержит строку, которая определяет к папке, которая определена в атрибуте **Id** версии. Этот атрибут является необязательным. Этот атрибут используется, чтобы убедиться в том, что используется правильный версии папки.  <br/> |
   
#### <a name="id-attribute-values"></a>Значения атрибута ID

|**Значение**|**Описание**|
|:-----|:-----|
|календарь  <br/> |Представляет папку «Календарь».  <br/> |
|contacts  <br/> |Представляет папку «Контакты».  <br/> |
|deleteditems  <br/> |Представляет папки "Удаленные".  <br/> |
|черновики  <br/> |Представляет папке "Черновики".  <br/> |
|папки «Входящие»  <br/> |Представляет папку "Входящие".  <br/> |
|журнал  <br/> |Представляет папку журнала.  <br/> |
|notes  <br/> |Представляет папка «заметки».  <br/> |
|Исходящие  <br/> |Представляет папку "Исходящие".  <br/> |
|папки "Отправленные"  <br/> |Представляет папку «Отправленные».  <br/> |
|tasks  <br/> |Представляет папку задачи.  <br/> |
|msgfolderroot  <br/> |Представляет корневая папка сообщений.  <br/> |
|root  <br/> |Представляет корневой папки почтового ящика.  <br/> |
|junkemail  <br/> |Представляет папку нежелательной почты.  <br/> |
|searchfolders  <br/> |Представляет папку папки поиска.  <br/> |
|Голосовая почта  <br/> |Представляет папку голосовой почты.  <br/> |
|recoverableitemsroot  <br/> |Представляет корзины корневую папку.  <br/> |
|recoverableitemsdeletions  <br/> |Представляет корзины удалений папки.  <br/> |
|recoverableitemsversions  <br/> |Представляет корзины папка версий.  <br/> |
|recoverableitemspurges  <br/> |Представляет корзины удаляет папку.  <br/> |
|archiveroot  <br/> |Представляет корневую папку архива.  <br/> |
|archivemsgfolderroot  <br/> |Представляет корневую папку архива сообщения.  <br/> |
|archivedeleteditems  <br/> |Представляет папку архива удаленных элементов.  <br/> |
|archiveinbox  <br/> |Представляет архив папки "Входящие". Версии Exchange, начиная с номер сборки 15.00.0913.09 включать это значение.  <br/> |
|archiverecoverableitemsroot  <br/> |Представляет корневую папку архива элементов для восстановления.  <br/> |
|archiverecoverableitemsdeletions  <br/> |Представляет папку удалений элементов для восстановления архива.  <br/> |
|archiverecoverableitemsversions  <br/> |Представляет папку версий элементов для восстановления архива.  <br/> |
|archiverecoverableitemspurges  <br/> |Представляет папку удаляет элементов для восстановления архива.  <br/> |
|syncissues  <br/> |Представляет папку ошибок синхронизации.  <br/> |
|конфликтов  <br/> |Представляет папки "конфликты".  <br/> |
|localfailures  <br/> |Представляет папку Локальные ошибки.  <br/> |
|serverfailures  <br/> |Представляет папку ошибки сервера.  <br/> |
|recipientcache  <br/> |Представляет папку получателей кэша.  <br/> |
|QuickContacts  <br/> |Представляет папку быстрого контакты.  <br/> |
|conversationhistory  <br/> |Представляет папку журнал бесед.  <br/> |
|adminauditlogs  <br/> |Представляет папку журналы аудита администратора.  <br/> |
|todosearch  <br/> |Представляет папку поиска задач.  <br/> |
|mycontacts  <br/> |Представляет папку Мои контакты.  <br/> |
|каталог  <br/> |Представляет папку каталога.  <br/> |
|imcontactlist  <br/> |Представляет папку списка контактов обмена мгновенными Сообщениями.  <br/> |
|peopleconnect  <br/> |Представляет людей подключение папки.  <br/> |
|Избранное  <br/> |Представляет папку "Избранное".  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Mailbox](mailbox.md) <br/> |Определяет основной SMTP-адрес. Адреса прокси-серверов не допускается.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |Указывает папку, предназначенных для действия беседы, использующие папок.  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |Определяет папку назначения для копирования и перемещения действия беседы.  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | Указывает папку, в которой создается на новую папку или элемент.  <br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>  `/CreateItem/ParentFolderId` <br/><br/>`/CreateFolder/ParentFolderId` <br/> |
|[ParentFolderIds](parentfolderids.md) <br/> |Идентифицирует папок поиска [операции FindItem](finditem-operation.md) и [FindFolder операции](findfolder-operation.md).  <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |Представляет коллекцию папок, которые будут использоваться для определения содержимого папки поиска.  <br/> |
|[FolderIds](folderids.md) <br/> |Содержит массив идентификаторов папок, которые используются для определения папок для копирования, перемещение, получение, удаление или отслеживание уведомлений о событиях.  <br/> |
|[FolderChange](folderchange.md) <br/> |Представляет коллекцию изменений выполняется на одной папке.  <br/> <br/>Ниже приведен выражение XPath для этого элемента.<br/><br/>`/UpdateFolder/FolderChanges/FolderChange`<br/> |
|[ToFolderId](tofolderid.md) <br/> | Представляет конечной папки для копируемые или перемещения элемента или папки.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/MoveFolder/ToFolderId`<br/><br/>`/CopyFolder/ToFolderId`<br/><br/>`/MoveItem/ToFolderId`<br/><br/>`/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Определяет папку назначения для операций, обновление, отправка и создания элементов в хранилище Exchange.<br/><br/>Ниже приведены выражения XPath для этого элемента.<br/><br/>`/CreateItem/SavedItemFolderId`<br/><br/>`/UpdateItem/SavedItemFolderId`<br/><br/>`/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |Представляет папку, содержащую элементы для синхронизации.  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |Представляет имя объекта конфигурации пользователя. Имя объекта конфигурации пользователя — это идентификатор объекта конфигурации пользователя.  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |Представляет идентификатор папки, элементы копируются в сообщение электронной почты.  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |Представляет идентификатор папки элементы будут перемещены в сообщение электронной почты.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

**DistinguishedFolderId** разрешается **FolderId**. 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)
- [Создание папки (веб-служб Exchange)](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

