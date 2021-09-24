---
title: Occurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: Элемент Occurrence представляет собой одно изменение повторяющегося элемента календаря.
ms.openlocfilehash: 465c02263eadfc74629a8e21ebccf076206ec0d2
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518094"
---
# <a name="occurrence"></a>Occurrence

Элемент **Occurrence** представляет собой одно изменение повторяющегося элемента календаря. 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

**OccurrenceInfoType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

Нет.
  
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ItemId](itemid.md) <br/> |Содержит уникальный идентификатор и ключ изменения измененного появления повторяющегося элемента календаря.  <br/> |
|[Start](start.md) <br/> |Представляет время начала изменения возникновения повторяющегося элемента календаря.  <br/> |
|[End ](end-ex15websvcsotherref.md) <br/> |Представляет собой конечное время изменения вхождения повторяющегося элемента календаря.  <br/> |
|[OriginalStart](originalstart.md) <br/> |Представляет исходное время начала изменения возникновения повторяющегося элемента календаря.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[ModifiedOccurrences](modifiedoccurrences.md) <br/> |Содержит коллекцию повторяющихся вхождений элементов календаря, которые были изменены таким образом, чтобы они отличались от обычного элемента повторяемости.  <br/> |
   
## <a name="remarks"></a>Заметки

Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

