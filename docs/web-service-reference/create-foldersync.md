---
title: Создание (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Create
api_type:
- schema
ms.assetid: 6b463d0a-70e9-40c5-ade4-c7d9a5f36bc1
description: Создать элемент идентифицирует одной папке для создания в локальном хранилище клиента.
ms.openlocfilehash: 867eecb89c115b008d4828e162b21d078eba695c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761850"
---
# <a name="create-foldersync"></a>Создание (FolderSync)

**Создать** элемент идентифицирует одной папке для создания в локальном хранилище клиента. 
  
[SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md)
  
[ResponseMessages](responsemessages.md)
  
[SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)
  
[Изменения (иерархии)](changes-hierarchy.md)
  
[Создание (FolderSync)](create-foldersync.md)
  
```xml
<Create>
   <Folder/>
   <CalendarFolder/>
   <ContactsFolder/>
   <SearchFolder/>
   <TasksFolder/>
</Create>
```

 **SyncFolderHierarchyCreateOrUpdateType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Определяет папку для создания, получение, найти, синхронизировать или обновить.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку, содержащую элементы календаря в первую очередь.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папке контактов в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска, содержащихся в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач, содержащихся в почтовом ящике.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Изменения (иерархии)](changes-hierarchy.md) <br/> |Содержит массив последовательности типов изменений, которые представляют тип различия между элементами на стороне клиента и элементов на сервере Exchange.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[Операция SyncFolderItems](syncfolderitems-operation.md)


- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

