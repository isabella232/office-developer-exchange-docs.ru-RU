---
title: Update (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: Элемент обновления определяет один элемент для обновления в локальном хранилище клиента.
ms.openlocfilehash: bf560f18184151a3f17d7016d05cdb725db934ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353632"
---
# <a name="update-itemsync"></a>Update (ItemSync)

**Обновить** элемент определяет один элемент для обновления в локальном хранилище клиента. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md)  
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md)  
- [Changes (Items)](changes-items.md)  
- [Update (ItemSync)](update-itemsync.md)
  
```xml
<Update>
   <Item/>
</Update>
```

```xml
<Update>
   <MeetingRequest/>
</Update>
```

```xml
<Update>
   <MeetingCancellation/>
</Update>
```

```xml
<Update>
   <Task/>
</Update>
```

```xml
<Update>
   <CalendarItem/>
</Update>
```

```xml
<Update>
   <MeetingResponse/>
</Update>
```

```xml
<Update>
   <Message/>
</Update>
```

```xml
<Update>
   <DistributionList/>
</Update>
```

```xml
<Update>
   <MeetingMessage/>
</Update>
```

```xml
<Update>
   <Contact/> 
</Update>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange для обновления.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange для обновления.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange для обновления.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange для обновления.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки, чтобы обновить.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания для обновления.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашения на собрание для обновления.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение для обновления.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмены собрания для обновления.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу для обновления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Содержит массив последовательности типов изменений, которые представляют тип различия между элементами на стороне клиента и элементов на сервере Exchange.  <br/> |
   
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

- [Операция SyncFolderItems](syncfolderitems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

