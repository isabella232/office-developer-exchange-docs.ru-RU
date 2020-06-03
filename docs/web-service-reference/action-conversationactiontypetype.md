---
title: Action (Конверсатионактионтипетипе)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Action
api_type:
- schema
ms.assetid: 8bbc12f2-76c5-4fda-828f-56b2086a0454
description: Элемент Action содержит действие, которое необходимо выполнить для диалога, указанного элементом ConversationId.
ms.openlocfilehash: f97b04b98cdc29bee9aff5fa1fc6f37400b8314c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527546"
---
# <a name="action-conversationactiontypetype"></a>Action (Конверсатионактионтипетипе)

Элемент **Action** содержит действие, которое необходимо выполнить для диалога, указанного элементом [ConversationId](conversationid.md) . 
  
- [ApplyConversationAction](applyconversationaction.md)
  
- [конверсатионактионс](conversationactions.md)
  
- [конверсатионактион](conversationaction.md)
  
- [Action (Конверсатионактионтипетипе)](action-conversationactiontypetype.md)
  
```XML
<Action> AlwaysCategorize | AlwaysDelete | AlwaysMove | Delete | Move | Copy | SetReadState </Action>
```

 **конверсатионактионтипетипе**
## <a name="attributes-and-elements"></a>Атрибуты и элементы

В следующих разделах описываются атрибуты, дочерние и родительские элементы.
  
### <a name="attributes"></a>Атрибуты

Отсутствуют.
  
### <a name="child-elements"></a>Дочерние элементы

Отсутствуют.
  
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[конверсатионактион](conversationaction.md) <br/> |Содержит одно действие, которое будет применено к одной беседе.  <br/> |
   
## <a name="text-value"></a>Текстовое значение

Текстовое значение элемента **Action** указывает, какое действие будет выполнено для беседы. Ниже приведены возможные текстовые значения и соответствующие действия. 
  
- **Алвайскатегоризе** . для текущих элементов и новых элементов в беседе будут автоматически заданы категории, указанные в элементе [Categories](categories-ex15websvcsotherref.md) . 
    
- **Алвайсделете** — текущие элементы и новые элементы беседы будут автоматически удалены. Режим удаления задается элементом [делететипе](deletetype.md) . 
    
- **Алвайсмове** — текущие элементы и новые элементы в беседе будут автоматически перемещены в папку, определяемую элементом [дестинатионфолдерид](destinationfolderid.md) . 
    
- **Delete** — будут удалены текущие элементы беседы. Последующие элементы беседы не будут удалены. Режим удаления задается элементом [делететипе](deletetype.md) . 
    
- **Move** — текущие элементы беседы будут перемещены в папку, указанную элементом [дестинатионфолдерид](destinationfolderid.md) . Последующие элементы беседы не будут перемещены. 
    
- **Copy** — текущие элементы в беседе будут скопированы в папку, определяемую элементом [дестинатионфолдерид](destinationfolderid.md) . Последующие элементы беседы не будут скопированы. 
    
- **Сетреадстате** . для текущих элементов беседы будет задано состояние чтения. Состояние чтения задается элементом [читал](isread.md) . 
    
- **Flag** — флагы для текущих элементов в беседе будут установлены, как определено элементом [Flag](flag.md) . 
    
## <a name="remarks"></a>Примечания

Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types. xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Операция ApplyConversationAction](applyconversationaction-operation.md)
- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

