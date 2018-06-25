---
title: Используйте фильтры поиска с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Узнайте, как использовать фильтры поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 0652c36fd610c2f9dfe22b55323b368997137e0c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761139"
---
# <a name="use-search-filters-with-ews-in-exchange"></a>Используйте фильтры поиска с помощью веб-служб Exchange в Exchange

Узнайте, как использовать фильтры поиска с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Фильтры поиска являются основным средством для выражения условия поиска в управляемый API EWS или приложение веб-служб Exchange. Рекомендуется использовать фильтры поиска, в отличие от [строки запроса](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), чтобы выполнить перечисленные ниже:
  
- Поиск на определенное свойство или набор свойств.  
- Поиск с использованием нескольких условий поиска.
    
Фильтры поиска являются единственным вариантом при выполнении одной из следующих:
  
- Поиск настраиваемых свойств.  
- Выполняет поиск для выполнения строк с учетом регистра.  
- Выполняется поиск точного совпадения строки или префикс для выполнения. 
- Для выполнения битовой маски выполняется поиск.
- Поиск элементов, которые имеют определенное свойство задано, независимо от значения.
- Поиск папок.
- Создание папки поиска.
    
## <a name="determine-what-type-of-search-filter-you-need"></a>Определите, какой тип фильтра поиска нужно
<a name="bk_SelectFilter"> </a>

Перед созданием поисковый фильтр сначала определите, какой тип фильтра. Типы фильтра реализуются потомкам классы класса [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в управляемый API веб-служб Exchange, а дочерние элементы элемента [ограничение](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в веб-служб Exchange. 
  
**В таблице 1. Типы фильтров поиска**

|**Тип фильтра**|**Управляемый API EWS класс**|**Элемент веб-служб Exchange**|**Описание**|
|:-----|:-----|:-----|:-----|
|Содержит фильтра  <br/> |[ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |Наиболее тип фильтра для использования для сравнения строк. Позволяет управлять регистра, следует ли игнорировать пробел и устанавливать вложенности режим.  <br/> |
|Битовая маска фильтра  <br/> |[ExcludesBitmask](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[Исключает](http://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |Можно найти целое число свойств как битовой маски и возвращать только результаты, соответствующий указанного Битовая маска, которая неопределенные битов.  <br/> |
|Существует ли фильтр  <br/> |[Существует](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[Существует](http://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |Возвращает все элементы, которые имеют этот параметр указан, независимо от того, значение указанного свойства.  <br/> |
|Равенство фильтра  <br/> |[Выражение IsEqualTo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [IsNotEqualTo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[Выражение IsEqualTo](http://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [IsNotEqualTo](http://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |Сравнивает значение указанного свойства с указанным константа или значение другого свойства и возвращаются все элементы, которые имеют одинаковые значения (в случае фильтром **выражение IsEqualTo** ) или не равно значение (в случае **IsNotEqualTo **фильтр).  <br/> |
|Реляционные тестирования фильтра  <br/> |[IsGreaterThan](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [IsGreaterThanOrEqualTo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [IsLessThan](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [IsLessThanOrEqualTo](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[IsGreaterThan](http://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [IsGreaterThanOrEqualTo](http://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [IsLessThan](http://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [IsLessThanOrEqualTo](http://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |Возвращает все элементы, для которых значение для указанного свойства в соответствующие отношения для указанного константа или другого свойства. К примеру фильтром **IsGreaterThan** возвращает все элементы, которые имеют значение, которое больше, чем значение, указанное в указанное свойство.  <br/> |
|Операция над значением фильтра  <br/> |[Не](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[Не](http://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |Инвертирует результат другие фильтры.  <br/> |
|Составные фильтра  <br/> |[SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[И](http://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [Или](http://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |Объединяет несколько фильтров, позволяя выполнять более сложные условия поиска.  <br/> |
   
### <a name="contains-filter"></a>Содержит фильтра

Содержит объект фильтра — это лучший вариант для поиска свойства строки. С помощью содержит фильтра, можно управлять аспектами сравнения строк, таких как учет регистра букв и порядок обработки пробелы, задав вложенности режим и режим сравнения.
  
#### <a name="contains-filter-in-the-ews-managed-api"></a>Содержит фильтр в управляемый API веб-служб Exchange
<a name="bk_ContainsEWSMA"> </a>

Если вы используете управляемый API веб-служб Exchange, режим вложения с помощью свойства [ContainmentMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) класса [ContainsSubstring](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) и задайте режим сравнения с помощью свойства [ComparisonMode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) ** ContainsSubstring** класса. Следующем примере показано, как создать фильтр поиска, которая выполняет поиск поле темы элементов поиск подстроки «собрания». В этом примере не учитывает регистр, но не пропускает пробелы. 
  
```cs
// Find all items with a subject that contain the substring
// "meeting notes", regardless of case.
// Matches include:
//   - meeting notes
//   - Meeting Notes
//   - Here are my meeting notes
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
```

#### <a name="contains-filter-in-ews"></a>Содержит фильтра в веб-служб Exchange
<a name="bk_ContainsEWSMA"> </a>

В веб-служб Exchange режим вложения с помощью атрибута **ContainmentMode** на элемент [Contains](http://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) и задайте режим сравнения с помощью атрибута **ContainmentComparison** на элемент **Contains** . Следующем примере показано, как создать фильтр поиска для поиска в поле Тема элементов поиск подстроки «собрания». В этом примере не учитывает регистр, но не пропускает пробелы. 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a>Битовая маска фильтра

Битовая маска фильтра позволяет вам для поиска свойств целое число как битовой маски и возвращать результаты которой определенные биты не установлено в значение указанного свойства.
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a>Битовая маска фильтра в управляемый API веб-служб Exchange

Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые имеют значение в настраиваемое свойство **ItemIndex** (определенные в [Пример: поиск элементов с помощью поисковый фильтр и управляемый API EWS](#bk_ExampleEWSMA) раздела этой статьи), не имеющие второй бит (10 в двоичном формате). 
  
```cs
// Find all items with a value of the custom property that does not
// have the second bit (0010) set.
// Matches include:
//   - Property not set
//   - 1 (0001)
//   - 4 (0100)
//   - 5 (0101)
//   - 8 (1000)
SearchFilter.ExcludesBitmask bit2NotSetFilter = 
    new SearchFilter.ExcludesBitmask(customPropDefinition, 2);
```

#### <a name="bitmask-filter-in-ews"></a>Битовая маска фильтра в веб-служб Exchange

Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые имеют значение в настраиваемое свойство **ItemIndex** (определенные в [Пример: поиск элементов с помощью поисковый фильтр и управляемый API EWS](#bk_ExampleEWSMA) этой статьи) у которых нет второй бит (10 в двоичном формате). 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a>Существует ли фильтр

Существует ли фильтр позволяет выполнять поиск для элементов, которые имеют определенное свойство задать для них, независимо от значения.
  
#### <a name="exists-filter-in-the-ews-managed-api"></a>Существует ли фильтр в управляемый API веб-служб Exchange

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют пользовательское свойство **ItemIndex** задать. 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a>Существует ли фильтр в веб-служб Exchange

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют пользовательское свойство **ItemIndex** задать. 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a>Равенство фильтра

Равенство фильтры позволяют выполнять поиск всех элементов, которые имеют значение для указанного свойства, определенное значение равно или не равно определенного значения. Значение для сравнения с может быть константа или значение другого свойства для каждого элемента.
  
#### <a name="equality-filter-in-the-ews-managed-api"></a>Равенство фильтр в управляемый API веб-служб Exchange

Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые не будут прочитаны.
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют значение в свойстве **ItemIndex** , не равно размер элемента. 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a>Равенство фильтра в веб-служб Exchange

Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, которые не будут прочитаны.
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, которые имеют значение в свойстве **ItemIndex** , не равно размер элемента. 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a>Реляционные тестирования фильтра

Реляционные тестирования фильтры позволяют выполнять поиск всех элементов, для которых значение в указанное свойство, которое соответствует любому из больше, чем (\>), больше или равно (\>=), меньше, чем (\<), или меньше или равно (\<=) заданным значением. Значение для сравнения с может быть константа или значение другого свойства для каждого элемента.
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a>Реляционные тестирования фильтра в управляемый API веб-служб Exchange

Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтров поиска для возвращения всех элементов со значением в свойства **ItemIndex** с указанного отношения константное значение 3. 
  
```cs
// Find all items where the custom property value is > 3.
SearchFilter.IsGreaterThan greaterThanFilter =
    new SearchFilter.IsGreaterThan(customPropDefinition, 3);
// Find all items where the custom property value is >= 3.
SearchFilter.IsGreaterThanOrEqualTo greaterThanOrEqualFilter =
    new SearchFilter.IsGreaterThanOrEqualTo(customPropDefinition, ItemSchema.Size);
// Find all items where the custom property value is < 3.
SearchFilter.IsLessThan lessThanFilter =
    new SearchFilter.IsLessThan(customPropDefinition, 3);
// Find all items where the custom property value is <= 3.
SearchFilter.IsLessThanOrEqualTo lessThanOrEqualFilter =
    new SearchFilter.IsLessThanOrEqualTo(customPropDefinition, 3);
```

#### <a name="relational-testing-filter-in-ews"></a>Реляционные тестирования фильтра в веб-служб Exchange

Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска для возвращения всех элементов со значением в свойство **ItemIndex** , больше, чем константное значение 3. 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в **ItemIndex** свойства, которое больше или равно постоянным значением 3. 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в свойство **ItemIndex** , меньше, чем константное значение 3. 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов со значением в свойство **ItemIndex** , меньше или равно постоянным значением 3. 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a>Операция над значением фильтра

Фильтр negating позволяет сведет другого фильтра и положительно результатов поиска. В то время как другие фильтры возврата результатов, соответствующих определенным условиям, negating фильтр возвращает результаты, которые не соответствуют условиям, указанным фильтр, который применяется к.
  
#### <a name="negating-filter-in-the-ews-managed-api"></a>Операция над значением фильтра в управляемый API веб-служб Exchange

Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска для возвращения всех элементов, не связанные с подстроки «собрания» в теме сообщения.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a>Операция над значением фильтра в веб-служб Exchange

Следующем примере показано, как создать фильтр поиска для возвращения всех элементов, не связанные с подстроки «собрания» в теме сообщения.
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a>Составные фильтра

Составные фильтра позволяет объединять несколько фильтров для создания более сложного условия поиска. Критерии, можно объединить с помощью логических операторов и и или. Таким образом можно выполнить поиск как «все сообщения из Sadie Daniels, содержащий «собрания» в теме».
  
#### <a name="compound-filter-in-the-ews-managed-api"></a>Составные фильтр в управляемый API веб-служб Exchange

Следующий пример показывает, как использовать управляемый API веб-служб Exchange для создания фильтра поиска, которое возвращает все элементы, отправленные из Sadie Daniels и содержат «собрания» в теме сообщения.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a>Составные фильтра в веб-служб Exchange

Следующем примере показано, как использовать веб-служб Exchange для создания фильтра поиска, которое возвращает все элементы, которые отправляются из Sadie Daniels и содержат «собрания» в теме сообщения.
  
```XML
<t:And>
  <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
  <t:IsEqualTo>
    <t:FieldURI FieldURI="message:Sender" />
    <t:FieldURIOrConstant>
      <t:Constant Value="sadie@fourthcoffee.com" />
    </t:FieldURIOrConstant>
  </t:IsEqualTo>
</t:And>
```

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a>Пример: Поиск элементов с помощью поисковый фильтр и управляемый API веб-служб Exchange
<a name="bk_ExampleEWSMA"> </a>

Фильтры поиска использовать следующие методы управляемый API EWS:
  
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
В следующем примере используется метод **ExchangeService.FindItems** ; Тем не менее же правила и основные понятия применяются ко всем методам. В следующем примере определяется метод с именем **SearchWithFilter** . Принимает объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект [SearchFilter](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) как параметры. В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . Класс **SearchFilter** является базовым классом для всех различных поисковых фильтров. 
  
```cs
using Microsoft.Exchange.WebServices.Data
private static Guid SearchTestGUID = new Guid("{AA3DF801-4FC7-401F-BBC1-7C93D6498C2E}");
private static ExtendedPropertyDefinition customPropDefinition =
        new ExtendedPropertyDefinition(SearchTestGUID, "ItemIndex", MapiPropertyType.Integer);
static void SearchWithFilter(ExchangeService service, WellKnownFolderName folder, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject, 
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead,
                                       customPropDefinition);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        FindItemsResults<Item> results = service.FindItems(folder, filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item.ExtendedProperties.Count > 0 &&
                 item.ExtendedProperties[0].PropertyDefinition == customPropDefinition)
            {
                Console.WriteLine("Search Index: {0}", item.ExtendedProperties[0].Value);
            }
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

Эта функция с любыми поисковых фильтров, показано в примерах в этой статье. В этом примере использует составные фильтр для возврата всех элементов в папке "Входящие" Sadie Daniels с «собрания» в теме сообщения.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, greaterThanFilter);
SearchWithFilter(service, WellKnownFolderName.Inbox, compoundFilter);
```

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a>Пример: Поиск элемента с помощью поисковый фильтр и веб-служб Exchange
<a name="bk_ExampleEWS"> </a>

Фильтры поиска использовать следующие операции EWS:
  
- [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
В следующем примере используется операция **FindItem** ; Тем не менее же правил и концепции применить обе операции. Фильтры поиска содержатся в элементе [ограничения](http://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) запросов SOAP. В этом примере отправляет запрос SOAP, который соответствует поиска, приведенные в предыдущем примере управляемый API веб-служб Exchange. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
          <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:And>
          <t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
            <t:FieldURI FieldURI="item:Subject" />
            <t:Constant Value="meeting notes" />
          </t:Contains>
          <t:IsEqualTo>
            <t:FieldURI FieldURI="message:Sender" />
            <t:FieldURIOrConstant>
              <t:Constant Value="sadie@contoso.com" />
            </t:FieldURIOrConstant>
          </t:IsEqualTo>
        </t:And>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано ответ от сервера, включая результаты поиска.
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="3" TotalItemsInView="3" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>5</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting Notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>6</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
                <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
                  <t:Value>7</t:Value>
                </t:ExtendedProperty>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a>Дальнейшие действия
<a name="bk_ExampleEWS"> </a>

Теперь, когда вы знакомы с использованием поисковых фильтров в обычного поиска, можно перейти к более сложные приемы поиска.
  
- [Выполнение поиска по сгруппированных с помощью веб-служб Exchange в Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Выполнение поиска по выгружаемый с помощью веб-служб Exchange в Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Поиск и веб-службах Exchange](search-and-ews-in-exchange.md)    
- [Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [FindFolder Operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

