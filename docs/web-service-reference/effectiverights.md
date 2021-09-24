---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: Элемент EffectiveRights содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.
ms.openlocfilehash: a3207a9971065d3b69b6a0b7056fa8012425fd5b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59514713"
---
# <a name="effectiverights"></a>EffectiveRights

Элемент **EffectiveRights** содержит права клиента на основе параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 **EffectiveRightsType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[CreateAssociated](createassociated.md) <br/> |Указывает, может ли клиент создать связанную таблицу контента. Это свойство используется только для объектов папок.  <br/> |
|[CreateContents](createcontents.md) <br/> |Указывает, может ли клиент создать таблицу контента. Это свойство используется только для объектов папок.  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |Указывает, может ли клиент создать таблицу иерархии. Это свойство используется только для объектов папок.  <br/> |
|[удаление](delete.md); <br/> |Указывает, может ли клиент удалить папку или элемент.  <br/> |
|[Modify](modify.md) <br/> |Указывает, может ли клиент изменить папку или элемент.  <br/> |
|[Read](read.md) <br/> |Указывает, может ли клиент читать папку или элемент.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Указывает, можно ли просматривать частный элемент.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задач в почтовом ящике.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку календаря в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет общий элемент Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент столба в Exchange магазине.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

**EffectiveRights** поддерживается в ответах GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy и SyncFolderItems. Свойство **EffectiveRights** выставлено в форме **AllProperties** для папок и элементов. 
  
Это **свойство EffectiveRights** предоставляет доступ к той же информации, что и **PR_ACCESS MAPI.** 
  
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
- [Setting Folder-Level Permissions](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

