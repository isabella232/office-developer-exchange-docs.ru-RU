---
title: тасксфолдер
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TasksFolder
api_type:
- schema
ms.assetid: 5a9a4612-8064-4986-b467-c44f268c64df
description: Элемент Тасксфолдер представляет папку Tasks, содержащуюся в почтовом ящике.
ms.openlocfilehash: 522fe485482bd8159927f9925b7a5582ba2e1c22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465340"
---
# <a name="tasksfolder"></a>тасксфолдер

Элемент **тасксфолдер** представляет папку Tasks, содержащуюся в почтовом ящике. 
  
```xml
<TasksFolder>
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
</TasksFolder>
```

**тасксфолдертипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |Содержит идентификатор и ключ изменения папки Tasks.  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |Представляет идентификатор родительской папки, содержащей папку Tasks.  <br/> |
|[фолдеркласс](folderclass.md) <br/> |Представляет класс Folder для папки Tasks.  <br/> |
|[DisplayName (строка)](displayname-string.md) <br/> |Содержит отображаемое имя папки задач.  <br/> |
|[тоталкаунт](totalcount.md) <br/> |Представляет общее количество элементов в папке "задачи".  <br/> |
|[чилдфолдеркаунт](childfoldercount.md) <br/> |Представляет количество дочерних папок, содержащихся в папке Tasks. Это свойство доступно только для чтения.  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |Определяет расширенные свойства для папки Tasks.  <br/> |
|[манажедфолдеринформатион](managedfolderinformation.md) <br/> |Содержит сведения об управляемой папке.  <br/> |
|[унреадкаунт](unreadcount.md) <br/> |Представляет количество непрочитанных элементов в папке "задачи".  <br/> |
|[PermissionSet (Пермиссионсеттипе)](permissionset-permissionsettype.md) <br/> |Содержит все настроенные разрешения для папки. Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).  <br/> |
|[еффективеригхтс](effectiverights.md) <br/> |Содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. Этот элемент появился в Microsoft Exchange 2007 с пакетом обновления 1 (SP1).  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[аппендтофолдерфиелд](appendtofolderfield.md) <br/> |Задает данные, добавляемые к свойству folder во время [операции операцию UpdateFolder](updatefolder-operation.md).  <br/> |
|[Create (Фолдерсинк)](create-foldersync.md) <br/> |Определяет одну папку для создания в локальном хранилище клиента.  <br/> |
|[сетфолдерфиелд](setfolderfield.md) <br/> |Представляет обновление одного свойства папки в [операции операцию UpdateFolder](updatefolder-operation.md).  <br/> |
|[Обновление (Фолдерсинк)](update-foldersync.md) <br/> |Определяет одну папку для обновления в локальном хранилище клиента.  <br/> |
|[Folders](folders-ex15websvcsotherref.md) <br/> |Содержит массив папок, используемых в операциях с папками.  <br/> |
   
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

