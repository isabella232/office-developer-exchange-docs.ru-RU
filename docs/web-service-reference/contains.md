---
title: Contains
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Contains
api_type:
- schema
ms.assetid: 476d059d-c243-43e9-b475-319fc413ade2
description: Элемент Contains представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа.
ms.openlocfilehash: b25b69aadf2c331527a17ad81ed46f61aa7b93c2
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354290"
---
# <a name="contains"></a>Contains

Элемент **Contains** представляет выражение поиска, которое определяет, содержит ли данное свойство указанную константу строчного типа. 
  
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
|**ContainmentComparison** <br/> |Определяет, будет ли поиска игнорироваться регистр и пробелы.  <br/> |
   
#### <a name="containmentmode-attribute-values"></a>Значения атрибутов ContainmentMode

|**Значение**|**Описание**|
|:-----|:-----|
|FullString  <br/> |Полной строки сравнивается константу. Значение свойства и указанная константа, точно совпадают.  <br/> |
|Префикс  <br/> |Префикс строки сравнивается константу.  <br/> |
|Подстроки  <br/> |Подстрока строки сравнивается константу.  <br/> |
|PrefixOnWords  <br/> |Префикс на отдельные слова в строке сравнивается константу.  <br/> |
|ExactPhrase  <br/> |Точной фразы в строке сравнивается константу.  <br/> |
   
#### <a name="containmentcomparison-attribute-values"></a>Значения атрибутов ContainmentComparison

|**Значение**|**Описание**|
|:-----|:-----|
|Точное  <br/> |Сравнение нужно ввести точно.  <br/> |
|IgnoreCase  <br/> |Сравнение не учитывает регистр.  <br/> |
|IgnoreNonSpacingCharacters  <br/> |Сравнение игнорирует дополнительный символов.  <br/> |
|Слабый контроль  <br/> |Требуется удалить.  <br/> |
|IgnoreCaseAndNonSpacingCharacters  <br/> |Сравнение игнорирует строчных букв и дополнительный символов.  <br/> |
|LooseAndIgnoreCase  <br/> |Требуется удалить.  <br/> |
|LooseAndIgnoreNonSpace  <br/> |Требуется удалить.  <br/> |
|LooseAndIgnoreCaseAndIgnoreNonSpace  <br/> |Требуется удалить.  <br/> |
   
### <a name="child-elements"></a>Дочерние элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[FieldURI](fielduri.md) <br/> |Идентифицирует часто упоминаемые свойства по URI.  <br/> |
|[IndexedFieldURI](indexedfielduri.md) <br/> |Идентифицирует отдельных элементов словаря.  <br/> |
|[ExtendedFieldURI](extendedfielduri.md) <br/> |Задает свойства MAPI.  <br/> |
|[Constant](constant.md) <br/> |Задает значение константы в качестве ограничения.  <br/> |
   
### <a name="parent-elements"></a>Родительские элементы

|**Элемент**|**Описание**|
|:-----|:-----|
|[Restriction](restriction.md) <br/> |Представляет ограничение или запрос, используемый для фильтрации элементов или папок в папке операциях FindItem/FindFolder и поиска.  <br/> |
|[Не](not.md) <br/> |Представляет выражение поиска, которое Инвертирует логическое значение выражения поиска, которые он содержит.  <br/> |
|[И](and.md) <br/> |Представляет выражение поиска, которое позволяет выполнять логическое и операции между двумя или более выражений для поиска. Операции получается **значение true,** **Если все выражения поиска, содержащихся в And**.  <br/> |
|[Или](or.md) <br/> |Представляет выражение поиска, используемая для выполнения логического или выражения поиска, которые он содержит. Элемент [или](or.md) возвращает **значение true** , если какие-либо из их дочерних элементов возвращало **значение true**.  <br/> |
   
## <a name="remarks"></a>Замечания

Атрибуты используются для определения сопоставления элементов.
  
Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.
  
## <a name="element-information"></a>Сведения об элементе

|||
|:-----|:-----|
|Пространство имен  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|Имя схемы  <br/> |Схема Types  <br/> |
|Файл проверки  <br/> |Types.xsd  <br/> |
|Может быть пустым  <br/> |False  <br/> |
   
## <a name="see-also"></a>См. также

- [Элементы XML веб-служб Exchange в Exchange](ews-xml-elements-in-exchange.md)

