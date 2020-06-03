---
title: оккурренцеитемид
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OccurrenceItemId
api_type:
- schema
ms.assetid: 4a15bbc3-5b93-4193-b9ec-da32f0a9a552
description: Элемент Оккурренцеитемид определяет один экземпляр повторяющегося элемента.
ms.openlocfilehash: 37c3a2442afb3302bca88ef0301e98013ff0319b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468378"
---
# <a name="occurrenceitemid"></a>оккурренцеитемид

Элемент **оккурренцеитемид** определяет один экземпляр повторяющегося элемента. 
  
```XML
<OccurrenceItemId RecurringMasterId="" ChangeKey="" InstanceIndex=""/>
```

**оккурренцеитемидтипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**рекуррингмастерид** <br/> |Определяет шаблон повторяющегося элемента повторяющегося элемента. Этот атрибут является обязательным.  <br/> |
|**чанжекэй** <br/> |Определяет определенную версию шаблона повторения или вхождение элемента. При изменении одного или обоих его повторений **чанжекэй** изменяется. **Чанжекэй** одинаково для шаблона повторения и всех вхождений.  <br/> |
|**инстанцеиндекс** <br/> |Определяет индекс экземпляра элемента. Этот атрибут является обязательным. Это значение представляет целое число.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[глобалитемидс](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.  <br/> |
|[итемидс](itemids.md) <br/> | Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange. <br/><br/>Ниже приведены выражения XPath для этого элемента. <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/><br/>**Note**: [Операция MoveItem](moveitem-operation.md) и [CopyItem](copyitem-operation.md) работают только с одними элементами календаря и повторяющимися элементами шаблона. Недопустимые вхождения элементов для этих операций.           |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления, применяемые к элементу.<br/><br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В приведенном ниже примере показано, как определить Четвертый экземпляр повторяющегося элемента с идентификатором 34vswe4.
  
```XML
<OccurrenceItemId RecurringMasterId="34vswe4" InstanceIndex="4" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [рекуррингмастеритемид](recurringmasteritemid.md)
- [Операция FindConversation](findconversation-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

