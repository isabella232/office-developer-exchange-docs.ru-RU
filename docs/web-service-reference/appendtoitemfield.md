---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: Элемент AppendToItemField определяет данные для добавления к отдельное свойство элемента во время операции UpdateItem.
ms.openlocfilehash: b432399e84ee4a3fd7edc5d3f803079435c79143
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761396"
---
# <a name="appendtoitemfield"></a>AppendToItemField

Элемент **AppendToItemField** определяет данные для добавления к отдельное свойство элемента во время [операции UpdateItem](updateitem-operation.md).
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Обновления (элемент)](updates-item.md)
  
- [AppendToItemField](appendtoitemfield.md)
  
```xml
<AppendToItemField>
   <FieldURI/>
   <Item/>
</AppendToItemField>
```

 **AppendToItemFieldType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает расширенные свойства MAPI для добавления.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[Элемента календаря, имеющего](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
|[Контакт](contact.md) <br/> |Представляет элемент контакта Exchange.  <br/> |
|[DistributionList](distributionlist.md) <br/> |Представляет список рассылки.  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Представляет собрание в хранилище Exchange.  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Представляет ответ на приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Представляет приглашение на собрание в хранилище Exchange.  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Представляет отмену собрания в хранилище Exchange.  <br/> |
|[Задача](task.md) <br/> |Представляет задачу в хранилище Exchange.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Обновления (элемент)](updates-item.md) <br/> |Содержит массив, определяющий добавьте, Установка и удаление изменения свойств элемента.  <br/> Ниже приведен выражение XPath для этого элемента.`/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Замечания

Только определенные свойства поддержка добавления операции. При попытке добавить свойство, которое не поддерживает добавление приведет к ошибке.
  
Для операции обновления только одно свойство может быть изменено в рамках одного запроса. Что в элементе [путь](path.md) должен указанный отдельное свойство. **Элемент в производные классы** можно только удержание отдельное свойство, который является согласуется единственный элемент **пути** . 
  
> [!NOTE]
> Элемент [пути](path.md) абстрактный. Он должен быть заменен элемент [FieldURI](fielduri.md), [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI](extendedfielduri.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [UpdateItem Operation](updateitem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

