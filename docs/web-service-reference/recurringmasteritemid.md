---
title: RecurringMasterItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurringMasterItemId
api_type:
- schema
ms.assetid: 5800b58c-f3d7-4d8f-acc0-d13e02f4e258
description: Элемент RecurringMasterItemId определяет мастер-элемент повторения, определяя идентификаторы одного из связанных с ним элементов возникновения.
ms.openlocfilehash: d00794f2b5b1893e1829a3f09df9f3e88266964d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59523631"
---
# <a name="recurringmasteritemid"></a>RecurringMasterItemId

Элемент **RecurringMasterItemId** определяет мастер-элемент повторения, определяя идентификаторы одного из связанных с ним элементов возникновения. 
  
```XML
<RecurringMasterItemId OccurrenceId="" ChangeKey="" />
```

 **RecurringMasterItemIdType**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**OccurrenceId** <br/> |Определяет одно возникновение повторяющегося элемента магистра. Этот атрибут является обязательным.  <br/> |
|**ChangeKey** <br/> |Определяет определенную версию одного появления повторяющегося элемента. Кроме того, повторяющийся главный элемент также идентифицирован, так как он и одно возникновение будут содержать один и тот же ключ изменения. Этот атрибут является необязательным.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

Нет.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[GlobalItemIds](globalitemids.md) <br/> |Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.  <br/> |
|[ItemChange](itemchange.md) <br/> |Содержит идентификатор элемента и обновления, которые необходимо применить к элементу. <br/> <br/> Ниже приводится выражение XPath к этому элементу: <br/> <br/>  `/UpdateItem/ItemChanges/ItemChange[i]` <br/> |
|[ItemIds](itemids.md) <br/> | Содержит уникальные удостоверения элементов, элементов возникновения и повторяющихся элементов, используемых для удаления, отправки, получения, перемещения или копирования элементов в Exchange магазине. <br/> <br/>  Ниже приводится выражение XPath к этому элементу:  <br/><br/>  `/DeleteItem/ItemIds` <br/>  `/SendItem/ItemIds` <br/>  `/GetItem/ItemIds` <br/>  `/MoveItem/ItemIds` <br/>  `/CopyItem//ItemIds` <br/> |
   
## <a name="text-value"></a>Текстовое значение

Нет.
  
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.
  
## <a name="example"></a>Пример

В следующем примере определяется повторяющийся мастер-элемент путем определения одного из его случаев с идентификатором 56lkjh6.
  
```XML
<RecurringMasterItemId OccurrenceId="56lkjh6" />
```

## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [OccurrenceItemId](occurrenceitemid.md)
- [Операция FindConversation](findconversation-operation.md)

