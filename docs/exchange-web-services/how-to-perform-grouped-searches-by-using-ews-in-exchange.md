---
title: Выполнение группового поиска с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 55de92eb-8e8b-4156-8ad9-dd3828024242
description: Узнайте, как выполнять группировку поисков в управляемом API EWS или приложении EWS, предназначенном для Exchange.
ms.openlocfilehash: 65c6f75ea6b8ab848a263349dcceceead52fa210
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527931"
---
# <a name="perform-grouped-searches-by-using-ews-in-exchange"></a><span data-ttu-id="1ad02-103">Выполнение группового поиска с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ad02-103">Perform grouped searches by using EWS in Exchange</span></span>

<span data-ttu-id="1ad02-104">Узнайте, как выполнять группировку поисков в управляемом API EWS или приложении EWS, предназначенном для Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ad02-104">Find out how to perform grouped searches in your EWS Managed API or EWS application that targets Exchange.</span></span>
  
<span data-ttu-id="1ad02-105">Сгруппированные поиски удобны в том, что они дают вам возможность контролировать организацию результатов поиска.</span><span class="sxs-lookup"><span data-stu-id="1ad02-105">Grouped searches are useful in that they gives you control over how search results are organized.</span></span> <span data-ttu-id="1ad02-106">Упорядоченные результаты поиска могут облегчить приложению обработку результатов или отобразить их конечному пользователю в управляемом виде.</span><span class="sxs-lookup"><span data-stu-id="1ad02-106">Organized search results can make it easier for your application to process results or display them to an end user in a manageable way.</span></span>
  
<span data-ttu-id="1ad02-107">Группирование заключается в размещении всех элементов в наборе результатов с одинаковым значением определенного поля в группе.</span><span class="sxs-lookup"><span data-stu-id="1ad02-107">Grouping works by putting all items within the result set that have the same value of a specific field into a group.</span></span> <span data-ttu-id="1ad02-108">Например, вы можете группировать результаты по отправителю, и все элементы из одного лица будут находиться в отдельной группе, а элементы в каждой группе будут отсортированы в соответствии с порядком, указанным в представлении.</span><span class="sxs-lookup"><span data-stu-id="1ad02-108">For example, you can group your results by the sender, and all items from the same person will be in a separate group, and the items within each group will be sorted according to the order you specify on the view.</span></span> <span data-ttu-id="1ad02-109">Сами группы сортируются по статистическому значению, основанному на выбранном поле.</span><span class="sxs-lookup"><span data-stu-id="1ad02-109">The groups themselves are sorted by an aggregate value based on a field you choose.</span></span>
  
<span data-ttu-id="1ad02-110">**Таблица 1. Методы управляемого API EWS и операции EWS для организации результатов поиска**</span><span class="sxs-lookup"><span data-stu-id="1ad02-110">**Table 1. EWS Managed API methods and EWS operations for organizing search results**</span></span>

|<span data-ttu-id="1ad02-111">**Задача**</span><span class="sxs-lookup"><span data-stu-id="1ad02-111">**If you want to…**</span></span>|<span data-ttu-id="1ad02-112">**В управляемом API EWS используйте...**</span><span class="sxs-lookup"><span data-stu-id="1ad02-112">**In the EWS Managed API, use…**</span></span>|<span data-ttu-id="1ad02-113">**В EWS используйте...**</span><span class="sxs-lookup"><span data-stu-id="1ad02-113">**In EWS, use…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ad02-114">Упорядочение элементов с одинаковым значением в определенном свойстве в результатах по группам</span><span class="sxs-lookup"><span data-stu-id="1ad02-114">Organize items with the same value in a specific property in your results into groups</span></span>  <br/> |[<span data-ttu-id="1ad02-115">Группирование. GroupOn</span><span class="sxs-lookup"><span data-stu-id="1ad02-115">Grouping.GroupOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.groupon%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="1ad02-116">Элемент [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) в качестве дочернего элемента для элемента [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ad02-116">[FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="1ad02-117">Сортировка элементов в каждой группе по значению в определенном свойстве</span><span class="sxs-lookup"><span data-stu-id="1ad02-117">Sort items within each group by the value in a specific property</span></span>  <br/> |[<span data-ttu-id="1ad02-118">Итемвиев. OrderBy</span><span class="sxs-lookup"><span data-stu-id="1ad02-118">ItemView.OrderBy</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="1ad02-119">Элемент [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ad02-119">[SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element</span></span>  <br/> |
|<span data-ttu-id="1ad02-120">Сортировка групп</span><span class="sxs-lookup"><span data-stu-id="1ad02-120">Sort the groups</span></span>  <br/> |[<span data-ttu-id="1ad02-121">GROUPING. Аггрегатеон</span><span class="sxs-lookup"><span data-stu-id="1ad02-121">Grouping.AggregateOn</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="1ad02-122">GROUPING. Аггрегатетипе</span><span class="sxs-lookup"><span data-stu-id="1ad02-122">Grouping.AggregateType</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) <br/><br/> [<span data-ttu-id="1ad02-123">GROUPING. SortDirection</span><span class="sxs-lookup"><span data-stu-id="1ad02-123">Grouping.SortDirection</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="1ad02-124">Элемент **фиелдури** в качестве дочернего элемента для элемента [аггрегатеон](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ad02-124">**FieldURI** element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element</span></span><br/><br/> <span data-ttu-id="1ad02-125">**Статистический** атрибут для элемента **аггрегатеон**</span><span class="sxs-lookup"><span data-stu-id="1ad02-125">**Aggregate** attribute on the **AggregateOn** element</span></span><br/><br/><span data-ttu-id="1ad02-126">Атрибут **Order** для элемента **GroupBy**</span><span class="sxs-lookup"><span data-stu-id="1ad02-126">**Order** attribute on the **GroupBy** element</span></span>  <br/> |
   
<span data-ttu-id="1ad02-127">Давайте попробуем пошаговое выполнение.</span><span class="sxs-lookup"><span data-stu-id="1ad02-127">Let's take it step by step.</span></span>
  
## <a name="group-results-by-a-specific-property"></a><span data-ttu-id="1ad02-128">Группировка результатов по определенному свойству</span><span class="sxs-lookup"><span data-stu-id="1ad02-128">Group results by a specific property</span></span>
<span data-ttu-id="1ad02-129"><a name="bk_GroupResults"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-129"><a name="bk_GroupResults"> </a></span></span>

<span data-ttu-id="1ad02-130">Первый шаг по использованию группирования — выбор свойства или атрибута элементов в хранилище Exchange для группировки по.</span><span class="sxs-lookup"><span data-stu-id="1ad02-130">The first step to using grouping is to select a property, or attribute on the items in the Exchange store, to group by.</span></span> <span data-ttu-id="1ad02-131">Управляемый API EWS предоставляет эти свойства классам в соответствующих классах, а EWS представляет их в виде элементов XML.</span><span class="sxs-lookup"><span data-stu-id="1ad02-131">The EWS Managed API exposes these as class properties on the corresponding classes, while EWS exposes them as XML elements.</span></span> <span data-ttu-id="1ad02-132">Вы можете выбрать любое свойство, включая настраиваемые или расширенные свойства, но при этом полезно знать, как группируются элементы в зависимости от значения свойства, которое вы выбрали.</span><span class="sxs-lookup"><span data-stu-id="1ad02-132">You can choose any property, including custom or extended properties, but it is helpful to understand how items are grouped based on the value of the property you choose.</span></span> 

<span data-ttu-id="1ad02-133">Все элементы, имеющие одинаковое значение в свойстве, выбранном для группировки, будут сгруппированы вместе.</span><span class="sxs-lookup"><span data-stu-id="1ad02-133">All items that have the same value in the property you choose to group by will be grouped together.</span></span> <span data-ttu-id="1ad02-134">Это может показаться очевидным, но это очень важная информация.</span><span class="sxs-lookup"><span data-stu-id="1ad02-134">This might seem obvious, but it is an important detail.</span></span> <span data-ttu-id="1ad02-135">Обратите внимание на то, что происходит при группировке по свойству даты и времени, например [Item. DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или элемент [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) в EWS.</span><span class="sxs-lookup"><span data-stu-id="1ad02-135">Consider what happens if you group by a date/time property, such as [Item.DateTimeReceived](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.datetimereceived%28v=exchg.80%29.aspx) in the EWS Managed API, or the [DateTimeReceived](https://msdn.microsoft.com/library/8f489bd4-2434-4d0a-91fe-1b5ba7eb5765%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="1ad02-136">Цель может быть упорядочена по группам, при этом каждая группа содержит элементы из одного дня.</span><span class="sxs-lookup"><span data-stu-id="1ad02-136">The intent might be to organize the results into groups, with each group containing items from the same day.</span></span> <span data-ttu-id="1ad02-137">Тем не менее, группирование просматривает все значение, которое включает время.</span><span class="sxs-lookup"><span data-stu-id="1ad02-137">However, grouping looks at the entire value, which includes the time.</span></span> 

<span data-ttu-id="1ad02-138">Конечный результат заключается в том, что элементы будут сгруппированы, так что одновременно получаемые элементы перемещаются в свои группы.</span><span class="sxs-lookup"><span data-stu-id="1ad02-138">The end result is that the items will be grouped so that items received at the same time, down to the second, are in their own groups.</span></span> <span data-ttu-id="1ad02-139">Скорее всего, результаты будут отсортированы в большом количестве групп с небольшим количеством элементов в каждой группе.</span><span class="sxs-lookup"><span data-stu-id="1ad02-139">The results will most likely be sorted into a large number of groups with a small number of items in each group.</span></span> 
  
<span data-ttu-id="1ad02-140">Чтобы получить набор результатов с небольшим количеством групп и большим количеством элементов в каждой группе, выберите свойство, которое может иметь меньшее количество значений, например [EmailMessage. from](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) или [Item. Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) в управляемом API EWS или [из](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) [категорий](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) в EWS.</span><span class="sxs-lookup"><span data-stu-id="1ad02-140">To get a results set with a smaller number of groups and a larger number of items in each group, choose a property that is likely to have a smaller number of values, such as [EmailMessage.From](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.from%28v=exchg.80%29.aspx) or [Item.Categories](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.categories%28v=exchg.80%29.aspx) in the EWS Managed API, or [From](https://msdn.microsoft.com/library/5a52d644-3677-4049-874c-12bd5c3080dc%28Office.15%29.aspx) or [Categories](https://msdn.microsoft.com/library/d84d4927-b524-4e62-bf3d-1f12fec8c21a%28Office.15%29.aspx) in EWS.</span></span> <span data-ttu-id="1ad02-141">На следующем рисунке показан список сообщений электронной почты, которые отображаются в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="1ad02-141">The following figure shows a list of emails that appear in an Inbox.</span></span> 
  
<span data-ttu-id="1ad02-142">**Рис. 1. Сообщения в папке "Входящие"**</span><span class="sxs-lookup"><span data-stu-id="1ad02-142">**Figure 1. Messages in an Inbox**</span></span>

![Пример списка сообщений в папке "Входящие".](media/Ex15_GroupedSearch_MsgList.png)
  
<span data-ttu-id="1ad02-144">Если сгруппировать элементы на рис. 1 по свойству **EmailMessage. from** , то результатом будет две группы, одна для сообщений, отправленных с "счастливых брутто", а другой для сообщений, отправляемых Ольга Даниелс.</span><span class="sxs-lookup"><span data-stu-id="1ad02-144">If you group the items in Figure 1 by the **EmailMessage.From** property, the result will be two groups, one for messages sent by Hope Gross, and one for messages sent by Sadie Daniels.</span></span> 
  
<span data-ttu-id="1ad02-145">**Рис. 2. Сообщения, разделенные на группы на основе свойства From**</span><span class="sxs-lookup"><span data-stu-id="1ad02-145">**Figure 2. Messages separated into groups based on the From property**</span></span>

![Изображение, на котором показаны сообщения, рассортированные по двум спискам согласно свойству "От".](media/Ex15_GroupedSearch_SeparateGroups.png)
  
## <a name="sort-the-items-within-groups"></a><span data-ttu-id="1ad02-147">Сортировка элементов в группах</span><span class="sxs-lookup"><span data-stu-id="1ad02-147">Sort the items within groups</span></span>
<span data-ttu-id="1ad02-148"><a name="bk_SortItems"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-148"><a name="bk_SortItems"> </a></span></span>

<span data-ttu-id="1ad02-149">Вы можете управлять сортировкой элементов в каждой группе с помощью свойства [итемвиев. OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или элемента [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) в EWS.</span><span class="sxs-lookup"><span data-stu-id="1ad02-149">You can control how items are sorted within each group by using the [ItemView.OrderBy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemview.orderby%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [SortOrder](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="1ad02-150">Один и тот же порядок применяется к каждой группе.</span><span class="sxs-lookup"><span data-stu-id="1ad02-150">The same ordering applies to each group.</span></span> <span data-ttu-id="1ad02-151">Например, если Вы отсортируете элементы на рис. 1 по свойству **Item. DateTimeReceived** , в убывающем порядке, самый последний полученный из них элемент будет первым в группе вероятнее всего, а последний, полученный из Ольга Даниелс, будет первым в группе Ольга Даниелс.</span><span class="sxs-lookup"><span data-stu-id="1ad02-151">For example, if you sort the items from Figure 1 by the **Item.DateTimeReceived** property, in descending order, the item most recently received from Hope Gross will be first in the Hope Gross group, and the item most recently received from Sadie Daniels will be first in the Sadie Daniels group.</span></span> <span data-ttu-id="1ad02-152">С легкостью, группы на рисунке 2 уже отсортированы таким образом.</span><span class="sxs-lookup"><span data-stu-id="1ad02-152">Conveniently, the groups in Figure 2 are already sorted this way.</span></span> 
  
## <a name="sort-the-groups"></a><span data-ttu-id="1ad02-153">Сортировка групп</span><span class="sxs-lookup"><span data-stu-id="1ad02-153">Sort the groups</span></span>
<span data-ttu-id="1ad02-154"><a name="bk_SortGroups"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-154"><a name="bk_SortGroups"> </a></span></span>

<span data-ttu-id="1ad02-155">Теперь, когда ваши группы сопоставлены, последним шагом будет сортировка самих групп.</span><span class="sxs-lookup"><span data-stu-id="1ad02-155">Now that you have your groups settled, the final step is sorting the groups themselves.</span></span> <span data-ttu-id="1ad02-156">Так как сами группы не имеют определенных значений, процесс группирования должен назначить значение сортировки каждой группе.</span><span class="sxs-lookup"><span data-stu-id="1ad02-156">Because the groups themselves have no specific values, the grouping process has to assign a sort value to each group.</span></span> <span data-ttu-id="1ad02-157">Это выполняется путем объединения значений определенного свойства в каждой группе, заданного свойством [Group. аггрегатеон](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS, или элементом [фиелдури](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) в качестве дочернего элемента для элемента [аггрегатеон](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) в EWS.</span><span class="sxs-lookup"><span data-stu-id="1ad02-157">This is done by aggregation of the values of a specific property within each group, specified by the [Grouping.AggregateOn](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregateon%28v=exchg.80%29.aspx) property in the EWS Managed API, or the [FieldURI](https://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) element as a child of the [AggregateOn](https://msdn.microsoft.com/library/9b0a03f2-3282-46e1-b1a0-cbb9a0fbe9bb%28Office.15%29.aspx) element in EWS.</span></span> <span data-ttu-id="1ad02-158">Свойство [Group. аггрегатетипе](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS (или атрибут **Aggregate** для элемента **аггрегатеон** в EWS) указывает, какое значение из элементов в каждой группе назначается значению сортировки для группы — либо наибольшее значение, либо наименьшее значение.</span><span class="sxs-lookup"><span data-stu-id="1ad02-158">The [Grouping.AggregateType](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.aggregatetype%28v=exchg.80%29.aspx) property in the EWS Managed API (or the **Aggregate** attribute on the **AggregateOn** element in EWS) specifies which value from the items within each group is assigned to the sort value for the group — either the largest value or the smallest value.</span></span> <span data-ttu-id="1ad02-159">Наконец, порядок сортировки (по убыванию или по возрастанию) задается свойством [Group. SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) в УПРАВЛЯЕМОМ API EWS или атрибутом **Order** для элемента [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) в веб-службах EWS.</span><span class="sxs-lookup"><span data-stu-id="1ad02-159">Finally, the sort order (descending or ascending) is specified by the [Grouping.SortDirection](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping.sortdirection%28v=exchg.80%29.aspx) property in the EWS Managed API, or the **Order** attribute on the [GroupBy](https://msdn.microsoft.com/library/9728619b-4674-4b9d-9f6c-e75c6165966c%28Office.15%29.aspx) element in EWS.</span></span> 
  
<span data-ttu-id="1ad02-160">Например, если группы, показанные на рисунке 2, отсортированы по статистической обработке свойства **Item. DateTimeReceived** с наименьшим значением и сортировка по убыванию, элементы возвращаются в порядке, приведенном на рисунке 3.</span><span class="sxs-lookup"><span data-stu-id="1ad02-160">For example, if the groups from Figure 2 are sorted by aggregating on the **Item.DateTimeReceived** property, using the smallest value, and sorting in descending order, the items are returned in the order in shown Figure 3.</span></span> 
  
<span data-ttu-id="1ad02-161">**Рис. 3. Сгруппированные результаты поиска с группами, отсортированными по свойству DateTimeReceived**</span><span class="sxs-lookup"><span data-stu-id="1ad02-161">**Figure 3. Grouped search results with the groups sorted by the DateTimeReceived property**</span></span>

![Изображение, на котором показан отсортированный список сообщений, сгруппированный по свойству "От", где группы отсортированы по наименьшим времени и дате получения.](media/Ex15_GroupedSearch_Results.png)
  
<span data-ttu-id="1ad02-163">В следующих разделах показано, как можно забирать группирование и сортировку в коде.</span><span class="sxs-lookup"><span data-stu-id="1ad02-163">The next sections show you how you might pull grouping and sorting together in code.</span></span>
  
## <a name="example-perform-a-grouped-search-by-using-the-ews-managed-api"></a><span data-ttu-id="1ad02-164">Пример: выполнение группового поиска с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="1ad02-164">Example: Perform a grouped search by using the EWS Managed API</span></span>
<span data-ttu-id="1ad02-165"><a name="bk_GroupSearchEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-165"><a name="bk_GroupSearchEWSMA"> </a></span></span>

<span data-ttu-id="1ad02-166">Следующие методы управляемого API EWS могут использовать группировку:</span><span class="sxs-lookup"><span data-stu-id="1ad02-166">The following EWS Managed API methods can use grouping:</span></span>
  
- [<span data-ttu-id="1ad02-167">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="1ad02-167">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="1ad02-168">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="1ad02-168">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)
    
<span data-ttu-id="1ad02-169">В следующем примере используется метод **ExchangeService. FindItems** ; Тем не менее те же правила и концепции применяются к методу **Folder. FindItems** .</span><span class="sxs-lookup"><span data-stu-id="1ad02-169">The following example uses the **ExchangeService.FindItems** method; however, the same rules and concepts apply to the **Folder.FindItems** method.</span></span> <span data-ttu-id="1ad02-170">В этом примере определен метод под названием **граупитемсбифром** .</span><span class="sxs-lookup"><span data-stu-id="1ad02-170">In this example, a method called **GroupItemsByFrom** is defined.</span></span> <span data-ttu-id="1ad02-171">В качестве параметров в качестве параметров используется объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и объект [веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1ad02-171">It takes an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and a [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) object as parameters.</span></span> <span data-ttu-id="1ad02-172">Он запрашивает первые 50 элементов в папке, сгруппированные по свойству **EmailMessage. from** , отсортированному по свойству **Item. DateTimeReceived** в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="1ad02-172">It requests the first 50 items in the folder, grouped by the **EmailMessage.From** property, sorted by the **Item.DateTimeReceived** property in descending order.</span></span> <span data-ttu-id="1ad02-173">Сами группы сортируются по наименьшему значению свойства **Item. DateTimeReceived** в их элементах в порядке убывания.</span><span class="sxs-lookup"><span data-stu-id="1ad02-173">The groups themselves are sorted by the smallest **Item.DateTimeReceived** property value on their items, in descending order.</span></span> 
  
<span data-ttu-id="1ad02-174">В этом примере предполагается, что для объекта **ExchangeService** выполнена инициализация с допустимыми значениями в свойствах [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) и [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="1ad02-174">This example assumes that the **ExchangeService** object has been initialized with valid values in the [Credentials](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservicebase.credentials%28v=exchg.80%29.aspx) and [Url](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.url%28v=exchg.80%29.aspx) properties.</span></span> 
  
```cs
static void GroupItemsByFrom(ExchangeService service, WellKnownFolderName folder)
{
    // Limit the result set to 50 items.
    ItemView view = new ItemView(50);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.From,
                                       ItemSchema.Categories);
    // Item searches do not support Deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Specify the sorting done within the groups.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    // Configure grouping.
    Grouping groupByFrom = new Grouping();
    groupByFrom.GroupOn = EmailMessageSchema.From;
    groupByFrom.AggregateOn = ItemSchema.DateTimeReceived;
    groupByFrom.AggregateType = AggregateType.Minimum;
    groupByFrom.SortDirection = SortDirection.Descending;
    try
    {
        GroupedFindItemsResults<Item> results = service.FindItems(folder,
            view, groupByFrom);
        foreach (ItemGroup<Item> group in results.ItemGroups)
        {
            Console.WriteLine("Group: {0}", group.GroupIndex);
            foreach (Item item in group.Items)
            {
                if (item is EmailMessage)
                {
                    EmailMessage message = item as EmailMessage;
                    Console.WriteLine("From: {0}", message.From);
                    Console.WriteLine("Subject: {0}", message.Subject);
                    Console.WriteLine("Id: {0}\n", message.Id.ToString());
                }
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

## <a name="example-perform-a-grouped-search-by-using-ews"></a><span data-ttu-id="1ad02-175">Пример: выполнение группового поиска с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="1ad02-175">Example: Perform a grouped search by using EWS</span></span>
<span data-ttu-id="1ad02-176"><a name="bk_GroupSearchEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-176"><a name="bk_GroupSearchEWS"> </a></span></span>

<span data-ttu-id="1ad02-177">В следующем примере запроса показан запрос [операции FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для первых 50 элементов в папке, сгруппированных по элементу **from** и отсортированный по элементу **DateTimeReceived** в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="1ad02-177">The following request example shows a [FindItem operation](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) request for the first 50 items in the folder, grouped by the **From** element, sorted by the **DateTimeReceived** element in descending order.</span></span> <span data-ttu-id="1ad02-178">Сами группы сортируются по наименьшему значению элемента **DateTimeReceived** в их элементах в убывающем порядке.</span><span class="sxs-lookup"><span data-stu-id="1ad02-178">The groups themselves are sorted by the smallest **DateTimeReceived** element value on their items, in descending order.</span></span> 
  
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
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:From" />
          <t:FieldURI FieldURI="item:Categories" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="50" Offset="0" BasePoint="Beginning" />
      <m:GroupBy Order="Descending">
        <t:FieldURI FieldURI="message:From" />
        <t:AggregateOn Aggregate="Minimum">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:AggregateOn>
      </m:GroupBy>
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

<span data-ttu-id="1ad02-179">Сервер возвращает следующий ответ.</span><span class="sxs-lookup"><span data-stu-id="1ad02-179">The server returns the following response.</span></span>
  
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
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="10" TotalItemsInView="8" IncludesLastItemInRange="true">
            <t:Groups>
              <t:GroupedItems>
                <t:GroupIndex>0</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Planning resources</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:41:05Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Timeline</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:40:37Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>For your perusal</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:51:16Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Meeting notes</t:Subject>
                    <t:DateTimeReceived>2013-11-20T21:18:51Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Sadie Daniels</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=8D84A3F4CBB34D48838A3AECF99795C0-SADIE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
              <t:GroupedItems>
                <t:GroupIndex>1</t:GroupIndex>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Query</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:43:15Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>Update</t:Subject>
                    <t:DateTimeReceived>2013-12-10T17:42:33Z</t:DateTimeReceived>
                    <t:Categories>
                      <t:String>Project</t:String>
                      <t:String>Blue category</t:String>
                    </t:Categories>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                  <t:Message>
                    <t:ItemId Id="AAMkAGM2..." ChangeKey="CQAAABYA..." />
                    <t:Subject>This cat is hilarious!</t:Subject>
                    <t:DateTimeReceived>2013-10-15T20:22:12Z</t:DateTimeReceived>
                    <t:From>
                      <t:Mailbox>
                        <t:Name>Hope Gross</t:Name>
                        <t:EmailAddress>/O=FIRST ORGANIZATION/OU=EXCHANGE ADMINISTRATIVE GROUP (FYDIBOHF23SPDLT)/CN=RECIPIENTS/CN=9B55E4100C064D9D8C5F72FF36802ED3-HOPE</t:EmailAddress>
                        <t:RoutingType>EX</t:RoutingType>
                      </t:Mailbox>
                    </t:From>
                  </t:Message>
                </t:Items>
              </t:GroupedItems>
            </t:Groups>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="version-differences"></a><span data-ttu-id="1ad02-180">Различия версий</span><span class="sxs-lookup"><span data-stu-id="1ad02-180">Version differences</span></span>
<span data-ttu-id="1ad02-181"><a name="bk_VersionDiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="1ad02-181"><a name="bk_VersionDiffs"> </a></span></span>

<span data-ttu-id="1ad02-182">Версии Exchange, начиная с основной версии 15 и заканчивая сборкой 15.0.775.38, возвращают элементы **группы** (типа **граупедитемстипе**) вместо элементов [граупедитемс](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) в ответе SOAP.</span><span class="sxs-lookup"><span data-stu-id="1ad02-182">Versions of Exchange starting with major version 15 and ending with build 15.0.775.38 return **Group** elements (of type **GroupedItemsType**) in place of [GroupedItems](https://msdn.microsoft.com/library/53170df4-4272-4b37-b23f-cd8e2d4a7396%28Office.15%29.aspx) elements in the SOAP response.</span></span> <span data-ttu-id="1ad02-183">Если вы используете управляемый API EWS, это приведет к тому, что коллекция [граупедфиндитемсресултс. итемграупс](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) будет содержать 0 объектов.</span><span class="sxs-lookup"><span data-stu-id="1ad02-183">If you are using the EWS Managed API, this will cause the [GroupedFindItemsResults.ItemGroups](https://msdn.microsoft.com/library/office/dd633961%28v=exchg.80%29.aspx) collection to contain 0 objects.</span></span> <span data-ttu-id="1ad02-184">Если вы используете EWS, элементы **Group** должны обрабатываться как элементы **граупедитемс** .</span><span class="sxs-lookup"><span data-stu-id="1ad02-184">If you are using EWS, **Group** elements should be handled as **GroupedItems** elements.</span></span> 
  
<span data-ttu-id="1ad02-185">Версии Exchange, начиная с основной версии 15, возвращают дополнительные элементы **Group** или **граупедитемс** с атрибутом **xsi: nil** со значением **true** в ответе SOAP.</span><span class="sxs-lookup"><span data-stu-id="1ad02-185">Versions of Exchange starting with major version 15 return extra **Group** or **GroupedItems** elements with the **xsi:nil** attribute set to **true** in the SOAP response.</span></span> <span data-ttu-id="1ad02-186">Если вы используете управляемый API EWS, эти дополнительные элементы приведут к созданию [сервицексмлдесериализатионексцептион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="1ad02-186">If you are using the EWS Managed API, these extra elements will cause a [ServiceXmlDeserializationException](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.servicexmldeserializationexception%28v=exchg.80%29.aspx) to be thrown.</span></span> <span data-ttu-id="1ad02-187">Если вы используете EWS, эти дополнительные элементы следует игнорировать.</span><span class="sxs-lookup"><span data-stu-id="1ad02-187">If you are using EWS, these extra elements should be ignored.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1ad02-188">См. также</span><span class="sxs-lookup"><span data-stu-id="1ad02-188">See also</span></span>

- [<span data-ttu-id="1ad02-189">Поиск и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="1ad02-189">Search and EWS in Exchange</span></span>](search-and-ews-in-exchange.md)    
- [<span data-ttu-id="1ad02-190">ExchangeService.FindItems</span><span class="sxs-lookup"><span data-stu-id="1ad02-190">ExchangeService.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="1ad02-191">Folder. FindItems</span><span class="sxs-lookup"><span data-stu-id="1ad02-191">Folder.FindItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="1ad02-192">Класс GROUPING</span><span class="sxs-lookup"><span data-stu-id="1ad02-192">Grouping class</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.grouping%28v=exchg.80%29.aspx)    
- [<span data-ttu-id="1ad02-193">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="1ad02-193">FindItem operation</span></span>](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)
    

