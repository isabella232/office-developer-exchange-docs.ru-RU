---
title: Create (ItemSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Create
api_type:
- schema
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Элемент Create определяет один элемент, который необходимо создать в локальном клиентской магазине.
ms.openlocfilehash: 2b36fad021c7ccb767eb80b31f71f12ef6cbbd22
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510339"
---
# <a name="create-itemsync"></a>Create (ItemSync)

Элемент **Create** определяет один элемент, который необходимо создать в локальном клиентской магазине. 
  
- [SyncFolderItemsResponse](syncfolderitemsresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [SyncFolderItemsResponseMessage](syncfolderitemsresponsemessage.md) 
- [Changes (Items)](changes-items.md) 
- [Create (ItemSync)](create-itemsync.md)
  
```xml
<Create>
   <Item/>
</Create>
```

```xml
<Create>
   <Task/> 
</Create>
```

```xml
<Create>
   <MeetingResponse/>
</Create>
```

```xml
<Create>
   <CalendarItem/>
</Create>
```

```xml
<Create>
   <MeetingMessage/>
</Create>
```

```xml
<Create>
   <DistributionList/>
</Create>
```

```xml
<Create>
   <MeetingCancellation/>
</Create>
```

```xml
<Create>
   <MeetingRequest/> 
</Create>
```

```xml
<Create>
   <Message/> 
</Create>
```

```xml
<Create>
   <Contact/> 
</Create>
```

**SyncFolderItemsCreateOrUpdateType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Элемент](item.md) <br/> |Представляет универсальный элемент Exchange для создания.  <br/> |
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет собой Exchange для создания сообщения электронной почты.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент Exchange календаря для создания.  <br/> |
|[Contact](contact.md) <br/> |Представляет элемент Exchange для создания.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки для создания.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания для создания.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет запрос на собрание для создания.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ собрания для создания.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания для создания.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу для создания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Содержит массив типов изменений последовательности, которые представляют типы различий между элементами клиента и элементами на Exchange сервере.  <br/> |
   
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

