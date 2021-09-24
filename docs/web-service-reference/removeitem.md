---
title: RemoveItem
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RemoveItem
api_type:
- schema
ms.assetid: 766878e3-9007-454f-8501-45139bc5c0e2
description: Элемент RemoveItem представляет объект отклика, который используется для удаления элемента собрания при получении сообщения MeetingCancellation.
ms.openlocfilehash: 4dbe9ede36bf6e3c008a2186cfe617519ecfae1f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517961"
---
# <a name="removeitem"></a>RemoveItem

Элемент **RemoveItem представляет** объект отклика, который используется для удаления элемента собрания при получении сообщения MeetingCancellation. 
  
```xml
<RemoveItem ObjectName="">
   <ReferenceItemId/>
</RemoveItem>
```

 **RemoveItemType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ObjectName** <br/> |Представляет имя объекта-объекта RemoveItem в качестве английской строки.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ReferenceItemId](referenceitemid.md) <br/> |Определяет элемент, к которому относится объект ответа RemoveItem.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Items (NonEmptyArrayOfAllItemsType)](items-nonemptyarrayofallitemstype.md) <br/> |Содержит массив элементов, которые необходимо создать в папке, идентифицированной элементом [ParentFolderId (TargetFolderIdType).](parentfolderid-targetfolderidtype.md)  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Содержит коллекцию всех объектов отклика, связанных с элементом в Exchange магазине.  <br/> |
   
## <a name="remarks"></a>Заметки

 **RemoveItem** действителен только для [MeetingCancellation.](meetingcancellation.md) В противном случае ошибка будет выброшена.
  
> [!NOTE]
> [ItemClass для](itemclass.md) отмены собрания — это IPM. Schedule.Meeting.Canceled. 
  
Чтобы удалить [объект MeetingRequest](meetingrequest.md) и связанный [с ним CalendarItem,](calendaritem.md)используйте объект ответа [DeclineItem](declineitem.md) вместо **RemoveItem.**
  
 **RemoveItem** не поддерживается для доступа делегатов. 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

