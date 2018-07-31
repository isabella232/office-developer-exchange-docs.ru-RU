---
title: Create (ItemSync)
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
ms.assetid: cb5e64a2-66a5-4447-921e-7c13efb8f6bf
description: Создать элемент определяет один элемент для создания в локальном хранилище клиента.
ms.openlocfilehash: d49e54c64f7bd53dcb296d998a856c20570d81be
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353947"
---
# <a name="create-itemsync"></a>Create (ItemSync)

**Создать** элемент определяет один элемент для создания в локальном хранилище клиента. 
  
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
|[Сообщение](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange для создания.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange для создания.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange для создания.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки, чтобы создать.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет сообщение собрания для создания.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет Создание приглашения на собрание.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение для создания.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмены собрания для создания.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу для создания.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Changes (Items)](changes-items.md) <br/> |Содержит массив последовательности типов изменений, которые представляют типы различия между элементами на стороне клиента и элементов на сервере Exchange.  <br/> |
   
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

