---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Элемент Contains представляет собой выражение поиска, определяющие, содержит ли заданное свойство постоянное значение строки.
ms.openlocfilehash: 6e36ede6a10c64a4aa53e68721d9edf7893c4c05
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 09/24/2021
ms.locfileid: "59547549"
---
# <a name="contains"></a>Contains

Элемент **Contains** представляет собой выражение поиска, определяющие, содержит ли заданное свойство постоянное значение строки. 
  
```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <FieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <ExtendedFieldURI/>
   <Constant/>
</Contains>
```

```xml
<Contains ContainmentMode="" ContainmentComparison="">
   <IndexedFieldURI/>
   <Constant/>
</Contains>
```


**ContainsExpressionType**

## <a name="attributes-and-elements"></a>Атрибуты и элементы

В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.
  
### <a name="attributes"></a>Атрибуты

|**Атрибут**|**Описание**|
|:-----|:-----|
|**ContainmentMode** <br/> |Определяет границы поиска.  <br/> |
|**ContainmentComparison** <br/> |Определяет, игнорирует ли поиск случаи и пробелы.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Значения атрибута ContainmentMode

|**Значение**|**Описание**|
|:-----|:-----|
|FullString  <br/> |Сравнение между полной строкой и константой. Значение свойства и поставленная константа точно такие же.  <br/> |
|Префикс  <br/> |Сравнение между префиксом строки и константой.  <br/> |
|Подстройка  <br/> |Сравнение между подстройкой строки и константой.  <br/> |
|PrefixOnWords  <br/> |Сравнение между префиксом отдельных слов в строке и константой.  <br/> |
|ExactPhrase  <br/> |Сравнение между точной фразой в строке и константой.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Значения атрибута ContainmentComparison

|**Значение**|**Описание**|
|:-----|:-----|
|Точный  <br/> |Сравнение должно быть точным.  <br/> |
|IgnoreCase  <br/> |Сравнение игнорирует оболочку.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |Сравнение игнорирует не интервальные символы.  <br/> |
|Loose  <br/> |Удалить.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |Сравнение игнорирует символы оболочки и не интервалы.  <br/> |
|LooseAndIgnoreCase  <br/> |Удалить.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |Удалить.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |Удалить.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Определяет часто ссылаясь свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Определяет отдельных членов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Определяет свойства MAPI.  <br/> |
|[Константа](constant.md) <br/> |Определяет постоянное значение в ограничении.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в операциях FindItem/FindFolder и папках поиска.  <br/> |
|[Not](not.md) <br/> |Представляет выражение поиска, которое отменяет значение Boolean содержащемся в нем выражения поиска.  <br/> |
|[And](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять boolean и операцию между двумя или более выражениями поиска. Результат операции And является **верным,** если все выражения поиска, содержащиеся в И являются **верными.**  <br/> |
|[Or](or.md) <br/> |Представляет выражение поиска, которое выполняет логическое или логическое выражение поиска, содержащемся в нем. Элемент [Or](or.md) возвращается **true,** если любой из его детей **возвращается true**.  <br/> |
   
## <a name="remarks"></a>Заметки

Атрибуты используются для определения совпадения элементов.
  
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

