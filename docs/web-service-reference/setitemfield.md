---
title: SetItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetItemField
api_type:
- schema
ms.assetid: 85284fcb-bd1e-4fda-9dab-cb4cd637cd5b
description: Элемент SetItemField представляет отдельное свойство элемента в рамках одной операции UpdateItem обновление.
ms.openlocfilehash: 012e6ae21af653b4bf12588e5a97334a62884059
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835439"
---
# <a name="setitemfield"></a>SetItemField

Элемент **SetItemField** представляет отдельное свойство элемента в рамках одной [операции UpdateItem](updateitem-operation.md)обновление.
  
```xml
<SetItemField>
   <FieldURI/>
   <Item/>
</SetItemField>
```

 **SetItemFieldType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает расширенные свойства MAPI для установки.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange для обновления.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange для обновления.  <br/> |
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
|[Обновления (элемент)](updates-item.md) <br/> |Содержит набор элементов, которые определяют добавьте, Установка и удаление изменения свойств элемента.  <br/> |
   
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также



[UpdateItem Operation](updateitem-operation.md)

