---
title: Folder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Элемент Folder определяет папку для создания, получения, поиска, синхронизации или обновления.
ms.openlocfilehash: 156813b3f7ecc6a2e1437f473ae1daa76b138e6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457251"
---
# <a name="folder"></a>Folder

Элемент **Folder** определяет папку для создания, получения, поиска, синхронизации или обновления. 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 **фолдертипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей папку.  <br/> |
|[фолдеркласс](folderclass.md) <br/> |Представляет класс папки для данной папки.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Содержит отображаемое имя папки.  <br/> |
|[тоталкаунт](totalcount.md) <br/> |Представляет общее количество элементов в заданной папке.  <br/> |
|[чилдфолдеркаунт](childfoldercount.md) <br/> |Представляет количество дочерних папок, содержащихся в папке. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папок.  <br/> |
|[манажедфолдеринформатион](managedfolderinformation.md) <br/> |Содержит сведения об управляемой папке.  <br/> |
|[унреадкаунт](unreadcount.md) <br/> |Представляет количество непрочитанных элементов в заданной папке.  <br/> |
|[PermissionSet (Пермиссионсеттипе)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Exchange 2007 с пакетом обновления 1.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аппендтофолдерфиелд](appendtofolderfield.md) <br/> |Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).  <br/> |
|[Create (Фолдерсинк)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[сетфолдерфиелд](setfolderfield.md) <br/> |Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).  <br/> |
|[Обновление (Фолдерсинк)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, используемых в операциях с папками.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Exchange 2007, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

