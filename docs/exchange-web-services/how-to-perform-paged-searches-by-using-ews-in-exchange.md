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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456847"
---
# <a name="perform-paged-searches-by-using-ews-in-exchange"></a><span data-ttu-id="30fcc-103">Выполнение постраничного поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="30fcc-103">Perform paged searches by using EWS in Exchange</span></span>

<span data-ttu-id="30fcc-104">Узнайте, как выполнять постраничный Поиск в управляемом API EWS или приложении EWS, предназначенном для Exchange.</span><span class="sxs-lookup"><span data-stu-id="30fcc-104">Find out how to perform paged searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="30fcc-105">Разбиение по страницам — это функция EWS, позволяющая управлять размером результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="30fcc-105">Paging is a feature in EWS that enables you to control the size of the results of a search.</span></span> <span data-ttu-id="30fcc-106">Вместо того чтобы извлекать весь набор результатов в одном ответе EWS, можно получить небольшие наборы в нескольких ответах EWS.</span><span class="sxs-lookup"><span data-stu-id="30fcc-106">Rather than retrieve the entire result set in one EWS response, you can retrieve smaller sets in multiple EWS responses.</span></span> <span data-ttu-id="30fcc-107">Например, рассмотрим пользователя с 10 000 сообщениями электронной почты в своих папках "Входящие".</span><span class="sxs-lookup"><span data-stu-id="30fcc-107">For example, consider a user with 10,000 email messages in their Inbox.</span></span> <span data-ttu-id="30fcc-108">Гипотетическо вы можете получить всю электронную почту 10 000 в одном очень большом ответе, но вы можете попытаться разбить их на более управляемые блоки для повышения пропускной способности или производительности.</span><span class="sxs-lookup"><span data-stu-id="30fcc-108">Hypothetically, you could retrieve all 10,000 emails in one very large response, but you might want to break that up into more manageable chunks for bandwidth or performance reasons.</span></span> <span data-ttu-id="30fcc-109">Подкачка страниц предоставляет вам инструменты.</span><span class="sxs-lookup"><span data-stu-id="30fcc-109">Paging gives you the tools to do just that.</span></span>
  
> [!NOTE]
> <span data-ttu-id="30fcc-110">Несмотря на то, что вы можете получить элементы 10 000 в одном запросе, маловероятно, что это маловероятно из-за регулирования EWS.</span><span class="sxs-lookup"><span data-stu-id="30fcc-110">While you can hypothetically retrieve 10,000 items in one request, in reality, this is unlikely due to EWS throttling.</span></span> <span data-ttu-id="30fcc-111">Чтобы узнать больше, ознакомьтесь со статьей [регулирование службы EWS в Exchange](ews-throttling-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="30fcc-111">To find out more, see [EWS throttling in Exchange](ews-throttling-in-exchange.md).</span></span> 
  
<span data-ttu-id="30fcc-112">**Таблица 1. Параметры разбиения по страницам в управляемом API EWS и EWS**</span><span class="sxs-lookup"><span data-stu-id="30fcc-112">**Table 1. Paging parameters in the EWS Managed API and EWS**</span></span>

|<span data-ttu-id="30fcc-113">**Чтобы настроить или получить...**</span><span class="sxs-lookup"><span data-stu-id="30fcc-113">**To configure or retrieve the…**</span></span>|<span data-ttu-id="30fcc-114">**В управляемом API EWS используйте...**</span><span class="sxs-lookup"><span data-stu-id="30fcc-114">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="30fcc-115">**В EWS используйте...**</span><span class="sxs-lookup"><span data-stu-id="30fcc-115">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="30fcc-116">Максимальное число элементов или папок в отклике</span><span class="sxs-lookup"><span data-stu-id="30fcc-116">Maximum number of items or folders in a response</span></span>  <br/> |<span data-ttu-id="30fcc-117">Параметр **pageSize** для [конструктора Итемвиев](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) или [конструктора FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-117">The **pageSize** parameter to the [ItemView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.itemview%28v=exchg.80%29.aspx) or the [FolderView constructor](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview.folderview%28v=exchg.80%29.aspx)</span></span> <br/> <span data-ttu-id="30fcc-118">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="30fcc-118">Or</span></span>  <br/> <span data-ttu-id="30fcc-119">Свойство [пажедвиев. PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-119">The [PagedView.PageSize](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.pagesize%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-120">Атрибут **максентриесретурнед** элемента [Индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [индекседпажефолдервиев](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-120">The **MaxEntriesReturned** attribute on the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="30fcc-121">Начальная точка в списке элементов или папок</span><span class="sxs-lookup"><span data-stu-id="30fcc-121">Starting point in the list of items or folders</span></span>  <br/> |<span data-ttu-id="30fcc-122">Параметр **оффсетбасепоинт** для конструктора **Итемвиев** или конструктора **FolderView**</span><span class="sxs-lookup"><span data-stu-id="30fcc-122">The **offsetBasePoint** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="30fcc-123">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="30fcc-123">Or</span></span>  <br/> <span data-ttu-id="30fcc-124">Свойство [пажедвиев. оффсетбасепоинт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-124">The [PagedView.OffsetBasePoint](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offsetbasepoint%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-125">Атрибут **басепоинт** элемента **Индекседпажеитемвиев** или элемента **индекседпажефолдервиев**</span><span class="sxs-lookup"><span data-stu-id="30fcc-125">The **BasePoint** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="30fcc-126">Смещение от начальной точки</span><span class="sxs-lookup"><span data-stu-id="30fcc-126">Offset from the starting point</span></span>  <br/> |<span data-ttu-id="30fcc-127">Параметр **offset** для конструктора **Итемвиев** или конструктора **FolderView**</span><span class="sxs-lookup"><span data-stu-id="30fcc-127">The **offset** parameter to the **ItemView** constructor or the **FolderView** constructor</span></span>  <br/> <span data-ttu-id="30fcc-128">ИЛИ</span><span class="sxs-lookup"><span data-stu-id="30fcc-128">Or</span></span>  <br/> <span data-ttu-id="30fcc-129">Свойство [пажедвиев. offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-129">The [PagedView.Offset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.pagedview.offset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-130">Атрибут **offset** элемента **Индекседпажеитемвиев** или элемента **индекседпажефолдервиев**</span><span class="sxs-lookup"><span data-stu-id="30fcc-130">The **Offset** attribute on the **IndexedPageItemView** element or the **IndexedPageFolderView** element</span></span>  <br/> |
|<span data-ttu-id="30fcc-131">Общее количество результатов на сервере</span><span class="sxs-lookup"><span data-stu-id="30fcc-131">Total number of results on the server</span></span>  <br/> |<span data-ttu-id="30fcc-132">Свойство [финдитемсресултс. тоталкаунт](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) или [финдфолдерсресултс. тоталкаунт](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-132">The [FindItemsResults.TotalCount](https://msdn.microsoft.com/library/dd635348%28v=exchg.80%29.aspx) property or the [FindFoldersResults.TotalCount](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.totalcount%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-133">Атрибут **тоталитемсинвиев** элемента [рутфолдер (финдитемреспонсемессаже)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или элемента [рутфолдер (финдфолдерреспонсемессаже)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-133">The **TotalItemsInView** attribute on the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="30fcc-134">Смещение первого элемента или папки, не включенных в текущий ответ</span><span class="sxs-lookup"><span data-stu-id="30fcc-134">Offset of first item or folder not included in current response</span></span>  <br/> |<span data-ttu-id="30fcc-135">Свойство [финдитемсресултс. некстпажеоффсет](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) или [финдфолдерсресултс. некстпажеоффсет](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-135">The [FindItemsResults.NextPageOffset](https://msdn.microsoft.com/library/ee693014%28v=exchg.80%29.aspx) property or the [FindFoldersResults.NextPageOffset](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.nextpageoffset%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-136">Атрибут **индекседпагингоффсет** элемента **рутфолдер**</span><span class="sxs-lookup"><span data-stu-id="30fcc-136">The **IndexedPagingOffset** attribute on the **RootFolder** element</span></span>  <br/> |
|<span data-ttu-id="30fcc-137">Признак включения в ответ последнего элемента или папки в списке</span><span class="sxs-lookup"><span data-stu-id="30fcc-137">Indicator that response includes the last item or folder in the list</span></span>  <br/> |<span data-ttu-id="30fcc-138">Свойство [финдитемсресултс. мореаваилабле](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) или [финдфолдерсресултс. мореаваилабле](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="30fcc-138">The [FindItemsResults.MoreAvailable](https://msdn.microsoft.com/library/dd635477%28v=exchg.80%29.aspx) property or the [FindFoldersResults.MoreAvailable](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults.moreavailable%28v=exchg.80%29.aspx) property</span></span>  <br/> |<span data-ttu-id="30fcc-139">Атрибут **инклудесластитеминранже** элемента **рутфолдер**</span><span class="sxs-lookup"><span data-stu-id="30fcc-139">The **IncludesLastItemInRange** attribute on the **RootFolder** element</span></span>  <br/> |
   
## <a name="how-paging-works"></a><span data-ttu-id="30fcc-140">Как работает разбиение по страницам</span><span class="sxs-lookup"><span data-stu-id="30fcc-140">How paging works</span></span>
<span data-ttu-id="30fcc-141"><a name="bk_HowPagingWorks"> </a></span><span class="sxs-lookup"><span data-stu-id="30fcc-141"><a name="bk_HowPagingWorks"> </a></span></span>

<span data-ttu-id="30fcc-142">Чтобы узнать, как работает разбиение по страницам, удобно визуализировать сообщения в папке в виде объявлений, расположенных рядом друг с другом в поле за пределами дома.</span><span class="sxs-lookup"><span data-stu-id="30fcc-142">To understand how paging works, it's helpful to visualize the messages in a folder as billboards lined up side by side in a field outside your house.</span></span> <span data-ttu-id="30fcc-143">Некоторые из этих объявлений можно увидеть с помощью окна Волшебная.</span><span class="sxs-lookup"><span data-stu-id="30fcc-143">You can see some of these billboards through a magical window.</span></span> <span data-ttu-id="30fcc-144">Вы можете изменить размер окна (чтобы увеличить или уменьшить число объявлений одновременно) и переместить окно (чтобы определить, какие рекламные объявления вы видите).</span><span class="sxs-lookup"><span data-stu-id="30fcc-144">You have the ability to change the size of the window (to see more or fewer billboards at once) and to move the window (to control which billboards you can see).</span></span> <span data-ttu-id="30fcc-145">Эта обработка окна — разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="30fcc-145">This manipulation of the window is paging.</span></span> 
  
<span data-ttu-id="30fcc-146">При отправке запроса на сервер Exchange задается размер окна в зависимости от количества возвращаемых элементов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-146">When you send your request to the Exchange server, you specify the size of your window in terms of how many items to return.</span></span> <span data-ttu-id="30fcc-147">Положение окна задается путем указания отправной точки (либо начала линии, либо конца строки) и смещения от этой начальной точки, выраженного в виде числа элементов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-147">You set the position of the window by specifying a starting point (either the beginning of the line or the end of the line) and an offset from that starting point, expressed in a number of items.</span></span> <span data-ttu-id="30fcc-148">Начало окна — это количество элементов, заданных смещением от начальной точки.</span><span class="sxs-lookup"><span data-stu-id="30fcc-148">The beginning of the window is the number of items specified by the offset from the starting point.</span></span>
  
<span data-ttu-id="30fcc-149">Где разбиение на страницы немного сложнее в ответе сервера, и как ваше приложение может использовать этот ответ для формирования следующего запроса.</span><span class="sxs-lookup"><span data-stu-id="30fcc-149">Where paging gets a bit more interesting is in the server's response, and how your application can use that response to shape its next request.</span></span> <span data-ttu-id="30fcc-150">Сервер предоставляет три части информации, которые можно использовать для определения способа настройки "окна" для следующего запроса:</span><span class="sxs-lookup"><span data-stu-id="30fcc-150">The server gives you three pieces of information that you can use to determine how to configure your "window" for your next request:</span></span> 
  
- <span data-ttu-id="30fcc-151">Содержит ли результаты в ответе последний элемент в общем наборе результатов на сервере.</span><span class="sxs-lookup"><span data-stu-id="30fcc-151">Whether the results in the response include the last item in the overall result set on the server.</span></span>
    
- <span data-ttu-id="30fcc-152">Общее количество элементов в наборе результатов на сервере.</span><span class="sxs-lookup"><span data-stu-id="30fcc-152">The total number of items in the result set on the server.</span></span>
    
- <span data-ttu-id="30fcc-153">Значение, которое должно быть следующим смещением, если вы хотите переместить окно на следующий элемент в наборе результатов, который не включен в текущий ответ.</span><span class="sxs-lookup"><span data-stu-id="30fcc-153">What the next offset value should be, if you want to advance your window to the next item in the result set that isn't included in the current response.</span></span>
    
<span data-ttu-id="30fcc-154">Рассмотрим простой пример.</span><span class="sxs-lookup"><span data-stu-id="30fcc-154">Let's look at a simple example.</span></span> <span data-ttu-id="30fcc-155">Представьте себе папку "Входящие" с 15 сообщениями.</span><span class="sxs-lookup"><span data-stu-id="30fcc-155">Imagine an Inbox with 15 messages in it.</span></span> <span data-ttu-id="30fcc-156">Ваше приложение отправляет исходный запрос на получение не более 10 элементов, начиная с начала списка сообщений (поэтому смещение равно нулю).</span><span class="sxs-lookup"><span data-stu-id="30fcc-156">Your application sends an initial request to retrieve a maximum of 10 items, starting at the beginning of the list of messages (so the offset is zero).</span></span> <span data-ttu-id="30fcc-157">Сервер отвечает первыми 10 сообщениями и указывает, что в ответ не включается последний элемент, в котором всего 15 элементов, а следующее смещение должно быть равно 10.</span><span class="sxs-lookup"><span data-stu-id="30fcc-157">The server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10.</span></span>
  
<span data-ttu-id="30fcc-158">**Рис. 1. Запрос 10 элементов со смещением 0 от начала списка, состоящего из 15 элементов**</span><span class="sxs-lookup"><span data-stu-id="30fcc-158">**Figure 1. Requesting 10 items at offset 0 from the beginning of a list of 15 items**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов с нулевым смещением от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_FirstPage.png)
  
<span data-ttu-id="30fcc-160">Затем приложение повторно отправляет тот же запрос на сервер, только если это смещение теперь равно 10.</span><span class="sxs-lookup"><span data-stu-id="30fcc-160">Your application then resends the same request to the server, with the only change being that the offset is now 10.</span></span> <span data-ttu-id="30fcc-161">Сервер возвращает последние пять элементов и указывает на то, что в ответ включается последний элемент, в котором имеется 15 элементов, а следующее смещение должно быть равно 15 (хотя конечно, вы достигли конца, поэтому не будет следующего смещения).</span><span class="sxs-lookup"><span data-stu-id="30fcc-161">The server returns the last five items, and indicates that the response does include the last item, that there are a total of 15 items, and that the next offset should be 15 (though of course, you've reached the end, so there won't be a next offset.)</span></span>
  
<span data-ttu-id="30fcc-162">**Рис. 2. Запрос 10 элементов со смещением 10 от начала списка, состоящего из 15 элементов**</span><span class="sxs-lookup"><span data-stu-id="30fcc-162">**Figure 2. Requesting 10 items at offset 10 from the beginning of a list of 15 items**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего их 15 элементов.](media/Ex15_PagedSearch_SecondPage.png)
  
## <a name="design-considerations-for-paging"></a><span data-ttu-id="30fcc-164">Рекомендации по проектированию для разбиения по страницам</span><span class="sxs-lookup"><span data-stu-id="30fcc-164">Design considerations for paging</span></span>
<span data-ttu-id="30fcc-165"><a name="bk_DesignConsiderations"> </a></span><span class="sxs-lookup"><span data-stu-id="30fcc-165"><a name="bk_DesignConsiderations"> </a></span></span>

<span data-ttu-id="30fcc-166">Для обеспечения максимально возиспользования разбиения на страницы в приложении необходимо учитывать некоторые соображения.</span><span class="sxs-lookup"><span data-stu-id="30fcc-166">Making the most out of paging in your application does require some consideration.</span></span> <span data-ttu-id="30fcc-167">Например, как крупнее вы сделаете "окно"?</span><span class="sxs-lookup"><span data-stu-id="30fcc-167">For example, how large do you make your "window"?</span></span> <span data-ttu-id="30fcc-168">Что делать, если вы изменяете результаты на сервере во время перемещения "окна"?</span><span class="sxs-lookup"><span data-stu-id="30fcc-168">What do you do if the results on the server change while you're moving your "window"?</span></span>
  
### <a name="determine-the-size-of-your-window"></a><span data-ttu-id="30fcc-169">Определение размера окна</span><span class="sxs-lookup"><span data-stu-id="30fcc-169">Determine the size of your window</span></span>

<span data-ttu-id="30fcc-170">Отсутствует "один-размер — все" — максимальное количество записей, которое должно использовать все приложения.</span><span class="sxs-lookup"><span data-stu-id="30fcc-170">There is no "one-size-fits-all" maximum number of entries that all applications should use.</span></span> <span data-ttu-id="30fcc-171">Определение количества, которое подходит для вашего приложения, зависит от нескольких разных факторов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-171">Determining the number that's right for your application depends on several different factors.</span></span> <span data-ttu-id="30fcc-172">Тем не менее, полезно учитывать следующие рекомендации:</span><span class="sxs-lookup"><span data-stu-id="30fcc-172">However, it's helpful to keep the following guidelines in mind:</span></span>
  
- <span data-ttu-id="30fcc-173">По умолчанию Exchange ограничение максимального числа элементов, которые могут быть возвращены в один запрос, в 1000.</span><span class="sxs-lookup"><span data-stu-id="30fcc-173">By default, Exchange limits the maximum number of items that can be returned in a single request to 1000.</span></span>
    
- <span data-ttu-id="30fcc-174">Задание максимального количества записей для большего числа приводит к уменьшению числа запросов на получение всех элементов с учетом затрат на ожидание отклика.</span><span class="sxs-lookup"><span data-stu-id="30fcc-174">Setting the maximum number of entries to a larger number results in having to send fewer requests to get all items, at the cost of having to wait longer for responses.</span></span>
    
- <span data-ttu-id="30fcc-175">Задание максимального количества записей меньшего числа приводит к более быстрому времени отклика, а также по затратам на отправку запросов на получение всех элементов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-175">Setting the maximum number of entries to a smaller number results in quicker response times, at the cost of having to send more requests to get all items.</span></span>
    
### <a name="handling-changes-to-the-result-set"></a><span data-ttu-id="30fcc-176">Обработка изменений в наборе результатов</span><span class="sxs-lookup"><span data-stu-id="30fcc-176">Handling changes to the result set</span></span>

<span data-ttu-id="30fcc-177">В простом примере, приведенном ранее в этой статье, количество элементов в папке "Входящие" пользователя остается неизменным.</span><span class="sxs-lookup"><span data-stu-id="30fcc-177">In the simple example earlier in this article, the number of items in the user's Inbox remained constant.</span></span> <span data-ttu-id="30fcc-178">Однако в реальности количество элементов в папке "Входящие" может меняться часто.</span><span class="sxs-lookup"><span data-stu-id="30fcc-178">However, in reality, the number of items in an Inbox can change frequently.</span></span> <span data-ttu-id="30fcc-179">Новые сообщения могут поступать и удаляться или перемещаться в любое время.</span><span class="sxs-lookup"><span data-stu-id="30fcc-179">New messages can arrive and items can be deleted or moved at any time.</span></span> <span data-ttu-id="30fcc-180">Но как это влияет на разбиение по страницам?</span><span class="sxs-lookup"><span data-stu-id="30fcc-180">But how does this impact paging?</span></span> <span data-ttu-id="30fcc-181">Рассмотрим сценарий, приведенный в предыдущем примере, чтобы узнать, как это сделать.</span><span class="sxs-lookup"><span data-stu-id="30fcc-181">Let's modify the earlier example scenario to find out.</span></span>
  
<span data-ttu-id="30fcc-182">Мы начнем еще раз с 15 элементами в папке "Входящие" пользователя и отправляя такой же исходный запрос.</span><span class="sxs-lookup"><span data-stu-id="30fcc-182">We'll start again with the 15 items in the user's Inbox, and send the same initial request.</span></span> <span data-ttu-id="30fcc-183">Как и раньше, сервер отвечает первыми 10 сообщениями и указывает, что в ответ не включается последний элемент, в котором всего 15 элементов, а следующее смещение должно быть равно 10, как показано на рисунке 1.</span><span class="sxs-lookup"><span data-stu-id="30fcc-183">As before, the server responds with the first 10 messages, and indicates that the response does not include the last item, that there are a total of 15 items, and that the next offset should be 10, as shown in Figure 1.</span></span>
  
<span data-ttu-id="30fcc-184">Теперь, пока приложение обрабатывает эти 10 элементов, новое сообщение поступает в папку "Входящие" и добавляется в набор результатов на сервере.</span><span class="sxs-lookup"><span data-stu-id="30fcc-184">Now, while your application is processing those 10 items, a new message arrives in the Inbox and is added to the result set on the server.</span></span> <span data-ttu-id="30fcc-185">Приложение повторно отправляет тот же запрос на сервер (только в том случае, если для параметра offset задано значение 10).</span><span class="sxs-lookup"><span data-stu-id="30fcc-185">Your application resends the same request to the server (only with the offset set to 10).</span></span> <span data-ttu-id="30fcc-186">На этот раз сервер получает шесть элементов и указывает, что в результирующем наборе присутствует 16 элементов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-186">This time the server gets back six items, and indicates that there are a total of 16 items in the result set.</span></span>
  
<span data-ttu-id="30fcc-187">На этом шаге вы, возможно, захотите, что это даже проблема.</span><span class="sxs-lookup"><span data-stu-id="30fcc-187">At this point you might be wondering if this is even a problem.</span></span> <span data-ttu-id="30fcc-188">В конце концов, у вас есть 16 элементов, которые отправляются по двум ответам, поэтому, почему бы все Фусс?</span><span class="sxs-lookup"><span data-stu-id="30fcc-188">After all, you got 16 items back over the two responses, so why all the fuss?</span></span> <span data-ttu-id="30fcc-189">Ответ зависит от того, где в списке размещается новый элемент.</span><span class="sxs-lookup"><span data-stu-id="30fcc-189">The answer depends on where in the list the new item is placed.</span></span> <span data-ttu-id="30fcc-190">Если список отсортирован таким образом, что самые старые элементы (по полученным дате и времени) не являются причинами в этом сценарии.</span><span class="sxs-lookup"><span data-stu-id="30fcc-190">If the list is sorted so that the oldest items (by received date/time) are first, there's no cause for concern in this scenario.</span></span> <span data-ttu-id="30fcc-191">Новый элемент будет добавлен в конец списка и будет включен во второй ответ.</span><span class="sxs-lookup"><span data-stu-id="30fcc-191">The new item will be placed at the end of the list, and will be included in the second response.</span></span>
  
<span data-ttu-id="30fcc-192">**Рис. 3. Запрос 10 элементов со смещением 10 от начала списка, сопоставленного 16 элементов, с шестнадцатым элементом в списке, который является новым**</span><span class="sxs-lookup"><span data-stu-id="30fcc-192">**Figure 3. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the 16th item in the list being new**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemEnd.png)
  
<span data-ttu-id="30fcc-194">Если список отсортирован таким образом, чтобы последние элементы были первыми, это другая статья.</span><span class="sxs-lookup"><span data-stu-id="30fcc-194">If the list is sorted so that the newest items are first, it's a different story.</span></span> <span data-ttu-id="30fcc-195">В этом случае первым элементом второго запроса будет последний элемент из предыдущего запроса плюс оставшиеся пять элементов из исходного 15.</span><span class="sxs-lookup"><span data-stu-id="30fcc-195">In this case, the first item in the second request would be the last item from the previous request plus the remaining five items from the original 15.</span></span> <span data-ttu-id="30fcc-196">Чтобы разместить его в терминах мнимого окна Волшебная, вы переместит положение окна на 10, но сами объявления также сдвигаются на 1.</span><span class="sxs-lookup"><span data-stu-id="30fcc-196">To put it in terms of our imaginary magical window, you shifted your window's position by 10, but the billboards themselves also shifted by 1.</span></span>
  
<span data-ttu-id="30fcc-197">**На рисунке 4. Запрос 10 элементов со смещением 10 от начала списка из 16 элементов, где первый элемент в списке является новым**</span><span class="sxs-lookup"><span data-stu-id="30fcc-197">**Figure 4. Requesting 10 items at offset 10 from the beginning of a list of 16 items, with the first item in the list being new**</span></span>

![Диаграмма, на которой показаны результаты запроса 10 элементов со смещением 10 от начала списка, состоящего из 16 элементов, где 16-й элемент добавлен в начало списка.](media/Ex15_PagedSearch_SecondPage_NewItemBeginning.png)
  
<span data-ttu-id="30fcc-199">Одним из способов обнаружения изменений результатов на сервере является использование концепции элемента привязки.</span><span class="sxs-lookup"><span data-stu-id="30fcc-199">One way to detect a change to the results on the server is to use the concept of an anchor item.</span></span> <span data-ttu-id="30fcc-200">Элемент anchor является дополнительным элементом в ответе, который не обрабатывается вместе с остальными результатами, но используется для сравнения со следующим результатом, чтобы проверить, не изменились ли сами элементы.</span><span class="sxs-lookup"><span data-stu-id="30fcc-200">An anchor item is an additional item in your response that is not processed along with the rest of the results, but is used to compare with the next results to see if the items themselves have shifted.</span></span> <span data-ttu-id="30fcc-201">Построение еще раз в нашем простом примере, если в приложении используется "Window" размером 10, вы фактически устанавливаете максимальное количество элементов, возвращаемых в 11.</span><span class="sxs-lookup"><span data-stu-id="30fcc-201">Building again on our simple example, if your application is using a "window" size of 10, you actually set the maximum number of items to return to 11.</span></span> <span data-ttu-id="30fcc-202">Приложение обрабатывает первые 10 элементов в ответе как обычно.</span><span class="sxs-lookup"><span data-stu-id="30fcc-202">Your application processes the first 10 items in the response as usual.</span></span> <span data-ttu-id="30fcc-203">Для последнего элемента вы сохраняете идентификатор элемента в виде привязки, а затем выдается следующий запрос со смещением, равное 10.</span><span class="sxs-lookup"><span data-stu-id="30fcc-203">For the last item, you save the item's identifier as an anchor, then issue the next request with an offset of 10.</span></span> <span data-ttu-id="30fcc-204">Если данные не изменялись, первый элемент во втором ответе должен иметь идентификатор элемента, соответствующий привязке.</span><span class="sxs-lookup"><span data-stu-id="30fcc-204">If the data has not changed, the first item in the second response should have an item identifier that matches the anchor.</span></span> <span data-ttu-id="30fcc-205">Если идентификаторы элементов не совпадают, вы знаете, что эти данные были удалены или вставлены в части списка, над которым вы уже разбирали страницы.</span><span class="sxs-lookup"><span data-stu-id="30fcc-205">If the item identifiers don't match, you know that the data has been removed or inserted in the parts of the list you have already "paged" over.</span></span>
  
<span data-ttu-id="30fcc-206">Даже если вы знаете, что данные изменились, вам по-прежнему нужно решить, как реагировать.</span><span class="sxs-lookup"><span data-stu-id="30fcc-206">Even when you know that the data has changed, you still need to decide how to react.</span></span> <span data-ttu-id="30fcc-207">Для этого вопроса не существует одного и того же ответа на полный размер.</span><span class="sxs-lookup"><span data-stu-id="30fcc-207">There isn't a one-size-fits-all answer for this question either.</span></span> <span data-ttu-id="30fcc-208">Ваши действия будут зависеть от природы приложения и от того, как важно записать все элементы.</span><span class="sxs-lookup"><span data-stu-id="30fcc-208">Your actions will depend on the nature of your application and how critical it is to capture all items.</span></span> <span data-ttu-id="30fcc-209">Вы можете проигнорировать его совсем, перезапустить процесс из начальной или обратной записи и попробовать определить, где произошло изменение.</span><span class="sxs-lookup"><span data-stu-id="30fcc-209">You might ignore it altogether, restart the process from the beginning, or back track and try to detect where the change happened.</span></span>
  
## <a name="example-perform-a-paged-search-by-using-the-ews-managed-api"></a><span data-ttu-id="30fcc-210">Пример: выполнение страничного поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="30fcc-210">Example: Perform a paged search by using the EWS Managed API</span></span>
<span data-ttu-id="30fcc-211"><a name="bk_PagedSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="30fcc-211"><a name="bk_PagedSearchEWSMA"> </a></span></span>

<span data-ttu-id="30fcc-212">Разбиение по страницам поддерживается следующими методами управляемого API EWS:</span><span class="sxs-lookup"><span data-stu-id="30fcc-212">Paging is supported by the following EWS Managed API methods:</span></span>
  
- [<span data-ttu-id="30fcc-213">ExchangeService. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-213">ExchangeService.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-214">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="30fcc-214">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-215">Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-215">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-216">Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-216">Folder.FindFolders</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="30fcc-217">Если вы используете управляемый API EWS, ваше приложение настраивает разбиение по страницам с помощью класса [итемвиев](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) или [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) и получает от сервера сведения, связанные с разбиением по страницам в классе [финдитемсресултс](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) или [финдфолдерсресултс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="30fcc-217">If you are using the EWS Managed API, your application configures paging with the [ItemView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview%28v=exchg.80%29.aspx) or [FolderView](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx) class and receives information from the server regarding paging from the [FindItemsResults](https://msdn.microsoft.com/library/dd635381%28v=exchg.80%29.aspx) or [FindFoldersResults](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.findfoldersresults%28v=exchg.80%29.aspx) class.</span></span> 
  
<span data-ttu-id="30fcc-218">В приведенном ниже примере показано получение всех элементов в папке с помощью постраничного поиска, который возвращает пять элементов в каждом ответе.</span><span class="sxs-lookup"><span data-stu-id="30fcc-218">The following example retrieves all the items in a folder using a paged search that returns five items in each response.</span></span> <span data-ttu-id="30fcc-219">Он также получает дополнительный элемент, который будет служить привязкой для обнаружения изменений результатов на сервере.</span><span class="sxs-lookup"><span data-stu-id="30fcc-219">It also retrieves an additional item to serve as an anchor to detect changes to the results on the server.</span></span> 
  
<span data-ttu-id="30fcc-220">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="30fcc-220">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
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

## <a name="example-perform-a-paged-search-by-using-ews"></a><span data-ttu-id="30fcc-221">Пример: выполнение страничного поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="30fcc-221">Example: Perform a paged search by using EWS</span></span>
<span data-ttu-id="30fcc-222"><a name="bk_PagedSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="30fcc-222"><a name="bk_PagedSearchEWS"> </a></span></span>

<span data-ttu-id="30fcc-223">Разбиение по страницам поддерживается следующими операциями EWS:</span><span class="sxs-lookup"><span data-stu-id="30fcc-223">Paging is supported by the following EWS operations:</span></span>
  
- [<span data-ttu-id="30fcc-224">FindFolder</span><span class="sxs-lookup"><span data-stu-id="30fcc-224">FindFolder</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="30fcc-225">FindItem</span><span class="sxs-lookup"><span data-stu-id="30fcc-225">FindItem</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
<span data-ttu-id="30fcc-226">Если вы используете EWS, ваше приложение настраивает разбиение по страницам с помощью элемента [индекседпажеитемвиев](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) или элемента [индекседпажефолдервиев](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) и получает сведения от сервера, связанные с разбиением по страницам в элементе [Рутфолдер (Финдитемреспонсемессаже)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) или [рутфолдер (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="30fcc-226">If you're using EWS, your application configures paging with the [IndexedPageItemView](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) element or the [IndexedPageFolderView](https://msdn.microsoft.com/library/c6dac232-244b-4db0-9a15-5e01b8aa7a7d%28Office.15%29.aspx) element and receives information from the server regarding paging from the [RootFolder (FindItemResponseMessage)](https://msdn.microsoft.com/library/187e009f-efaa-42a8-8962-329a645213ab%28Office.15%29.aspx) element or the [RootFolder (FindFolderResponseMessage)](https://msdn.microsoft.com/library/5089c815-663f-46be-bc59-aed9ee20f94a%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="30fcc-227">В этом примере запроса **FindItem** отправляется не более шести элементов, начиная со смещением от нуля до начала списка элементов в папке "Входящие" пользователя.</span><span class="sxs-lookup"><span data-stu-id="30fcc-227">In this request example, a **FindItem** request is sent for a maximum of six items, starting at an offset of zero from the beginning of the list of items in the user's Inbox.</span></span> 
  
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

<span data-ttu-id="30fcc-228">Сервер возвращает следующий ответ, который содержит шесть элементов.</span><span class="sxs-lookup"><span data-stu-id="30fcc-228">The server returns the following response, which contains six items.</span></span> <span data-ttu-id="30fcc-229">Ответ также указывает на то, что в результатах на сервере есть восемь элементов и что последний элемент в списке результатов отсутствует в этом ответе.</span><span class="sxs-lookup"><span data-stu-id="30fcc-229">The response also indicates that there are a total of eight items in the results on the server, and that the last item in the results list is not present in this response.</span></span>
  
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

<span data-ttu-id="30fcc-230">В этом примере отправляется тот же запрос, но в этот раз атрибут **offset** изменяется на 5, что указывает на то, что сервер должен возвратить не более шести элементов начиная с 5 по сравнению с начала.</span><span class="sxs-lookup"><span data-stu-id="30fcc-230">In this example, the same request is sent, but this time, the **Offset** attribute is changed to five, which indicates that the server should return at most six items starting at offset five from the beginning.</span></span> 
  
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

<span data-ttu-id="30fcc-231">Сервер отправляет следующий ответ, который содержит три элемента.</span><span class="sxs-lookup"><span data-stu-id="30fcc-231">The server sends the following response, which contains three items.</span></span> <span data-ttu-id="30fcc-232">Ответ также указывает на то, что общее количество элементов в результатах на сервере по-прежнему равно 8, а последний элемент в списке результатов включен в этот ответ.</span><span class="sxs-lookup"><span data-stu-id="30fcc-232">The response also indicates that the total number of items in the results on the server is still eight, and that the last item in the results list is included in this response.</span></span>
  
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

## <a name="see-also"></a><span data-ttu-id="30fcc-233">См. также</span><span class="sxs-lookup"><span data-stu-id="30fcc-233">See also</span></span>


- [<span data-ttu-id="30fcc-234">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="30fcc-234">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)
    
- [<span data-ttu-id="30fcc-235">Метод ExchangeService. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-235">ExchangeService.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-236">Метод ExchangeService. FindItems</span><span class="sxs-lookup"><span data-stu-id="30fcc-236">ExchangeService.FindItems method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-237">Метод Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-237">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-238">Метод Folder. Финдфолдерс</span><span class="sxs-lookup"><span data-stu-id="30fcc-238">Folder.FindFolders method</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="30fcc-239">Операция FindFolder</span><span class="sxs-lookup"><span data-stu-id="30fcc-239">FindFolder operation</span></span>](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)
    
- [<span data-ttu-id="30fcc-240">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="30fcc-240">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    
- [<span data-ttu-id="30fcc-241">EWS регулирование в Exchange</span><span class="sxs-lookup"><span data-stu-id="30fcc-241">EWS throttling in Exchange</span></span>](ews-throttling-in-exchange.md)
    

