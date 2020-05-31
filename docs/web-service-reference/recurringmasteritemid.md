---
title: рекуррингмастеритемид
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
description: Элемент Рекуррингмастеритемид определяет элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения.
ms.openlocfilehash: ae59e33ece55d85435ece4c9030ccda32eb62eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835015"
---
# <a name="recurringmasteritemid"></a>рекуррингмастеритемид

Элемент **рекуррингмастеритемид** определяет элемент шаблона повторения, определяя идентификаторы одного из связанных элементов вхождения. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **рекуррингмастеритемидтипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**оккурренцеид** <br/> |Определяет один экземпляр повторяющегося элемента шаблона. Этот атрибут является обязательным.  <br/> |
|**чанжекэй** <br/> |Определяет конкретную версию одного экземпляра повторяющегося элемента шаблона. Кроме того, также идентифицируется шаблон повторяющегося элемента, так как он и один экземпляр будут содержать один и тот же ключ изменения. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[глобалитемидс](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.  <br/> |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления, применяемые к элементу. <br/> <br/> Ниже приведено выражение XPath для этого элемента: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[итемидс](itemids.md) <br/> | Содержит уникальные идентификаторы элементов, элементы вхождений и повторяющиеся элементы шаблона, которые используются для удаления, отправки, получения, перемещения или копирования элементов в хранилище Exchange. <br/> <br/>  Ниже приведены выражения XPath для этого элемента.  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В примере ниже показано, как определить шаблон повторяющегося элемента, определив один из его экземпляров с идентификатором 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [оккурренцеитемид](occurrenceitemid.md)
- [Операция FindConversation](findconversation-operation.md)

