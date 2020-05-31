---
title: Папки
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Элемент Folders содержит массив папок, которые используются в операциях с папками.
ms.openlocfilehash: 34372f2480825c7a9977eeae8e730c201307f36b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353590"
---
# <a name="folders"></a>Folders

Элемент **Folders** содержит массив папок, которые используются в операциях с папками. 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

**Аррайоффолдерстипе** или **нонемптяррайоффолдерстипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Определяет папку для создания, получения, поиска, синхронизации или обновления.  <br/> |
|[календарфолдер](calendarfolder.md) <br/> |Представляет папку, в которой в основном содержатся элементы календаря.  <br/> |
|[контактсфолдер](contactsfolder.md) <br/> |Представляет папку "Контакты" в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащуюся в почтовом ящике.  <br/> |
|[тасксфолдер](tasksfolder.md) <br/> |Представляет папку Tasks в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[копифолдерреспонсемессаже](copyfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CopyFolder](copyfolder-operation.md) .  <br/> |
|[CreateFolder](createfolder.md) <br/> |Определяет запрос на создание папки в хранилище Exchange.  <br/> |
|[креатефолдерреспонсемессаже](createfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateFolder](createfolder-operation.md) .  <br/> |
|[креатеманажедфолдерреспонсемессаже](createmanagedfolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции CreateManagedFolder](createmanagedfolder-operation.md) .  <br/> |
|[жетфолдерреспонсемессаже](getfolderresponsemessage.md) <br/> |Содержит состояние и результат запроса операции " [операция с папкой](getfolder-operation.md) ".  <br/> |
|[мовефолдерреспонсемессаже](movefolderresponsemessage.md) <br/> |Содержит состояние и результат запроса [операции MoveFolder](movefolder-operation.md) .  <br/> |
|[ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) <br/> |Определяет папку, в которой создается новая папка.  <br/> |
|[Рутфолдер (Финдфолдерреспонсемессаже)](rootfolder-findfolderresponsemessage.md) <br/> |Содержит результаты поиска в одной корневой папке во время [операции FindFolder](findfolder-operation.md).  <br/> |
|[упдатефолдерреспонсемессаже](updatefolderresponsemessage.md) <br/> |Содержит состояние и результат одного запроса [операции операцию UpdateFolder](updatefolder-operation.md) .  <br/> |
   
## <a name="remarks"></a>Примечания

Этот элемент является обязательным дочерним элементом элемента [ParentFolderId (таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md) . 
  
Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера под управлением Microsoft Exchange Server 2010, на котором установлена роль сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [ParentFolderId (Таржетфолдеридтипе)](parentfolderid-targetfolderidtype.md)

