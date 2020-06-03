---
title: манажедфолдеринформатион
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
description: Элемент Манажедфолдеринформатион содержит сведения о настраиваемой управляемой папке.
ms.openlocfilehash: ce15dcb15cccdce253494beefd2f4a2a7a0c0ad8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44450951"
---
# <a name="managedfolderinformation"></a>манажедфолдеринформатион

Элемент **манажедфолдеринформатион** содержит сведения о настраиваемой управляемой папке. 
  
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

 **манажедфолдеринформатионтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[канделете](candelete.md) <br/> |Указывает, может ли клиент удалить управляемую папку.  <br/> |
|[канренамеормове](canrenameormove.md) <br/> |Указывает, может ли пользователь переименование или перемещение данной управляемой папки.  <br/> |
|[мустдисплайкоммент](mustdisplaycomment.md) <br/> |Указывает, должен ли отображаться комментарий к управляемой папке.  <br/> |
|[хаскуота](hasquota.md) <br/> |Указывает, есть ли у управляемой папки квота.  <br/> |
|[исманажедфолдерсрут](ismanagedfoldersroot.md) <br/> |Указывает, является ли управляемая папка корневой для всех управляемых папок.  <br/> |
|[манажедфолдерид](managedfolderid.md) <br/> |Содержит идентификатор управляемой папки.  <br/> |
|[Comment](comment.md) <br/> |Содержит комментарий, связанный с управляемой папкой.  <br/> |
|[StorageQuota](storagequota.md) <br/> |Описывает квоту хранилища для управляемой папки.  <br/> |
|[FolderSize](foldersize.md) <br/> |Описывает общий размер всего содержимого управляемой папки.  <br/> |
|[HomePage](homepage.md) <br/> |Задает URL-адрес, который будет домашней страницей по умолчанию для управляемой папки.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в хранилище Exchange. Управляемые папки могут быть только вложенными папками с именем " **управляемые папки**".  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Не применимо.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Не применимо.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Не применимо.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Неприменимо.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция CreateManagedFolder](createmanagedfolder-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)


[Добавление управляемых папок](https://msdn.microsoft.com/library/846658c6-7043-40fb-8439-19f97c2a967f%28Office.15%29.aspx)

