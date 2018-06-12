---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: Элемент EffectiveRights содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения.
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762262"
---
# <a name="effectiverights"></a>EffectiveRights

Элемент **EffectiveRights** содержит права клиента на основании параметров разрешений для элемента или папки. Этот элемент доступен только для чтения. 
  
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
|[CreateAssociated](createassociated.md) <br/> |Указывает ли клиента можно создать таблицу связанного содержимого. Это свойство используется только для объектов папки.  <br/> |
|[CreateContents](createcontents.md) <br/> |Указывает ли клиента можно создать таблицу содержимого. Это свойство используется только для объектов папки.  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |Указывает ли клиента можно создать таблицу иерархии. Это свойство используется только для объектов папки.  <br/> |
|[удаление](delete.md); <br/> |Указывает, будет ли это клиент можно удалить папку или элемент.  <br/> |
|[Изменение](modify.md) <br/> |Указывает, будет ли это клиент можно изменить папку или элемент.  <br/> |
|[Чтение](read.md) <br/> |Указывает, будет ли это клиент могут читать папку или элемент.  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |Указывает ли закрытый элемент можно просмотреть.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Folder](folder.md) <br/> |Представляет папку в почтовом ящике.  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |Представляет папку задачи в почтовом ящике.  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |Представляет папку контактов в почтовом ящике.  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |Представляет папку Календарь в почтовом ящике.  <br/> |
|[SearchFolder](searchfolder.md) <br/> |Представляет папку поиска в почтовом ящике.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
|[PostItem](postitem.md) <br/> |Представляет элемент post в хранилище Exchange.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

**EffectiveRights** поддерживается в ответы GetFolder, GetItem, FindFolder, FindItem, SyncFolderHierarchy и SyncFolderItems. Свойство **EffectiveRights** предоставляется в фигуре **AllProperties** для папок и элементов. 
  
Это свойство **EffectiveRights** предоставляет доступ к те же данные, предоставляемая в свойстве **PR_ACCESS MAPI** . 
  
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
- [Setting Folder-Level Permissions](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

