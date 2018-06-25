---
title: Выполнение поиска по выгружаемый с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Узнайте, как выполнять выгружаемый поисков в управляемый API EWS или приложение веб-служб Exchange, предназначенное для Exchange.
ms.openlocfilehash: 3f82f46d0582b0b7ff8be63de8a7054b5f3cacab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761096"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Выполнение поиска по выгружаемый с помощью веб-служб Exchange в Exchange

Узнайте, как выполнять выгружаемый поисков в управляемый API EWS или приложение веб-служб Exchange, предназначенное для Exchange.
  
Разбиение на страницы — это функция в веб-служб Exchange, которая позволяет контролировать размер результатов поиска. А не получить весь результирующий набор в один ответа веб-служб Exchange, вы можете получить меньшего размера в несколько ответов веб-служб Exchange. Например рассмотрим пользователя с 10 000 сообщений электронной почты в своей папки "Входящие". Гипотетически можно извлечь все 10 000 сообщения электронной почты в один большой ответ, но может потребоваться, разбить на более управляемые фрагменты для повышения производительности и пропускной способности. Разбиение на страницы предоставляет средства делать это.
  
> [!NOTE]
> Во время гипотетически можно получить 10 000 элементов в один запрос на самом деле, вероятнее всего, не из-за регулирование веб-служб Exchange. Чтобы узнать, обратитесь к разделу [регулирование веб-служб Exchange в Exchange](ews-throttling-in-exchange.md). 
  
**В таблице 1. Параметры разбивки по страницам в управляемый API EWS и веб-служб Exchange**

|**Порядок настройки или получить...**|**В управляемый API веб-служб Exchange используйте...**|**В веб-служб Exchange используйте...**|
|:-----|:-----|:-----|
|Максимальное количество элементов или папок в ответ  <br/> |Параметр **pageSize** [Конструктор ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) или [FolderView конструктор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Или  <br/> Свойство [PagedView.PageSize](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |Атрибут **MaxEntriesReturned** на элемент [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемент [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Отправная точка в список элементов и папок  <br/> |Параметр **offsetBasePoint** конструктор **ItemView** или конструктор **FolderView**  <br/> Или  <br/> Свойство [PagedView.OffsetBasePoint](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |Атрибут **Базисная точка** на элемент **IndexedPageItemView** или элемент **IndexedPageFolderView**  <br/> |
|Смещение от начальной точки  <br/> |Значение параметра **offset** конструктор **ItemView** или конструктор **FolderView**  <br/> Или  <br/> Свойство [PagedView.Offset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |Атрибут **смещение** на элемент **IndexedPageItemView** или элемент **IndexedPageFolderView**  <br/> |
|Общее число результатов на сервере  <br/> |Свойство [FindItemsResults.TotalCount](http://msdn.microsoft.com/en-us/library/dd635348%28v=exchg.80%29.aspx) или [FindFoldersResults.TotalCount](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |Атрибут **TotalItemsInView** на элемент [RootFolder (FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемент [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Смещение первого элемента или папки, не включенные в текущий ответ  <br/> |Свойство [FindItemsResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/ee693014%28v=exchg.80%29.aspx) или [FindFoldersResults.NextPageOffset](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |Атрибут **IndexedPagingOffset** на элемент **RootFolder**  <br/> |
|Индикатор ответа включает последнего элемента или папки в список  <br/> |Свойство [FindItemsResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/dd635477%28v=exchg.80%29.aspx) или [FindFoldersResults.MoreAvailable](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |Атрибут **IncludesLastItemInRange** на элемент **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Как работает разбиение на страницы
<a name="bk_HowPagingWorks"> </a>

Чтобы понять, как работает разбиение на страницы, будет полезно представить сообщений в папке как реклама на стендах разместить рядом друг с другом в поле за пределами дома. Вы можете увидеть некоторые из этих Реклама на стендах через магического окно. У вас есть возможность изменять размер окна (для одновременного просмотра большего или меньшего числа Реклама на стендах) и переместить окно (для управления какой Реклама на стендах, могут видеть). В этом манипуляции окна подкачки. 
  
При отправке запроса на сервере Exchange, укажите размер окна с точки зрения количества элементов для возврата. Задать позицию окна, путем указания начальной точки либо (начало строки) или в конце строки и смещение из этого отправной точки, выраженная в количестве элементов. В начало окна — это число элементов, указанных с учетом смещения от начальной точки.
  
Где разбиение на страницы получает несколько интересных — в ответ сервера, а также как приложения могут использовать этот ответ для фигуры его следующего запроса. Сервер предоставляет три свойства, которые можно использовать для определения способа настройки «окна» для следующего запроса: 
  
- Ли результаты в ответе содержат последнего элемента в общей результирующий набор на сервере.
    
- Общее число элементов в результирующем наборе на сервере.
    
- Что далее значение смещения следует, чтобы перейти к следующему элементу в наборе результатов, не включенные в текущий ответ окна.
    
Рассмотрим простой пример. Например, вы можете с 15 сообщений в его папки «Входящие». Приложение отправляет начального запроса для извлечения не более 10 элементов, начиная с начала списка сообщений (чтобы смещение равно нулю). Сервер отвечает кодом первые 10 сообщений и указывает, что ответ не включает последнего элемента, что всего их 15 элементов, и что следующего смещения должна быть 10.
  
**На рисунке 1. Запроса 10 элементов с нулевым смещением от начала списка 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов с нулевым смещением от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_FirstPage.png)
  
Затем приложение выполняется повторная отправка же запрос к серверу при изменении только, что смещение теперь — 10. Сервер возвращает последние пять элементов и указывает, что ответ включают последнего элемента, что всего их 15 элементов, и что следующего смещения должен быть 15 (хотя Конечно, вы достигнут конец, поэтому не может быть следующего смещения.)
  
**На рисунке 2. Запроса 10 элементов с нулевым смещением от начала списка 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Рекомендации по проектированию для разбивки по страницам
<a name="bk_DesignConsiderations"> </a>

Максимально эффективно разбиение на страницы в приложении требуются некоторые внимание. Например ограничениями на максимальный размер необходимо сделать «окна»? Что делать, если изменить результаты на сервере при перемещении «окна»?
  
### <a name="determine-the-size-of-your-window"></a>Определите размер окна

Нет нет «универсальная» максимальное число элементов, которые следует использовать все приложения. Определение числа, необходимой для приложения зависит от нескольких различных факторов. Тем не менее будет полезно необходимо помнить следующее:
  
- По умолчанию Exchange ограничивает максимальное число элементов, которые могут быть возвращены в одном запросе до 1000.
    
- Установка максимальное число записей для большего число результатов в без отправки меньшее число запросов, чтобы получить все элементы, за счет того, чтобы больше ожидать ответа.
    
- Установка максимальное число записей меньшее число результатов для ускорения времени отклика, но при этом необходимости отправки нескольких запросов для получения всех элементов.
    
### <a name="handling-changes-to-the-result-set"></a>Обработка изменений в наборе результатов

В простой пример ранее в этой статье количество элементов в папке "Входящие" пользователя оставались константу. Тем не менее на самом деле, количество элементов в папке "Входящие" можно изменить часто. Новые сообщения могут поступать и элементов можно удалить или переместить в любое время. Но как листание воздействия? Изменим более ранних пример сценария можно найти сведения.
  
Мы будем еще раз запустите с 15 элементов в папке "Входящие" пользователя и отправить же начального запроса. Как до, сервер отвечает кодом первые 10 сообщений и указывает, что ответ не включает последнего элемента, что всего их 15 элементов, и что следующего смещения должна быть 10, как показано на рисунке 1.
  
Теперь во время приложения эти 10 элементов, новое сообщение поступает в папке "Входящие" и добавляется в результирующем наборе на сервере. Приложение выполняется повторная отправка одного запроса к серверу (только со смещением, равным 10). Данный момент сервер получает обратно шесть элементов и означает, что всего 16 элементов в наборе результатов.
  
На этом этапе может возникнуть вопрос, если это еще проблем. В конце концов, полученный 16 элементов обратно через две ответы так почему усилиями? Ответ зависит от того, где в списке помещается новый элемент. Если список сортируется таким образом, самые старые элементы (по времени и дате получения) первого, нет не причина для вопросов в этом сценарии. Новый элемент будет помещен в конце списка и будет включено в второй ответ.
  
**На рисунке 3. Запроса 10 элементов с нулевым смещением от начала списка, состоящего из 16 элементов с 16-й элемент в списке, новый**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Если список сортируется таким образом, первый новых элементов, — это различных сценариев. В этом случае первый элемент в второй запрос будет последний элемент из предыдущего запроса, а также оставшиеся пять элементов из исходного 15. Чтобы собрать это с точки зрения мнимой магического окна, вы сдвинуто позицию в вашем окне 10, но Реклама на стендах сами также переходят на 1.
  
**На рисунке 4. Запроса 10 элементов с нулевым смещением от начала списка, состоящего из 16 элементов с первый элемент в списке, новый**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Одним из способов для обнаружения изменений в результаты на сервере является использование концепции элемент привязки. Элемент привязки — это дополнительные элемента в ответ, который не обрабатывается наряду с результатов, но используется для сравнения с помощью следующего результатов, чтобы просмотреть, если сами элементы изменились. Построение еще раз в нашем примере, если приложение использует размер «окна» 10, вы фактически задать максимальное число элементов, чтобы вернуться на 11. Приложение обрабатывает первых 10 элементов в ответе как обычно. Для последнего элемента сохранение идентификатор элемента в качестве привязки, затем выполнить следующий запрос со смещением 10. Если данные не был изменен, первый элемент в второй ответ должен иметь идентификатор элемента, которая соответствует привязки. Идентификаторы элементов не совпадают, известно, что данные удалены или вставлен в частях списка, вы уже «разбитым на страницы» через.
  
Даже когда вы знаете, что данные были изменены, по-прежнему необходимо решить, как для выполнения действий. Либо не универсальная ответить на этот вопрос. Действия пользователя будут зависеть от характера приложения и как важна для захвата всех элементов. Может игнорировать полностью, перезапустите процесс с самого начала или резервного отслеживание и пытается определить, где произошло изменение.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Пример: Выполнение выгружаемый поиска с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_PagedSearchEWSMA"> </a>

Разбиение по страницам поддерживается следующими методами управляемый API EWS:
  
- [ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
При использовании управляемого интерфейса API EWS приложения настраивает разбиение на страницы с классом [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) или [FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) и получает данные с сервера в отношении разбиение на страницы из [FindItemsResults](http://msdn.microsoft.com/en-us/library/dd635381%28v=exchg.80%29.aspx) или [FindFoldersResults](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) класс. 
  
В следующем примере извлекается всех элементов в папке с помощью выгружаемый поиска, которое возвращает пять элементов в каждой ответ. Он также получает дополнительные элемента в качестве привязки для обнаружения изменений в результаты на сервере. 
  
В этом примере предполагается, что объект **ExchangeService** была ли инициализирована с допустимые значения для свойства [URL-адреса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) и [учетных данных](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) . 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>Пример: Выполнение выгружаемый поиска с помощью веб-служб Exchange
<a name="bk_PagedSearchEWS"> </a>

Разбиение на страницы поддерживает следующие операции веб-служб Exchange.
  
- [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
Если вы используете веб-служб Exchange, приложения настраивает разбиение на страницы элемент [IndexedPageItemView](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемент [IndexedPageFolderView](http://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) и получает данные с сервера в отношении разбиение на страницы из [RootFolder () FindItemResponseMessage)](http://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемент [RootFolder (FindFolderResponseMessage)](http://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) . 
  
В этом примере запрос отправляется запрос **FindItem** более шести элементов, начиная с смещением нуля в начале списка элементов в папке "Входящие" пользователя. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Сервер возвращает ответ, который содержит шесть элементов. В ответе также указывается, что всего восемь элементов в списке результатов на сервере, и что последнего элемента в списке результатов не указан в этом ответа.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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

В этом примере же запрос будет отправлен, но на этот раз атрибут **смещение** будет изменен до пяти, это означает, что сервер должен возвращать не более шести элементов, начиная с смещения пяти с самого начала. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отправляет ответ, который содержит три элемента. Ответ также указывает, что общее число элементов в списке результатов на сервере, по-прежнему восемь и этого последнего элемента в список включается в этот ответ результаты.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="775" MinorBuildNumber="35" Version="V2_4" 
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
    
- [Метод ExchangeService.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Метод ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Метод Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Метод Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [FindFolder Operation](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem Operation](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [Веб-служб Exchange регулирования в Exchange](ews-throttling-in-exchange.md)
    

