---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: Элемент ManagedFolderInformation содержит сведения о настраиваемой управляемой папки.
ms.openlocfilehash: ef46e2e0db440de2a8acae8316ce98d11bd6710e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834341"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

Элемент **ManagedFolderInformation** содержит сведения о настраиваемой управляемой папки. 
  
```xml
<ManagedFolderInformation>
   <CanDelete/>
   <CanRenameOrMove/>
   <MustDisplayComment/>
   <HasQuota/>
   <IsManagedFoldersRoot/>
   <ManagedFolderId/>
   <Comment/>
   <StorageQuota/>
   <FolderSize/>
   <HomePage/>
</ManagedFolderInformation>
```

 **ManagedFolderInformationType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CanDelete](candelete.md) <br/> |Указывает, можно ли удалить управляемой папки клиентом.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Указывает, переименованы или перемещены клиентом указанной управляемой папки.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Указывает, должно ли отображаться комментария управляемой папки.  <br/> |
|[HasQuota](hasquota.md) <br/> |Указывает, имеет ли управляемой папки квоту.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Указывает, является ли управляемых папок корневого каталога для всех управляемых папок.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Содержит идентификатор папки из управляемых папок.  <br/> |
|[�����������](comment.md) <br/> |Содержит комментарий, связанный с управляемой папки.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Описывает квоту хранилища для управляемых папок.  <br/> |
|[FolderSize](foldersize.md) <br/> |Описывает общий размер все содержимое управляемых папок.  <br/> |
|[Домашняя страница](homepage.md) <br/> |Задает URL-адрес, который будет по умолчанию домашнюю страницу для управляемых папок.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в хранилище Exchange. Управляемые настраиваемые папки можно только вложенные папки в папку с именем **Управляемых папок**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Не применимо.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Не применимо.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Не применимо.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Неприменимо.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление управляемых папок](http://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

