---
title: Выполнение страничного поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 64ed70e4-32eb-4c25-bfc4-43d1477296e5
description: Узнайте, как выполнять страничный поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.
localization_priority: Priority
ms.openlocfilehash: fa36a2ce77150f29e5a62876138c9693a3b4ab1f
ms.sourcegitcommit: 37d4ecd4f469690ba1de87baad2f2f58c40c96ba
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 11/18/2020
ms.locfileid: "49348824"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a>Выполнение страничного поиска с помощью EWS в Exchange

Узнайте, как выполнять страничный поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.
  
Разбиение на страницы — это функция в EWS, которая позволяет управлять размером результатов поиска. Вместо получения всех результатов в одном ответе EWS можно получить меньше результатов в нескольких ответах EWS.  Например, представьте, что в папке "Входящие" пользователя находится 10 000 сообщений электронной почты. Гипотетически можно получать все 10 000 сообщений электронной почты в одном огромном ответе, но можно разбить его на более доступные для управления блоки по соображениям пропускной способности или производительности. Разбиение на страницы дает вам инструменты для этого.
  
> [!NOTE]
> Хотя можно получить 10 000 элементов в одном запросе, в действительности это маловероятно из-за регулирования EWS. Дополнительные сведения см. в разделе [регулирование EWS в Exchange](ews-throttling-in-exchange.md). 
  
**Таблица 1. Параметры разбиения на страницы в управляемом API EWS и EWS**

|**Чтобы настроить или получить...**|**В управляемом API EWS, используйте...**|**В EWS используйте...**|
|:-----|:-----|:-----|
|Максимальное количество элементов или папок в ответе  <br/> |Параметр **pageSize** [конструктора ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) или [конструктора FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx) <br/> Или  <br/> Свойство [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)  <br/> |Атрибут **MaxEntriesReturned** элемента [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)  <br/> |
|Начальная точка в списке элементов или папок  <br/> |Параметр **offsetBasePoint** конструктора **ItemView** или конструктора **FolderView**  <br/> Или  <br/> Свойство [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)  <br/> |Атрибут **BasePoint** элемента **IndexedPageItemView** или элемента **IndexedPageFolderView**  <br/> |
|Смещение от начальной точки  <br/> |Параметр **offset** конструктора **ItemView** или конструктора **FolderView**  <br/> Или  <br/> Свойство [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)  <br/> |Атрибут **Offset** элемента **IndexedPageItemView** элемента **IndexedPageFolderView**  <br/> |
|Общее число результатов на сервере  <br/> |Свойство [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)  <br/> |Атрибут **TotalItemsInView** элемента [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)  <br/> |
|Смещение первого элемента или папки, не включенных в текущий ответ  <br/> |Свойство [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)  <br/> |Атрибут **IndexedPagingOffset** элемента **RootFolder**  <br/> |
|Индикатор того, что ответ включает последний элемент или папку в списке  <br/> |Свойство [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) или свойство [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)  <br/> |Атрибут **IncludesLastItemInRange** элемента **RootFolder**  <br/> |
   
## <a name="how-paging-works"></a>Как работает разбиение на страницы
<a name="bk_HowPagingWorks"> </a>

Чтобы понять, как работает разбиение на страницы, можно визуализировать сообщения в папке, чтобы они отображались в виде рекламных щитов, выстроенных бок о бок в поле за вашим домом. Некоторые из этих рекламных щитов можно увидеть через волшебное окно. У вас есть возможность изменять размер окна (чтобы видеть больше или меньше рекламных щитов одновременно) и перемещать окно (чтобы управлять тем, какие рекламные щиты вы видите). Эта манипуляция с окном и есть разбиение на страницы. 
  
При отправке запроса на сервер Exchange Server необходимо определить размер окна с точки зрения количества элементов, которые необходимо вернуть. Установить положение окна можно задав начальную точку (начало строки или конец строки) и смещение от этой начальной точки, выраженное в количестве элементов. Начало окна — это количество элементов, заданное смещением от начальной точки.
  
Разбиение на страницы более интереснее в ответе сервера и в том, как ваше приложение может использовать этот ответ для формирования следующего запроса. Сервер предоставляет три фрагмента сведений, которые можно использовать, чтобы определить, как настроить ваше «окно» для вашего следующего запроса: 
  
- Включают ли результаты в ответ последний элемент в общие результаты на сервере.
    
- Общее количество элементов в результатах на сервере.
    
- Каким должно быть следующее значение смещения, если вы хотите переместить ваше окно к следующему элементу в результатах, который не включен в текущий ответ.
    
Рассмотрим простой пример. Представьте папку "Входящие" с 15 сообщениями. Приложение отправляет начальный запрос на получение не более 10 элементов, начиная с начала списка сообщений (поэтому смещение равно нулю). Сервер отвечает первыми 10 сообщениями и указывает, что ответ не включает последний элемент, что всего присутствует 15 элементов и что следующее смещение должно быть равно 10.
  
**Рисунок 1. Запрос 10 элементов с нулевым смещением от начала списка, состоящего из 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов с нулевым смещением от начала списка, состоящего из 15 элементов.](media/Ex15_PagedSearch_FirstPage.png)
  
Приложение повторно отправляет тот же запрос на сервер с единственным изменением, заключающимся в том, что теперь смещение равно 10. Сервер возвращает последние пять элементов и указывает, что в ответе содержится последний элемент, что всего присутствует 15 элементов, а следующее смещение должно быть равно 15 (хотя конец достигнут, поэтому следующего смещения не будет.)
  
**Рисунок 2. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a>Анализ дизайна для разбиения на страницы
<a name="bk_DesignConsiderations"> </a>

Чтобы максимально эффективно использовать разбиение на страницы в приложении, необходимо учитывать некоторые вопросы. Например, насколько большим можно сделать "окно"? Что делать, если результаты на сервере меняются при перемещении «окна»?
  
### <a name="determine-the-size-of-your-window"></a>Определение размера окна

Не существует универсального максимального количества записей, которое должны использовать все приложения. Выбор числа, подходящего для вашего приложения, зависит от нескольких факторов. Тем не менее, рекомендуется учитывать следующие моменты:
  
- По умолчанию Exchange ограничивает максимальное количество элементов, которые могут быть возвращены в одном запросе, до 1000.
    
- Установка максимального числа записей на большее количество элементов приводит к необходимости отправлять меньше запросов для получения всех элементов за счет более длительного ожидания ответов.
    
- Установка максимального количества записей на меньшее количество элементов приводит к более быстрому времени отклика за счет необходимости отправлять больше запросов для получения всех элементов.
    
### <a name="handling-changes-to-the-result-set"></a>Обработка изменений в результирующем наборе

В простом примере, приведенном ранее в этой статье, количество элементов в папке «Входящие» пользователя оставалось постоянным. Однако в действительности количество элементов в папке «Входящие» может часто меняться. Новые сообщения могут приходить, а элементы могут быть удалены или перемещены в любое время. Но как это повлияет на разбиение на страницы? Давайте изменим предыдущий примерный сценарий, чтобы выяснить это.
  
Начнем снова с 15 элементов в папке «Входящие» пользователя и отправим тот же начальный запрос. Как и раньше, сервер отвечает первыми 10 сообщениями и указывает, что ответ не включает последний элемент, что всего присутствует 15 элементов и что следующее смещение должно быть равно 10, как показано на рисунке 1.
  
Пока приложение обрабатывает эти 10 элементов, новое сообщение поступает в папку «Входящие» и добавляется в результирующий набор на сервере. Приложение повторно отправляет тот же запрос на сервер (только с установленным смещением 10). На этот раз сервер возвращает шесть элементов и указывает, что всего в результирующем наборе 16 элементов.
  
На этом этапе вам может быть интересно, действительно ли это проблема. В конце концов, вы получили 16 элементов по двум ответам, так в чем проблема? Ответ зависит от того, где в списке размещен новый элемент. Если список отсортирован так, что самые старые элементы (по дате и времени получения) идут первыми, то с этим сценарием все в порядке. Новый элемент будет помещен в конец списка и будет включен во второй ответ.
  
**Рисунок 3. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, при этом 16-й элемент в списке является новым**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
Другое дело, если список отсортирован так, что на первом месте находятся самые новые элементы. В этом случае первый элемент во втором запросе будет последним элементом из предыдущего запроса плюс оставшиеся пять элементов из исходных 15. Выражаясь в терминах нашего воображаемого волшебного окна, вы сместили положение своего окна на 10, но сами рекламные щиты также сдвинулись на 1.
  
**Рисунок 4. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, при этом первый элемент в списке является новым**

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
Один из способов выявления изменения результатов на сервере является использование концепции элемента привязки. Элемент привязки — это дополнительный элемент в ответе, который не обрабатывается вместе с остальными результатами, но используется для сравнения со следующей результатами, чтобы проверить, сместились ли сами элементы. Опять же, основываясь на нашем простом примере, если приложение использует размер «окна» равный 10, вы фактически устанавливаете максимальное количество возвращаемых элементов равным 11. Приложение обрабатывает первые 10 элементов ответа обычным способом. Для последнего элемента вы сохраняете идентификатор элемента в качестве элемента привязки, а затем отправляете следующий запрос со смещением 10. Если данные не изменились, первый элемент во втором ответе должен иметь идентификатор элемента, соответствующий привязке. Если идентификаторы элементов не совпадают, вы знаете, что данные были удалены или вставлены в те части списка, которые вы уже «перелистали».
  
Даже если вы знаете, что данные изменились, вам все равно нужно решить, как реагировать. На этот вопрос также не существует универсального ответа. Ваши действия будут зависеть от характера вашего приложения и от того, насколько важно захватить все элементы. Можно проигнорировать это, перезапустить процесс с самого начала или вернуться назад и попытаться определить, где произошло изменение.
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a>Пример: Выполнение страничного поиска с помощью управляемого API EWS
<a name="bk_PagedSearchEWSMA"> </a>

Разбиение на страницы поддерживается следующими методами управляемого API EWS:
  
- [ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
При использовании управляемого API EWS приложение настраивает разбиение на страницы с помощью класса [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) или [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) и получает с сервера сведения о разбиении на страницы из класса [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) или [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx). 
  
В следующем примере все элементы в папке извлекаются с помощью страничного поиска, который возвращает пять элементов в каждом ответе. Он также извлекает дополнительный элемент, который будет использоваться в качестве привязки для обнаружения изменений результатов на сервере. 
  
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
            if (moreItems && anchorId != null)
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
            int displayCount = 0;
            if ((results.MoreAvailable == false && results.Items.Count > pageSize) || (results.Items.Count < pageSize))
            {
                displayCount = results.Items.Count;
            }
            else
            {
                displayCount = pageSize;
            }
            
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

## <a name="example-perform-a-paged-search-by-using-ews"></a>Пример: Выполнение страничного поиска с помощью EWS
<a name="bk_PagedSearchEWS"> </a>

Разбиение на страницы поддерживается следующими операциями EWS:
  
- [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
При использовании EWS приложение настраивает разбиение на страницы с помощью элемента [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) и получает с сервера сведения о разбиении на страницы из элемента [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx). 
  
В этом примере запроса запрос **FindItem** отправляется максимум для шести элементов, начиная с нулевого смещения от начала списка элементов в папке «Входящие» пользователя. 
  
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

Сервер возвращает следующий ответ, содержащий шесть элементов. Ответ также указывает, что в результатах на сервере содержится всего восемь элементов, а в этом ответе не присутствует последний элемент в списке результатов.
  
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

В этом примере отправляется тот же запрос, но на этот раз атрибут **Offset** изменен на 5, что указывает на то, что сервер должен вернуть не более шести элементов, начиная со смещения, равного пяти от начала. 
  
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

Сервер отправляет следующий ответ, содержащий три элемента. Ответ также указывает, что общее количество элементов в результатах на сервере по-прежнему равно восьми, и что последний элемент в списке результатов включен в этот ответ.
  
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


- [Поиск и EWS в Exchange](search-and-ews-in-exchange.md)
    
- [Метод ExchangeService.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [Метод ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [Метод Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [Метод Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [Операция FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [Операция FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [EWS регулирование в Exchange](ews-throttling-in-exchange.md)
    

