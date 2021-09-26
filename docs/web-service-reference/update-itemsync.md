---
title: Update (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Update
api_type:
- schema
ms.assetid: 4e204446-1c80-44f9-b93b-77ce630a01a5
description: Элемент Update определяет один элемент для обновления в локальном клиентской магазине.
ms.openlocfilehash: 936226c671916b974eed9dea9ad2ea39bde482a9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541821"
---
# <a name="update-itemsync"></a>Update (ItemSync)

Элемент **Update** определяет один элемент для обновления в локальном клиентской магазине. 
  
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
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение Exchange электронной почты для обновления.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент Exchange календаря для обновления.  <br/> |
|[Contact](contact.md) <br/> |Представляет элемент Exchange для обновления.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки для обновления.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания для обновления.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет запрос на собрание для обновления.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ собрания на обновление.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания для обновления.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу обновления.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Содержит массив типов изменений последовательности, которые представляют тип различий между элементами на клиенте и элементами на Exchange сервере.  <br/> |
   
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

- [Операция SyncFolderItems](syncfolderitems-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

