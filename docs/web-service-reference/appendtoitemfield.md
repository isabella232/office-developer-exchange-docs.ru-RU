---
title: AppendToItemField
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AppendToItemField
api_type:
- schema
ms.assetid: 66dbcb4a-ae6d-4648-8610-67187bdb105c
description: Элемент AppendToItemField определяет данные для приложения к одному свойству элемента во время операции UpdateItem.
ms.openlocfilehash: 8e94ca9174d11f1f6e4a0dd2fcfabeb30a64a40d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540330"
---
# <a name="appendtoitemfield"></a>AppendToItemField

Элемент **AppendToItemField** определяет данные для приложения к одному свойству элемента во время операции [UpdateItem.](updateitem-operation.md)
  
- [UpdateItem](updateitem.md)
  
- [ItemChanges](itemchanges.md)
  
- [ItemChange](itemchange.md)
  
- [Updates (Item)](updates-item.md)
  
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
|[FieldURI](fielduri.md) <br/> |Определяет часто ссылаясь свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Определяет отдельных членов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет расширенные свойства MAPI для приложения.  <br/> |
|[Элемент](item.md) <br/> |Представляет элемент в хранилище Exchange.  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Представляет сообщение электронной почты Exchange.  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Представляет элемент календаря Exchange.  <br/> |
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
|[Updates (Item)](updates-item.md) <br/> |Содержит массив, который определяет приложения, набор и удаление изменений свойств элементов.  <br/> Ниже приводится выражение XPath к этому элементу:  `/UpdateItem/ItemChanges/ItemChange[i]/Updates` <br/> |
   
## <a name="remarks"></a>Заметки

Операции приложения поддерживаются только определенными свойствами. Попытка приложения к свойству, которое не поддерживает приложение, приведет к ошибке.
  
Для операций обновления в одном запросе может быть изменено только одно свойство. Это одно свойство должно ссылаться в [элементе Path.](path.md) Элемент **Item** в производных классах может удерживать только одно свойство, которое согласовано с одним **элементом Path.** 
  
> [!NOTE]
> Элемент [Path](path.md) абстрактный. Он должен быть заменен элементом [FieldURI,](fielduri.md) [IndexedFieldURI](indexedfielduri.md)или [ExtendedFieldURI.](extendedfielduri.md) 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateItem](updateitem-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

