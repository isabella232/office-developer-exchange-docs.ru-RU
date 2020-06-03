---
title: Выполнение поиска AQS с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: c136901a-313e-4adf-a223-1d090d16917a
description: Узнайте, как выполнять поиск с помощью строк запросов и AQS в управляемом API EWS или приложении EWS.
localization_priority: Priority
ms.openlocfilehash: 9f611a8d90c6baf0f307897735c6366c82bb63c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455718"
---
# <a name="perform-an-aqs-search-by-using-ews-in-exchange"></a>Выполнение поиска AQS с помощью EWS в Exchange

Узнайте, как выполнять поиск с помощью строк запросов и AQS в управляемом API EWS или приложении EWS.
  
Строки запросов предоставляют альтернативу [фильтрам поиска](how-to-use-search-filters-with-ews-in-exchange.md) для задания условий поиска. Крупнейшим преимуществом для использования строк запросов является то, что не требуется указывать одно свойство для поиска. Можно просто указать значение, и поиск будет применяться ко всем часто используемым полям элементов. Вы также можете уточнить поиск с помощью расширенного синтаксиса запросов (AQS), а не простого значения. Однако строки запросов имеют следующие ограничения, которые необходимо знать перед их добавлением на панель элементов: 
  
- **Ограниченная возможность поиска определенных свойств.** При поиске с простым значением в строке запроса выполняется поиск по всем индексированным свойствам. Вы можете уточнить поиск по определенным свойствам, но свойства, доступные для использования в строке AQS, ограничены. Если свойство, которое вы хотите найти, не является одним из свойств, доступных для AQS, рассмотрите возможность использования фильтра поиска. 
    
- **Не выполняется поиск настраиваемых свойств.** Поиск строки запроса выполняется по индексу, а настраиваемые свойства не включены в этот индекс. Если вам нужно искать настраиваемые свойства, используйте фильтр поиска. 
    
- **Ограниченный элемент управления для поиска по строкам.** Поиск строки запроса всегда игнорирует регистр и всегда выполняет поиск в подстроках. Если вы хотите выполнять поиск с учетом регистра, префикса или точного совпадения, используйте фильтр поиска. 
    
- **Недоступно для папок или папок поиска.** Операции EWS для поиска папок не поддерживаются с помощью строки запроса. Кроме того, папки поиска не поддерживают строки запросов. В обоих случаях фильтр поиска является единственным вариантом. 
    
## <a name="creating-a-query-string"></a>Создание строки запроса
<a name="bk_CreateQueryString"> </a>

Строки запросов в управляемом API EWS и EWS интерпретируются как подмножество синтаксиса AQS. Строки AQS состоят из пар "значения" или "ключевое слово/значение", разделенных двоеточием (:).
  
`keyword:value`

Если значение задано без ключевого слова, выполняется поиск по всем индексированным свойствам. Если ключевое слово связанно со значением, ключевое слово указывает свойство для поиска соответствующего значения.
  
**Таблица 1. Поддерживаемые ключевые слова AQS**

|**Недопустим**|**Тип значения**|**Пример**|
|:-----|:-----|:-----|
|subject  <br/> |String  <br/> |Тема: Project  <br/> |
|body  <br/> |String  <br/> |текст: данные о продажах  <br/> |
|attachment  <br/> |String  <br/> |вложение: отчет  <br/> |
|на  <br/> |String  <br/> |Кому: "Ольга Даниелс"  <br/> |
|from  <br/> |String  <br/> |от: надеюсь  <br/> |
|копия;  <br/> |String  <br/> |CC: "ронние Стургис"  <br/> |
|СК.  <br/> |String  <br/> |СК: МАКК  <br/> |
|participants  <br/> |String  <br/> |Участники: Ольга  <br/> |
|category  <br/> |String  <br/> |Категория: Project  <br/> |
|importance  <br/> |String  <br/> |importance:high  <br/> |
|kind  <br/> |Тип элемента  <br/> |вид: собрания  <br/> |
|sent  <br/> |Дата  <br/> |Отправлено: 12/10/2013  <br/> |
|received  <br/> |Дата  <br/> |получено: вчера  <br/> |
|HasAttachment  <br/> |Логический  <br/> |Имеет вложение: true  <br/> |
|с пометкой  <br/> |Логический  <br/> |с пометкой: истина  <br/> |
|IsRead  <br/> |Логический  <br/> |чтение: false  <br/> |
|size  <br/> |Номер  <br/> |Размер: \> 5000  <br/> |
   
Давайте посмотрим, как работают различные типы значений.
  
### <a name="using-a-string-value-type"></a>Использование типа строковых значений

Типы строковых значений по умолчанию выполняют поиск в виде префикса подстроки без учета регистра. Это означает, что поиск темы: Project соответствует любой из следующих субъектов: 
  
- Заметки к собранию проекта
    
- У вас есть планы проекта?
    
- Проекции продаж за Декабрь
    
Вы можете изменить поиск так, чтобы он затребовал целое слово, а не сопоставленные префиксы, заключив строку в кавычки. Поиск темы: "Project" исключит значение "предпродажные проекции" из списка совпадений. Обратите внимание, что значение по-прежнему не зависит от регистра. 
  
Если вы используете несколько слов в строке запроса, для сравнения необходимо, чтобы оба слова отображались в полях поиска. Например, Поиск темы: план проекта будет соотнесен с любой из следующих субъектов: 
  
- План проекта
    
- У вас есть планы проекта?
    
- Отправьте мне план проекта.
    
- Планирование вех проекта
    
Если вы заключаете несколько слов в кавычки, они рассматриваются как одна фраза. Поиск темы: "план проекта" будет сопоставлен только теме "план проекта" из предыдущего списка. 
  
### <a name="using-an-item-type-value-type"></a>Использование типа значения типа элемента

Вы можете использовать следующие значения типа элементов с ключевым словом **Kind** , чтобы ограничить результаты поиска только определенным типом элемента, например адресами электронной почты или приглашения на собрания: 
  
- contacts    
- docs    
- email    
- faxes    
- Обмен мгновенными сообщениями (соответствует мгновенным сообщениям)    
- journals    
- собрания (соответствуют приглашениям на встречи и собрания);    
- notes    
- posts    
- rssfeeds    
- tasks    
- voicemail
    
### <a name="using-a-date-value-type"></a>Использование типа значения Date

Типы значений даты можно искать несколькими различными способами. Самый простой способ найти определенную дату. При поиске с полученным сообщением: 12/11/2013 возвращает все элементы, полученные на 11 декабря 2013 г. Однако вы также можете использовать менее конкретные особенности. Поиск с полученным: 12/11 возвращает все элементы, полученные на 11 декабря текущего года. 
  
Кроме того, можно использовать названия месяцев. Вы можете выполнять поиск с помощью Received: 11 декабря 2013 или 11 декабря, чтобы получить те же результаты, что и получено: 12/11/2013 и получено: 12/11, соответственно. Вы также можете выполнять поиск с помощью Received: Декабрь для получения всех элементов, полученных в декабре, в текущем году. 
  
Использование названий дней недели также является параметром. Поиск с получением: вторник возвращает все элементы, полученные во вторник текущей недели. 
  
Типы значений даты также поддерживают набор ключевых слов для поиска относительно текущего времени. Поддерживаются следующие ключевые слова:
  
- today  
- tomorrow
- yesterday
- this week    
- На прошлой неделе    
- следующий месяц    
- последний месяц    
- следующий год
    
Типы значений даты также можно сравнивать с операторами отношений, которые больше или меньше или указаны как диапазон с оператором Range **..**. Например, получено: \> 11/30/2013, Отправлено: \> = вчера и получено: 12/1/2013.. сегодня все допустимые строки запросов. 
  
### <a name="using-a-boolean-value-type"></a>Использование типа логического значения

Логические типы значений могут быть "true" или "false". В значениях регистр не учитывается, поэтому для свойства Read: false результаты будут такими же, как для свойства Read: FALSE.
  
### <a name="using-a-number-value-type"></a>Использование типа числового значения

Числовые типы значений могут выполнять поиск в виде точных совпадений, но их также можно искать с помощью операторов отношения, таких как больше или меньше. Например, размер: 10000 будет возвращать только элементы, размер которых равен 10000 байт, но размер: \> = 10000 будет возвращать элементы, размер которых не превышает 10000 байт. Кроме того, можно указать диапазон с помощью оператора диапазона ( **..**). Например, размер: 7000.. 8000 будут возвращать элементы, размер которых составляет от 7000 до 8000. 
  
### <a name="using-logical-operators"></a>Использование логических операторов

Строки запросов поддерживают следующие логические операторы.
  
**Таблица 2. Поддерживаемые логические операторы**

|**Operator**|**Примеры**|
|:-----|:-----|
|И  <br/> |Project и from: "Ольга Даниелс"  <br/> Тема: (проект и план)  <br/> |
|OR  <br/> |Тема: собрание или из: "надеюсь, брутто"  <br/> от:("Ольга Даниелс" или "надеюсь, брутто")  <br/> |
|NOT  <br/> |НЕ из: "ронние Стургис"  <br/> получено: не сегодня  <br/> |
   
Обратите внимание, что с помощью этих операторов можно присоединяться к нескольким критериям или присоединяться к нескольким значениям в одной и той же комбинации ключевых слов и значений. Однако при соединении нескольких значений в одной пары ключевое слово/значение следует использовать круглые скобки для заключения нескольких значений. Сведения о том, почему следует искать с помощью: "Ольга Даниелс" или "надеюсь, брутто". Этот поиск фактически интерпретируется как следующие условия:
  
- Элемент из Ольга Даниелс или
    
- Элемент имеет фразу "надеюсь брутто" в любом из его индексированных свойств.
    
В отличие от:("Ольга Даниелс" или "надеюсь брутто"), интерпретируется как: 
  
- Элемент из Ольга Даниелс или
    
- Элемент от "самый общий"
    
Оператор по умолчанию, если задано несколько критериев, но логический оператор не включен, и. Например, есть вложение: true Subject: Project эквивалентно: вложение: true AND Subject: Project.
  
## <a name="example-find-items-by-using-a-query-string-and-the-ews-managed-api"></a>Пример: Поиск элементов с помощью строки запроса и управляемого API EWS
<a name="bk_ExampleEWSMA"> </a>

В этом примере определен метод под названием **сеарчвискуеристринг** . Он принимает объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , объект [веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и объект **String** , который представляет строку запроса в качестве параметров. В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
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

Этот метод можно использовать для поиска всех элементов с фразой "план проекта" в теме, как показано в этом примере.
  
```cs
string queryString = "subject:\"project plan\"";
SearchWithQueryString(service, WellKnownFolderName.Inbox, queryString);
```

## <a name="example-find-items-by-using-a-query-string-and-ews"></a>Пример: Поиск элементов с помощью строки запроса и EWS
<a name="bk_ExampleEWS"> </a>

В этом примере запрос на SOAP [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) находит все элементы в папке "Входящие", используя фразу "план проекта" в теме. 
  
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

В следующем примере показан ответ от сервера с результатами поиска.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
- [Использование фильтров поиска с EWS в Exchange](how-to-use-search-filters-with-ews-in-exchange.md)    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

