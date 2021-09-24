---
title: ManagedFolderInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ManagedFolderInformation
api_type:
- schema
ms.assetid: dea980eb-8303-47fe-a380-20a8efc9ead6
description: Элемент ManagedFolderInformation содержит сведения об управляемой пользовательской папке.
ms.openlocfilehash: f25daeff82b4a30574a627f290c2fcd336a38a6c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524800"
---
# <a name="managedfolderinformation"></a>ManagedFolderInformation

Элемент **ManagedFolderInformation содержит** сведения об управляемой пользовательской папке. 
  
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
|[CanDelete](candelete.md) <br/> |Указывает, может ли клиент удалить управляемые папки.  <br/> |
|[CanRenameOrMove](canrenameormove.md) <br/> |Указывает, может ли клиент переименовать или перенаправить указанную управляемой папку.  <br/> |
|[MustDisplayComment](mustdisplaycomment.md) <br/> |Указывает, должен ли отображаться комментарий управляемой папки.  <br/> |
|[HasQuota](hasquota.md) <br/> |Указывает, имеет ли у управляемой папки квота.  <br/> |
|[IsManagedFoldersRoot](ismanagedfoldersroot.md) <br/> |Указывает, является ли управляемый папка корнем для всех управляемых папок.  <br/> |
|[ManagedFolderId](managedfolderid.md) <br/> |Содержит ID папки управляемой папки.  <br/> |
|[Comment](comment.md) <br/> |Содержит комментарий, связанный с управляемой папкой.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Описывает квоту хранения для управляемой папки.  <br/> |
|[FolderSize](foldersize.md) <br/> |Описывает общий размер всего содержимого управляемой папки.  <br/> |
|[HomePage](homepage.md) <br/> |Указывает URL-адрес, который будет домашней страницей по умолчанию для управляемой папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в Exchange магазине. Управляемые пользовательские папки могут быть только подмостки папки с именем **Управляемые папки**.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Неприменимо.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Неприменимо.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Неприменимо.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Неприменимо.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

