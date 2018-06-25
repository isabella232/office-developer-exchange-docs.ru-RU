---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: Элемент RecurringMasterItemId определяет элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835015"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

Элемент **RecurringMasterItemId** определяет элемент шаблона повторения с учетом идентификаторы одного из его элементы, связанных с ними вхождение. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**OccurrenceId** <br/> |Определяет одно вхождение повторяющегося элемента шаблона. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Идентифицирует определенной версии одного экземпляра повторяющегося элемента шаблона. Кроме того повторяющегося элемента шаблона также определены, так как он и одно вхождение будет содержать тем же ключом изменений. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления для применения к элементу. <br/> <br/> Ниже приведен выражение XPath для этого элемента. <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[Что ItemID](itemids.md) <br/> | Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся основные элементы, используемые для удаления, отправка, получение, перемещение и копирование элементов в хранилище Exchange. <br/> <br/>  Ниже приведены выражения XPath для этого элемента.  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Замечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

Следующий пример определяет повторяющиеся главных элемент, указав один из его вхождения, содержащие 56lkjh6 идентификатор.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [OccurrenceItemId](occurrenceitemid.md)
- [FindConversation Operation](findconversation-operation.md)

