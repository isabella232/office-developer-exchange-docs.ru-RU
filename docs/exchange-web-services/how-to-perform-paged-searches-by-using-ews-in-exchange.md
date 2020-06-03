---
title: Выполнение постраничного поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Узнайте, как выполнять постраничный Поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.
localization_priority: Priority
ms.openlocfilehash: 2b608584918c936f62883b8b444d59c05c5952ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456847"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Выполнение постраничного поиска с помощью EWS в Exchange

Узнайте, как выполнять постраничный Поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.
  
Разбиение по страницам — это функция EWS, позволяющая управлять размером результатов поиска. Вместо того чтобы извлекать весь набор результатов в одном ответе EWS, можно получить небольшие наборы в нескольких ответах EWS. Например, рассмотрим пользователя с 10 000 сообщениями электронной почты в своих папках "Входящие". Гипотетическо вы можете получить всю электронную почту 10 000 в одном очень большом ответе, но вы можете попытаться разбить их на более управляемые блоки для повышения пропускной способности или производительности. Подкачка страниц предоставляет вам инструменты.
  
> [!NOTE]
> Несмотря на то, что вы можете получить элементы 10 000 в одном запросе, маловероятно, что это маловероятно из-за регулирования EWS. Чтобы узнать больше, ознакомьтесь со статьей [регулирование службы EWS в Exchange](ews-throttling-in-exchange.md). 
  
**Таблица 1. Параметры разбиения по страницам в управляемом API EWS и EWS**

|**Чтобы настроить или получить...**|**В управляемом API EWS используйте...**|**В EWS используйте...**|
|:-----|:-----|:-----|
|Максимальное число элементов или папок в отклике  <br/> |Параметр **pageSize** для [конструктора Итемвиев](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) или [конструктора FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> ИЛИ  <br/> Свойство [пажедвиев. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |Атрибут **максентриесретурнед** элемента [Индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [индекседпажефолдервиев](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Начальная точка в списке элементов или папок  <br/> |Параметр **оффсетбасепоинт** для конструктора **Итемвиев** или конструктора **FolderView**  <br/> ИЛИ  <br/> Свойство [пажедвиев. оффсетбасепоинт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |Атрибут **басепоинт** элемента **Индекседпажеитемвиев** или элемента **индекседпажефолдервиев**  <br/> |
|Смещение от начальной точки  <br/> |Параметр **offset** для конструктора **Итемвиев** или конструктора **FolderView**  <br/> ИЛИ  <br/> Свойство [пажедвиев. offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |Атрибут **offset** элемента **Индекседпажеитемвиев** или элемента **индекседпажефолдервиев**  <br/> |
|Общее количество результатов на сервере  <br/> |Свойство [финдитемсресултс. тоталкаунт](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) или [финдфолдерсресултс. тоталкаунт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |Атрибут **тоталитемсинвиев** элемента [рутфолдер (финдитемреспонсемессаже)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [рутфолдер (финдфолдерреспонсемессаже)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Смещение первого элемента или папки, не включенных в текущий ответ  <br/> |Свойство [финдитемсресултс. некстпажеоффсет](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) или [финдфолдерсресултс. некстпажеоффсет](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |Атрибут **индекседпагингоффсет** элемента **рутфолдер**  <br/> |
|Признак включения в ответ последнего элемента или папки в списке  <br/> |Свойство [финдитемсресултс. мореаваилабле](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) или [финдфолдерсресултс. мореаваилабле](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |Атрибут **инклудесластитеминранже** элемента **рутфолдер**  <br/> |
   
## <a name="how-paging-works"></a>Как работает разбиение по страницам
<a name="bk_HowPagingWorks"> </a>

Чтобы узнать, как работает разбиение по страницам, удобно визуализировать сообщения в папке в виде объявлений, расположенных рядом друг с другом в поле за пределами дома. Некоторые из этих объявлений можно увидеть с помощью окна Волшебная. Вы можете изменить размер окна (чтобы увеличить или уменьшить число объявлений одновременно) и переместить окно (чтобы определить, какие рекламные объявления вы видите). Эта обработка окна — разбиение на страницы. 
  
При отправке запроса на сервер Exchange задается размер окна в зависимости от количества возвращаемых элементов. Положение окна задается путем указания отправной точки (либо начала линии, либо конца строки) и смещения от этой начальной точки, выраженного в виде числа элементов. Начало окна — это количество элементов, заданных смещением от начальной точки.
  
Где разбиение на страницы немного сложнее в ответе сервера, и как ваше приложение может использовать этот ответ для формирования следующего запроса. Сервер предоставляет три части информации, которые можно использовать для определения способа настройки "окна" для следующего запроса: 
  
- Содержит ли результаты в ответе последний элемент в общем наборе результатов на сервере.
    
- Общее количество элементов в наборе результатов на сервере.
    
- Значение, которое должно быть следующим смещением, если вы хотите переместить окно на следующий элемент в наборе результатов, который не включен в текущий ответ.
    
Рассмотрим простой пример. Представьте себе папку "Входящие" с 15 сообщениями. Ваше приложение отправляет исходный запрос на получение не более 10 элементов, начиная с начала списка сообщений (поэтому смещение равно нулю). Сервер отвечает первыми 10 сообщениями и указывает, что в ответ не включается последний элемент, в котором всего 15 элементов, а следующее смещение должно быть равно 10.
  
**Рис. 1. Запрос 10 элементов со смещением 0 от начала списка, состоящего из 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов с нулевым смещением от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_FirstPage.png)
  
Затем приложение повторно отправляет тот же запрос на сервер, только если это смещение теперь равно 10. Сервер возвращает последние пять элементов и указывает на то, что в ответ включается последний элемент, в котором имеется 15 элементов, а следующее смещение должно быть равно 15 (хотя конечно, вы достигли конца, поэтому не будет следующего смещения).
  
**Рис. 2. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Рекомендации по проектированию для разбиения по страницам
<a name="bk_DesignConsiderations"> </a>

Для обеспечения максимально возиспользования разбиения на страницы в приложении необходимо учитывать некоторые соображения. Например, как крупнее вы сделаете "окно"? Что делать, если вы изменяете результаты на сервере во время перемещения "окна"?
  
### <a name="determine-the-size-of-your-window"></a>Определение размера окна

Отсутствует "один-размер — все" — максимальное количество записей, которое должно использовать все приложения. Определение количества, которое подходит для вашего приложения, зависит от нескольких разных факторов. Тем не менее, полезно учитывать следующие рекомендации:
  
- По умолчанию Exchange ограничение максимального числа элементов, которые могут быть возвращены в один запрос, в 1000.
    
- Задание максимального количества записей для большего числа приводит к уменьшению числа запросов на получение всех элементов с учетом затрат на ожидание отклика.
    
- Задание максимального количества записей меньшего числа приводит к более быстрому времени отклика, а также по затратам на отправку запросов на получение всех элементов.
    
### <a name="handling-changes-to-the-result-set"></a>Обработка изменений в наборе результатов

В простом примере, приведенном ранее в этой статье, количество элементов в папке "Входящие" пользователя остается неизменным. Однако в реальности количество элементов в папке "Входящие" может меняться часто. Новые сообщения могут поступать и удаляться или перемещаться в любое время. Но как это влияет на разбиение по страницам? Рассмотрим сценарий, приведенный в предыдущем примере, чтобы узнать, как это сделать.
  
Мы начнем еще раз с 15 элементами в папке "Входящие" пользователя и отправляя такой же исходный запрос. Как и раньше, сервер отвечает первыми 10 сообщениями и указывает, что в ответ не включается последний элемент, в котором всего 15 элементов, а следующее смещение должно быть равно 10, как показано на рисунке 1.
  
Теперь, пока приложение обрабатывает эти 10 элементов, новое сообщение поступает в папку "Входящие" и добавляется в набор результатов на сервере. Приложение повторно отправляет тот же запрос на сервер (только в том случае, если для параметра offset задано значение 10). На этот раз сервер получает шесть элементов и указывает, что в результирующем наборе присутствует 16 элементов.
  
На этом шаге вы, возможно, захотите, что это даже проблема. В конце концов, у вас есть 16 элементов, которые отправляются по двум ответам, поэтому, почему бы все Фусс? Ответ зависит от того, где в списке размещается новый элемент. Если список отсортирован таким образом, что самые старые элементы (по полученным дате и времени) не являются причинами в этом сценарии. Новый элемент будет добавлен в конец списка и будет включен во второй ответ.
  
**Рис. 3. Запрос 10 элементов со смещением 10 от начала списка, сопоставленного 16 элементов, с шестнадцатым элементом в списке, который является новым**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Если список отсортирован таким образом, чтобы последние элементы были первыми, это другая статья. В этом случае первым элементом второго запроса будет последний элемент из предыдущего запроса плюс оставшиеся пять элементов из исходного 15. Чтобы разместить его в терминах мнимого окна Волшебная, вы переместит положение окна на 10, но сами объявления также сдвигаются на 1.
  
**На рисунке 4. Запрос 10 элементов со смещением 10 от начала списка из 16 элементов, где первый элемент в списке является новым**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Одним из способов обнаружения изменений результатов на сервере является использование концепции элемента привязки. Элемент anchor является дополнительным элементом в ответе, который не обрабатывается вместе с остальными результатами, но используется для сравнения со следующим результатом, чтобы проверить, не изменились ли сами элементы. Построение еще раз в нашем простом примере, если в приложении используется "Window" размером 10, вы фактически устанавливаете максимальное количество элементов, возвращаемых в 11. Приложение обрабатывает первые 10 элементов в ответе как обычно. Для последнего элемента вы сохраняете идентификатор элемента в виде привязки, а затем выдается следующий запрос со смещением, равное 10. Если данные не изменялись, первый элемент во втором ответе должен иметь идентификатор элемента, соответствующий привязке. Если идентификаторы элементов не совпадают, вы знаете, что эти данные были удалены или вставлены в части списка, над которым вы уже разбирали страницы.
  
Даже если вы знаете, что данные изменились, вам по-прежнему нужно решить, как реагировать. Для этого вопроса не существует одного и того же ответа на полный размер. Ваши действия будут зависеть от природы приложения и от того, как важно записать все элементы. Вы можете проигнорировать его совсем, перезапустить процесс из начальной или обратной записи и попробовать определить, где произошло изменение.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Пример: выполнение страничного поиска с помощью управляемого API EWS
<a name="bk_PagedSearchEWSMA"> </a>

Разбиение по страницам поддерживается следующими методами управляемого API EWS:
  
- [ExchangeService. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
Если вы используете управляемый API EWS, ваше приложение настраивает разбиение по страницам с помощью класса [итемвиев](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) или [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) и получает от сервера сведения, связанные с разбиением по страницам в классе [финдитемсресултс](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) или [финдфолдерсресултс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) . 
  
В приведенном ниже примере показано получение всех элементов в папке с помощью постраничного поиска, который возвращает пять элементов в каждом ответе. Он также получает дополнительный элемент, который будет служить привязкой для обнаружения изменений результатов на сервере. 
  
В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx). 
  
```cs
using Microsoft.Exchange.WebServices.Data;
static void PageSearchItems(ExchangeService service, WellKnownFolderName folder)
{
    int pageSize = 5;
    int offset = 0;
    // Request one more item than your actual pageSize.
    // This will be used to detect a change to the result
    // set while paging.
    ItemView view = new ItemView(pageSize + 1, offset);
    view.PropertySet = new PropertySet(ItemSchema.Subject);
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    view.Traversal = ItemTraversal.Shallow;
    bool moreItems = true;
    ItemId anchorId = null;
    while (moreItems)
    {
        try
        {
            FindItemsResults<Item> results = service.FindItems(folder, view);
            moreItems = results.MoreAvailable;
            if (moreItems &amp;&amp; anchorId != null)
            {
                // Check the first result to make sure it matches
                // the last result (anchor) from the previous page.
                // If it doesn't, that means that something was added
                // or deleted since you started the search.
                if (results.Items.First<Item>().Id != anchorId)
                {
                    Console.WriteLine("The collection has changed while paging. Some results may be missed.");
                }
            }
            if (moreItems)
                view.Offset += pageSize;
            anchorId = results.Items.Last<Item>().Id;
            // Because you're including an additional item on the end of your results
            // as an anchor, you don't want to display it.
            // Set the number to loop as the smaller value between
            // the number of items in the collection and the page size.
            int displayCount = results.Items.Count > pageSize ? pageSize : results.Items.Count;
            for (int i = 0; i < displayCount; i++)
            {
                Item item = results.Items[i];
                Console.WriteLine("Subject: {0}", item.Subject);
                Console.WriteLine("Id: {0}\n", item.Id.ToString());
            }
        }
        catch (Exception ex)
        {
            Console.WriteLine("Exception while paging results: {0}", ex.Message);
        }
    }
}
```

## <a name="example-perform-a-paged-search-by-using-ews"></a>Пример: выполнение страничного поиска с помощью EWS
<a name="bk_PagedSearchEWS"> </a>

Разбиение по страницам поддерживается следующими операциями EWS:
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Если вы используете EWS, ваше приложение настраивает разбиение по страницам с помощью элемента [индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [индекседпажефолдервиев](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) и получает сведения от сервера, связанные с разбиением по страницам в элементе [Рутфолдер (Финдитемреспонсемессаже)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или [рутфолдер (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
В этом примере запроса **FindItem** отправляется не более шести элементов, начиная со смещением от нуля до начала списка элементов в папке "Входящие" пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Сервер возвращает следующий ответ, который содержит шесть элементов. Ответ также указывает на то, что в результатах на сервере есть восемь элементов и что последний элемент в списке результатов отсутствует в этом ответе.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="6" TotalItemsInView="8" IncludesLastItemInRange="false">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Query</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Update</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Planning resources</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Timeline</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>For your perusal</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

В этом примере отправляется тот же запрос, но в этот раз атрибут **offset** изменяется на 5, что указывает на то, что сервер должен возвратить не более шести элементов начиная с 5 по сравнению с начала. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Eastern Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="6" Offset="5" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отправляет следующий ответ, который содержит три элемента. Ответ также указывает на то, что общее количество элементов в результатах на сервере по-прежнему равно 8, а последний элемент в списке результатов включен в этот ответ.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
          <m:RootFolder IndexedPagingOffset="8" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>Meeting notes</t:Subject>
              </t:Message>
              <t:Message>
                <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                <t:Subject>This cat is hilarious!</t:Subject>
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
    
- [Метод ExchangeService. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Метод ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Метод Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Метод Folder. Финдфолдерс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Операция FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    

