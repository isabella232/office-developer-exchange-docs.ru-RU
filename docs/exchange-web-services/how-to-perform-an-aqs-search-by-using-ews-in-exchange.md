---
title: Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Узнайте, как выполнять поиск с помощью строки запроса и AQS в управляемый API EWS или приложение веб-служб Exchange.
ms.openlocfilehash: dc859e24fa80cd5627477182979c9cc9527818d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761113"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Выполнение поискового запроса AQS с помощью веб-служб Exchange в Exchange

Узнайте, как выполнять поиск с помощью строки запроса и AQS в управляемый API EWS или приложение веб-служб Exchange.
  
Строки запросов представляют альтернативой [поисковых фильтров](how-to-use-search-filters-with-ews-in-exchange.md) для выражения условия поиска. Самое большое преимущество использования строк запросов — это, что не требуется указать отдельное свойство для поиска. Только что можно указывать значение и поиска будут применяться для всех полей часто используемых элементов. Также можно уточнить поиск с помощью расширенный синтаксис запроса (AQS) вместо простого значения. Тем не менее строки запросов имеют следующие ограничения, которые следует обратить внимание перед добавлением к панели инструментов: 
  
- **Ограниченный возможность выполнять поиск в определенных свойств.** При выполнении поиска с помощью простого значения в строку запроса, поиск выполняется по всем индексированные свойства. Можно уточнить поиск для конкретного свойства, но свойства, доступные для использования в строку AQS ограничены. Если свойство, которое вы хотите найти не соответствует ни одному из свойств, доступных для AQS, рекомендуется использовать фильтр поиска. 
    
- **Настраиваемые свойства не поиск.** От индекса выполняется поиск строки запроса и настраиваемых свойств не включаются в этом индексе. Если требуется выполнять поиск настраиваемые свойства, используйте фильтр поиска. 
    
- **Осуществляет поиск только элемент управления для строки.** Поиск строки запроса всегда игнорировать регистр и всегда поиск подстрок. Если вы собираетесь выполнить с учетом регистра, префикс или поиск точного совпадения, используйте фильтр поиска. 
    
- **Недоступно для папки или папки поиска.** Операции веб-служб Exchange для поиска папок не поддерживает использование строки запроса. Кроме того в папках поиска не поддерживают строки запроса. В обоих случаях фильтр поиска является единственно возможный вариант. 
    
## <a name="creating-a-query-string"></a>Создание строки запроса
<a name="bk_CreateQueryString"> </a>

Строки запроса в управляемый API EWS и веб-служб Exchange, интерпретируются как подмножество AQS синтаксис. Строки AQS состоят из значения или пары ключевых слов и значений, разделенных точкой с запятой (:).
  
`keyword:value`

Если значение указано без ключевое слово, все индексированные свойства выполняется поиск значения. Если ключевое слово соединяться со значением, ключевое слово задает свойство для поиска соответствующего значения.
  
**В таблице 1. Поддерживаемые AQS ключевых слов**

|**Ключевое слово**|**Value type**|**Пример**|
|:-----|:-----|:-----|
|subject  <br/> |Строка  <br/> |Тема: проекта  <br/> |
|body  <br/> |Строка  <br/> |графики BODY: продаж  <br/> |
|вложение  <br/> |Строка  <br/> |вложения: отчет  <br/> |
|to  <br/> |Строка  <br/> |Чтобы: «Sadie Daniels»  <br/> |
|from  <br/> |Строка  <br/> |от: надеюсь,  <br/> |
|cc  <br/> |Строка  <br/> |Копия: «Ronnie Sturgis»  <br/> |
|bcc  <br/> |Строка  <br/> |BCC:mack  <br/> |
|participants  <br/> |Строка  <br/> |Участники: sadie  <br/> |
|category  <br/> |String  <br/> |Категория: проект  <br/> |
|importance  <br/> |Строка  <br/> |Важность: высокая  <br/> |
|Тип  <br/> |Тип элемента  <br/> |Тип: собрания  <br/> |
|Отправленные  <br/> |Date  <br/> |отправлено: 12/10/2013  <br/> |
|Получено  <br/> |Date  <br/> |Получено: за вчерашний день  <br/> |
|hasattachment  <br/> |Логический  <br/> |Имеет вложение: true  <br/> |
|помечен флажком|с флажком|с флагом  <br/> |Логический  <br/> |isflagged:true  <br/> |
|isread  <br/> |Логический  <br/> |isread:false  <br/> |
|size  <br/> |Число  <br/> |Размер:\>5000  <br/> |
   
Давайте рассмотрим, как работают разных типов значений.
  
### <a name="using-a-string-value-type"></a>С помощью значение типа string

Типы строковое значение, по умолчанию, как поиск подстрок префикс, которые не учитывают регистр. Который означает, что поиск Тема: проекта будет соответствовать любой из следующие темы: 
  
- Примечания к собранию проекта
    
- У вас есть планов проектов?
    
- Декабрь прогнозов продаж
    
Вы можете изменить поиска, чтобы сделать обязательным наличие слово целиком, а не соответствующего префиксы введите строку в кавычки. Поиск Тема: «project» не будет выполняться значение «Декабря прогнозов продаж» из списка соответствий. Обратите внимание на то, что значение является по-прежнему без учета регистра. 
  
При использовании нескольких слов в строке запроса соответствие требуется, что оба слова отображаются в полях поиска. Например поиск план Тема: проекта будет соответствующих следующие темы: 
  
- План проекта
    
- У вас есть планов проектов?
    
- Отправлять мне план проекта
    
- Планирование вех проекта
    
Если несколько слов заключить в кавычки, они рассматриваются как одной фразы. Поиск Тема: «план проекта» будет соответствовать только темы «План проекта» в предыдущем списке. 
  
### <a name="using-an-item-type-value-type"></a>С помощью тип значение тип элемента

Чтобы ограничить результаты поиска конкретным типом элемента, например, электронной почты или приглашений на собрания можно использовать следующие значения типа элемента с ключевым словом **вида** : 
  
- contacts    
- документы    
- email    
- факсы    
- обмен мгновенными сообщениями (соответствует мгновенных сообщений)    
- журналы.    
- собрания (соответствует встреч и приглашений на собрания)    
- notes    
- posts    
- rssfeeds    
- tasks    
- Голосовая почта
    
### <a name="using-a-date-value-type"></a>С помощью типа значения даты

Можно выполнить поиск типов значений даты в несколько различных способов. Проще всего поиск в конкретный день. Поиск с помощью полученных: 12/11/2013 вернет все элементы, полученного по 11 декабря 2013 г. Тем не менее можно также быть менее конкретным. Поиск с помощью полученных: 12/11 вернет все элементы, полученного по 11 декабря текущего года. 
  
Другая возможность — это использование названия месяца. Можно выполнить поиск с помощью полученных: 11 декабря 2013 г. или 11 декабря для получения тех же результатов, получаемых: 12/11/2013 и полученных: 12/11, соответственно. Можно также выполнить поиск с помощью полученных: Декабрь для получения всех элементов, полученных за месяц декабря в текущем году. 
  
Использование названия дней недели является также параметр. Поиск с помощью полученных: вторник вернет все элементы, полученного по вторник текущей недели. 
  
Типы значения дат также поддерживает набор ключевых слов поиска относительно текущего времени. Поддерживаются следующие ключевые слова:
  
- today  
- tomorrow
- yesterday
- this week    
- На прошлой неделе    
- следующего месяца    
- последний месяц    
- следующий год
    
Типов значений даты также необходимо сравнить с реляционные операторы, такие как больше или меньше, чем, или указанный диапазон с оператором диапазона **.**. Например, полученных:\>11/30/2013 отправлено:\>= за вчерашний день, и received:12/1/2013..today являются все строки допустимый запрос. 
  
### <a name="using-a-boolean-value-type"></a>С помощью типа логическое значение

Типы логическое значение может быть «true» или «false». Значения не учитывают регистр, поэтому isread:false будут создавать те же результаты, что isread:FALSE.
  
### <a name="using-a-number-value-type"></a>С помощью числовой тип значения

Числовой тип значение может быть выполнен как точного совпадения, но они могут также быть поиск с помощью реляционные операторы, такие как больше или меньше чем. Например, размер: 10000 возвращает только элементы, которые имеют размер точно 10000 байт, но размер:\>= 10000 которого возвращаются элементы, которые имеют размер не менее 10000 в байтах. Также можно указать диапазон, используя оператор диапазона ( ****.). Например размер: 7000..8000 возвращает элементов, которые имеют размер от 7000 до 8000. 
  
### <a name="using-logical-operators"></a>С помощью логических операторов

Строки запросов поддерживает следующие логические операторы.
  
**В таблице 2. Поддерживаемые логические операторы**

|**Оператор**|**�������**|
|:-----|:-----|
|AND  <br/> |проект и от: «Sadie Daniels»  <br/> Тема:(project AND plan)  <br/> |
|OR  <br/> |Тема: собрания или из: «Полная надеюсь»  <br/> от: ("Sadie Daniels" или "Надеюсь, полная")  <br/> |
|NOT  <br/> |НЕ от: «Ronnie Sturgis»  <br/> Получено: не сегодня  <br/> |
   
Обратите внимание на то, что можно использовать следующие операторы объединить несколько условий или объединить несколько значений в паре одного ключевое слово/значение. Тем не менее при присоединении к несколько значений в паре одного ключевое слово/значение, следует использовать круглые скобки для обозначения несколько значений. Чтобы понять, почему, рассмотрите возможность поиска в из: «Sadie Daniels» или «Надеюсь валовой». В этом поиска фактически считается следующим критериям:
  
- — Это элемент из Sadie Daniels, OR
    
- Элемент содержит фразу «Полная надеюсь» в индексированные свойства.
    
С другой стороны, из: ("Sadie Daniels" или "Полная надеюсь") обрабатывается как: 
  
- — Это элемент из Sadie Daniels, OR
    
- — Это элемент из надеюсь полная
    
— Это оператор по умолчанию при нескольких условия, но не логический оператор, который включен и. Например имеет вложение: true Тема: project эквивалентен имеет: вложения: true и Тема: проекта.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Пример: Поиск элементов с помощью строки запроса и управляемый API веб-служб Exchange
<a name="bk_ExampleEWSMA"> </a>

В следующем примере определяется метод с именем **SearchWithQueryString** . Требуется объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект **string** , представляющий строки запроса в качестве параметров. В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void SearchWithQueryString(ExchangeService service, WellKnownFolderName folder, string queryString)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       ItemSchema.Size,
                                       ItemSchema.Importance,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Execute the search based on the query string.
        // Example: "subject:project plan"
        FindItemsResults<Item> results = service.FindItems(folder, queryString, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Received: {0}", item.DateTimeReceived.ToString());
            Console.WriteLine("Size: {0}", item.Size.ToString());
            Console.WriteLine("Importance: {0}", item.Importance.ToString());
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

Этот метод можно использовать для поиска всех элементов с фразой «план проекта» в теме сообщения, как показано в следующем примере.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Пример: Поиск элементов с помощью строки запроса и веб-служб Exchange
<a name="bk_ExampleEWS"> </a>

В этом примере запрос SOAP [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) выполняется поиск всех элементов в папке "Входящие" с фразой «план проекта» в теме сообщения. 
  
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
          <t:FieldURI FieldURI="item:Size" />
          <t:FieldURI FieldURI="item:Importance" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
      <m:QueryString>subject:"project plan"</m:QueryString>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

В следующем примере показано ответ от сервера с результатами поиска.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="1" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>project plan</t:Subject>
                <t:DateTimeReceived>2013-12-11T15:42:02Z</t:DateTimeReceived>
                <t:Size>7406</t:Size>
                <t:Importance>Normal</t:Importance>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также

- [Поиск и веб-службах Exchange](search-and-ews-in-exchange.md)    
- [Используйте фильтры поиска с помощью веб-служб Exchange в Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

