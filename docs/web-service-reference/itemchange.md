---
title: ItemChange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ItemChange
api_type:
- schema
ms.assetid: 5cb43b02-d444-4d9c-9075-cdc5a4427daf
description: Элемент Итемчанже содержит идентификатор элемента и обновления, применяемые к элементу.
ms.openlocfilehash: 916ef1ba2c7a709ec1fd80ababd72999506773c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459919"
---
# <a name="itemchange"></a>ItemChange

Элемент **итемчанже** содержит идентификатор элемента и обновления, применяемые к элементу. 
  
- [UpdateItem](updateitem.md) 
- [итемчанжес](itemchanges.md)
- [ItemChange](itemchange.md)
  
```xml
<ItemChange>
   <ItemId/>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <OccurrenceItemId>...</OccurrenceItemId>
   <Updates>...</Updates>
</ItemChange>
```

```xml
<ItemChange>
   <RecurringMasterItemId>...</RecurringMasterItemId>
   <Updates>...</Updates>
</ItemChange>
```

**итемчанжетипе**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Идентификатор](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения элемента в хранилище Exchange. Этот элемент является обязательным, если элемент [оккурренцеитемид](occurrenceitemid.md) или [рекуррингмастеритемид](recurringmasteritemid.md) не используется.  <br/> |
|[оккурренцеитемид](occurrenceitemid.md) <br/> |Определяет один экземпляр повторяющегося элемента. Этот элемент является обязательным при использовании. Этот элемент является обязательным, если элемент [рекуррингмастеритемид](recurringmasteritemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[рекуррингмастеритемид](recurringmasteritemid.md) <br/> |Определяет элемент шаблона повторения, определив один из идентификаторов связанных элементов вхождения. Этот элемент является обязательным при использовании. Этот элемент является обязательным, если элемент [оккурренцеитемид](occurrenceitemid.md) или [ItemId](itemid.md) не используется.  <br/> |
|[Обновления (элемент)](updates-item.md) <br/> |Содержит массив, определяющий Добавление, установку и удаление изменений свойств элемента. Этот элемент обязательный.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[итемчанжес](itemchanges.md) <br/> |Содержит массив элементов [итемчанже](itemchange.md) , определяющих элементы и обновления, которые необходимо применить к элементам.  <br/> Ниже приведено выражение XPath для этого элемента:  <br/>  `/UpdateItem/ItemChanges` <br/> |
   
## <a name="remarks"></a>Примечания

В элементе **итемчанже** можно использовать только один элемент [ItemId](itemid.md), [оккурренцеитемид](occurrenceitemid.md)или [рекуррингмастеритемид](recurringmasteritemid.md) . 
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция UpdateItem](updateitem-operation.md)

