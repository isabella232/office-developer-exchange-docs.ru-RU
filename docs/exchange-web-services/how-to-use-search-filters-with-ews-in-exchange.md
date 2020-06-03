---
title: Использование фильтров поиска с EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 20fc6d2d-41c2-4490-98b8-c52513977fef
description: Узнайте, как использовать фильтры поиска с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 04a74ec92d4bced8abd58d164a1c186d6405e679
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455837"
---
# <a name="use-search-filters-with-ews-in-exchange"></a>Использование фильтров поиска с EWS в Exchange

Узнайте, как использовать фильтры поиска с помощью управляемого API EWS или EWS в Exchange.
  
Фильтры поиска — это основное средство для задания критериев поиска в управляемом API EWS или приложении EWS. Рекомендуется использовать фильтры поиска, а не [строки запросов](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md), для выполнения следующих действий:
  
- Поиск по определенному свойству или набору свойств.  
- Поиск с использованием нескольких условий поиска.
    
Фильтры поиска — единственный вариант, если вы выполняете одно из следующих действий:
  
- Поиск настраиваемых свойств.  
- Выполняется поиск строки с учетом регистра.  
- Выполнение поиска по префиксу или точному совпадению строк. 
- Выполнение операций поиска по маске.
- Поиск элементов с определенным набором свойств, независимо от значения.
- Поиск папок.
- Создание папок поиска.
    
## <a name="determine-what-type-of-search-filter-you-need"></a>Определение необходимого типа фильтра поиска
<a name="bk_SelectFilter"> </a>

Прежде чем приступать к созданию фильтра поиска, сначала определите необходимый тип фильтра. Типы фильтров реализуются как классы потомков класса [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS, а также как дочерние элементы элемента [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в EWS. 
  
**Таблица 1. Типы фильтров поиска**

|**Тип фильтра**|**Класс управляемого API EWS**|**Элемент EWS**|**Описание**|
|:-----|:-----|:-----|:-----|
|Содержит фильтр  <br/> |[контаинссубстринг](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) <br/> |[Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) <br/> |Лучший тип фильтра, используемый для сравнений строк. Он позволяет управлять чувствительностью к регистру, независимо от того, следует ли игнорировать пробелы и устанавливать режим включения.  <br/> |
|Фильтр масок  <br/> |[ексклудесбитмаск](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.excludesbitmask%28v=exchg.80%29.aspx) <br/> |[Исключает](https://msdn.microsoft.com/library/bbaeddf6-9a67-4ee0-af99-7a7a5bbdc0e1%28Office.15%29.aspx) <br/> |Позволяет выполнять поиск в целых свойствах в виде битовых масок и возвращать только результаты с битами, соответствующими заданной битовой маске.  <br/> |
|Фильтр EXISTS  <br/> |[Exists](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.exists%28v=exchg.80%29.aspx) <br/> |[Exists](https://msdn.microsoft.com/library/55d568bd-8dbc-4d50-b9d7-54b74a54d4b5%28Office.15%29.aspx) <br/> |Возвращает все элементы, у которых есть указанное свойство, независимо от значения.  <br/> |
|Фильтр равенства  <br/> |[исекуалто](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isequalto%28v=exchg.80%29.aspx) <br/> [иснотекуалто](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isnotequalto%28v=exchg.80%29.aspx) <br/> |[исекуалто](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx) <br/> [иснотекуалто](https://msdn.microsoft.com/library/e2eff26c-3403-45cd-bb74-1eb98c7dbfcd%28Office.15%29.aspx) <br/> |Сравнивает значение указанного свойства с указанным значением константы или значением другого свойства и возвращает все элементы, имеющие значение равно (в случае фильтра **исекуалто** ) или не равное значение (в случае фильтра **иснотекуалто** ).  <br/> |
|Фильтр реляционного тестирования  <br/> |[исгреатерсан](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthan%28v=exchg.80%29.aspx) <br/> [исгреатерсанорекуалто](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.isgreaterthanorequalto%28v=exchg.80%29.aspx) <br/> [ислесссан](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthan%28v=exchg.80%29.aspx) <br/> [ислесссанорекуалто](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.islessthanorequalto%28v=exchg.80%29.aspx) <br/> |[исгреатерсан](https://msdn.microsoft.com/library/a6e9d462-cfa7-40ec-903e-128c95050352%28Office.15%29.aspx) <br/> [исгреатерсанорекуалто](https://msdn.microsoft.com/library/373cc954-314d-40e2-be03-cc08aefc0d5b%28Office.15%29.aspx) <br/> [ислесссан](https://msdn.microsoft.com/library/2550469b-6e5d-45a5-9ecc-090d1b409296%28Office.15%29.aspx) <br/> [ислесссанорекуалто](https://msdn.microsoft.com/library/b5d85eb2-5e15-4d01-ad49-6289e735ad8a%28Office.15%29.aspx) <br/> |Возвращает все элементы, имеющие значение указанного свойства в соответствии с указанным значением константы или с другим свойством. Например, фильтр **исгреатерсан** возвращает все элементы со значением, превышающим указанное значение в указанном свойстве.  <br/> |
|Фильтр отрицания  <br/> |[Not](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.not%28v=exchg.80%29.aspx) <br/> |[Not](https://msdn.microsoft.com/library/1aa16318-7e90-4b19-bce8-dd1a20a66223%28Office.15%29.aspx) <br/> |Инвертирует результат других фильтров.  <br/> |
|Составной фильтр  <br/> |[SearchFilterCollection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) <br/> |[And](https://msdn.microsoft.com/library/790246c2-37ad-49a8-91b9-6186d743b011%28Office.15%29.aspx) <br/> [Or](https://msdn.microsoft.com/library/4876d83a-73a3-4953-9d95-3048e6b76ccb%28Office.15%29.aspx) <br/> |Объединяет несколько фильтров, позволяя использовать более сложные критерии поиска.  <br/> |
   
### <a name="contains-filter"></a>Содержит фильтр

Фильтр содержит является лучшим выбором для поиска свойств строки. С помощью фильтра CONTAINS можно управлять аспектами совпадений строк, например чувствительностью к регистру и продолжением обработки пробела, путем установки режима включения и сравнения.
  
#### <a name="contains-filter-in-the-ews-managed-api"></a>Содержит фильтр в управляемом API EWS
<a name="bk_ContainsEWSMA"> </a>

Если вы используете управляемый API EWS, то задается режим включения с помощью свойства [контаинментмоде](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.containmentmode%28v=exchg.80%29.aspx) класса [контаинссубстринг](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring%28v=exchg.80%29.aspx) , а режим сравнения задается с помощью свойства [компарисонмоде](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter.containssubstring.comparisonmode%28v=exchg.80%29.aspx) класса **контаинссубстринг** . В приведенном ниже примере показано, как создать фильтр поиска, который выполняет поиск в поле subject элементов для подстроки "заметки к собранию". В этом примере игнорируется регистр, но не учитывается пробелы. 
  
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

#### <a name="contains-filter-in-ews"></a>Содержит фильтр в EWS
<a name="bk_ContainsEWSMA"> </a>

В EWS режим включения задается с помощью атрибута **контаинментмоде** в элементе [Contains](https://msdn.microsoft.com/library/476d059d-c243-43e9-b475-319fc413ade2%28Office.15%29.aspx) , а режим сравнения задается с помощью атрибута **контаинменткомпарисон** элемента **Contains** . В приведенном ниже примере показано, как создать фильтр поиска для поиска в поле темы элементов для подстроки "заметки к собранию". В этом примере игнорируется регистр, но не учитывается пробелы. 
  
```XML
<t:Contains ContainmentMode="Substring" ContainmentComparison="IgnoreCase">
  <t:FieldURI FieldURI="item:Subject" />
  <t:Constant Value="meeting notes" />
</t:Contains>
```

### <a name="bitmask-filter"></a>Фильтр масок

Фильтр битовая маска позволяет выполнять поиск в целых свойствах в виде битовых масок и возвращать результаты, в которых определенные биты не задаются в значении указанного свойства.
  
#### <a name="bitmask-filter-in-the-ews-managed-api"></a>Фильтр масок битов в управляемом API EWS

В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все элементы, имеющие значение в настраиваемом свойстве **итеминдекс** (которое определяется в [примере: Поиск элементов с помощью фильтра поиска и раздела УПРАВЛЯЕМого API EWS](#bk_ExampleEWSMA) в этой статье), для которых не задан второй бит (10 в двоичном формате). 
  
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

#### <a name="bitmask-filter-in-ews"></a>Фильтр масок битов в EWS

В приведенном ниже примере показано, как использовать EWS для создания фильтра поиска, чтобы возвратить все элементы, имеющие значение в настраиваемом свойстве **итеминдекс** (которое определяется в [примере: Поиск элементов с помощью фильтра поиска и раздела УПРАВЛЯЕМого API EWS](#bk_ExampleEWSMA) в этой статье), для которых не задан второй бит (10 в двоичном формате). 
  
```XML
<t:Excludes>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:Bitmask Value="2" />
</t:Excludes>
```

### <a name="exists-filter"></a>Фильтр EXISTS

Фильтр Exists позволяет искать элементы, для которых задано определенное свойство, независимо от значения.
  
#### <a name="exists-filter-in-the-ews-managed-api"></a>Фильтр EXISTS в управляемом API EWS

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых есть набор настраиваемых свойств **итеминдекс** . 
  
```cs
// Find all items that have the custom property set.
SearchFilter.Exists customPropSetFilter =
    new SearchFilter.Exists(customPropDefinition);
```

#### <a name="exists-filter-in-ews"></a>Фильтр EXISTS в EWS

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых есть набор настраиваемых свойств **итеминдекс** . 
  
```XML
<t:Exists>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
</t:Exists>
```

### <a name="equality-filter"></a>Фильтр равенства

Фильтры равенства позволяют выполнять поиск всех элементов со значением указанного свойства, которые либо равны определенному значению, либо не равны определенному значению. Значение, с которым выполняется сравнение, может быть постоянным значением или значением другого свойства для каждого элемента.
  
#### <a name="equality-filter-in-the-ews-managed-api"></a>Фильтр равенства в управляемом API EWS

В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все непрочитанные элементы.
  
```cs
// Find all items that are not marked as read.
SearchFilter.IsEqualTo unreadFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false);
```

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , не равным размеру элемента. 
  
```cs
// Find all items that are marked as read.
SearchFilter.IsNotEqualTo indexNotEqualToSizeFilter =
    new SearchFilter.IsNotEqualTo(customPropDefinition, ItemSchema.Size);
```

#### <a name="equality-filter-in-ews"></a>Фильтр равенства в EWS

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех непрочитанных элементов с помощью EWS.
  
```XML
<t:IsEqualTo>
  <t:FieldURI FieldURI="message:IsRead" />
  <t:FieldURIOrConstant>
    <t:Constant Value="false" />
  </t:FieldURIOrConstant>
</t:IsEqualTo>
```

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , не равным размеру элемента. 
  
```XML
<t:IsNotEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:FieldURI FieldURI="item:Size" />
  </t:FieldURIOrConstant>
</t:IsNotEqualTo>
```

### <a name="relational-testing-filter"></a>Фильтр реляционного тестирования

Фильтры реляционных тестов позволяют выполнять поиск всех элементов со значением в указанном свойстве, которое может быть больше ( \> ), больше или равно ( \> =), меньше ( \< ) или меньше или равно ( \< =) заданному значению. Значение, с которым выполняется сравнение, может быть постоянным значением или значением другого свойства для каждого элемента.
  
#### <a name="relational-testing-filter-in-the-ews-managed-api"></a>Фильтр реляционного тестирования в управляемом API EWS

В приведенном ниже примере показано, как с помощью управляемого API EWS создавать фильтры поиска, чтобы возвратить все элементы со значением в свойстве **итеминдекс** с указанным отношением в константное значение 3. 
  
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

#### <a name="relational-testing-filter-in-ews"></a>Фильтр реляционного тестирования в EWS

В приведенном ниже примере показано, как с помощью EWS создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое больше, чем значение константы 3. 
  
```XML
<t:IsGreaterThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThan>
```

В приведенном ниже примере показано, как создать фильтр поиска, чтобы возвратить все элементы со значением в свойстве **итеминдекс** , которое больше или равно значению константы 3. 
  
```XML
<t:IsGreaterThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsGreaterThanOrEqualTo>
```

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое меньше значения константы 3. 
  
```XML
<t:IsLessThan>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThan>
```

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов со значением в свойстве **итеминдекс** , которое меньше или равно константе 3. 
  
```XML
<t:IsLessThanOrEqualTo>
  <t:ExtendedFieldURI PropertySetId="aa3df801-4fc7-401f-bbc1-7c93d6498c2e" PropertyName="ItemIndex" PropertyType="Integer" />
  <t:FieldURIOrConstant>
    <t:Constant Value="3" />
  </t:FieldURIOrConstant>
</t:IsLessThanOrEqualTo>
```

### <a name="negating-filter"></a>Фильтр отрицания

Фильтр отрицания позволяет инвертировать другой фильтр и получить противоположные результаты поиска. Несмотря на то что другие фильтры возвращают результаты, которые удовлетворяют определенным условиям, фильтр отрицания возвращает результаты, которые не отвечают условиям фильтра, к которому он применяется.
  
#### <a name="negating-filter-in-the-ews-managed-api"></a>Фильтр отрицания в управляемом API EWS

В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, чтобы возвратить все элементы, у которых нет подстроки "заметки к собранию" в теме.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
SearchFilter.Not subjectNotFilter =
    new SearchFilter.Not(subjectFilter);
```

#### <a name="negating-filter-in-ews"></a>Фильтр отрицания в EWS

В приведенном ниже примере показано, как создать фильтр поиска для возврата всех элементов, у которых нет подстроки "заметки к собранию" в теме.
  
```XML
<t:Not>
  <t:Contains ContainmentMode="ExactPhrase" ContainmentComparison="IgnoreCase">
    <t:FieldURI FieldURI="item:Subject" />
    <t:Constant Value="meeting notes" />
  </t:Contains>
</t:Not>
```

### <a name="compound-filter"></a>Составной фильтр

Составной фильтр позволяет объединить несколько фильтров для создания более сложных условий поиска. Вы можете комбинировать критерии, используя логические операторы и или. Таким образом, вы можете выполнять поиски, например "все сообщения из Ольга Даниелс, которые содержат" заметки о собраниях "в теме".
  
#### <a name="compound-filter-in-the-ews-managed-api"></a>Составной фильтр в управляемом API EWS

В приведенном ниже примере показано, как использовать управляемый API EWS для создания фильтра поиска, который возвращает все элементы, отправленные из Ольга Даниелс и содержащие "заметки о собраниях" в теме.
  
```cs
SearchFilter.ContainsSubstring subjectFilter = new SearchFilter.ContainsSubstring(ItemSchema.Subject,
    "meeting notes", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
EmailAddress manager = new EmailAddress("sadie@contoso.com");
SearchFilter.IsEqualTo fromManagerFilter =
    new SearchFilter.IsEqualTo(EmailMessageSchema.Sender, manager);
SearchFilter.SearchFilterCollection compoundFilter =
    new SearchFilter.SearchFilterCollection(LogicalOperator.And, subjectFilter, fromManagerFilter);
```

#### <a name="compound-filter-in-ews"></a>Составной фильтр в EWS

В приведенном ниже примере показано, как использовать EWS для создания фильтра поиска, который возвращает все элементы, отправленные из Ольга Даниелс и содержащие "заметки о собраниях" в теме.
  
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

## <a name="example-find-items-by-using-a-search-filter-and-the-ews-managed-api"></a>Пример: Поиск элементов с помощью фильтра поиска и управляемого API EWS
<a name="bk_ExampleEWSMA"> </a>

В следующих методах управляемого API EWS используются фильтры поиска:
  
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
- [ExchangeService. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
- [Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
В следующем примере используется метод **ExchangeService. FindItems** ; Тем не менее, одни и те же правила и концепции применяются ко всем методам. В этом примере определен метод под названием **сеарчвисфилтер** . Он принимает объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [Веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект [SearchFilter](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.searchfilter%28v=exchg.80%29.aspx) в качестве параметров. В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). Класс **SearchFilter** является базовым классом для всех различных фильтров поиска. 
  
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

Эту функцию можно использовать с любыми фильтрами поиска, приведенными в примерах, приведенных в этой статье. В этом примере используется составной фильтр для возврата всех элементов из папки "Входящие" из Ольга Даниелс с "заметками о собраниях" в теме.
  
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

## <a name="example-find-an-item-by-using-a-search-filter-and-ews"></a>Пример: Поиск элемента с помощью фильтра поиска и EWS
<a name="bk_ExampleEWS"> </a>

Следующие операции EWS используют фильтры поиска:
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
В приведенном ниже примере используется операция **FindItem** ; Тем не менее, одни и те же правила и концепции применимы к обеим операциям. Фильтры поиска хранятся в элементе [restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) в запросах SOAP. В этом примере отправляется SOAP-запрос, эквивалентный поиску, который показан в предыдущем примере управляемого API EWS. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

В следующем примере показан ответ от сервера, включая результаты поиска.
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Теперь, когда вы знакомы с использованием фильтров поиска в основных операциях поиска, вы можете перейти на дополнительные приемы расширенного поиска.
  
- [Выполнение группового поиска с помощью EWS в Exchange](how-to-perform-grouped-searches-by-using-ews-in-exchange.md)
    
- [Выполнение постраничного поиска с помощью EWS в Exchange](how-to-perform-paged-searches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>См. также

- [Поиск и веб-службах Exchange](search-and-ews-in-exchange.md)    
- [Выполнение поиска AQS с помощью EWS в Exchange](how-to-perform-an-aqs-search-by-using-ews-in-exchange.md)   
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [ExchangeService. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)    
- [Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)    
- [Folder. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)    
- [Операция FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)   
- [Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

