---
title: Рутфолдер (Финдитемреспонсемессаже)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RootFolder
api_type:
- schema
ms.assetid: 187e009f-efaa-42a8-8962-329a645213ab
description: Элемент Рутфолдер содержит результаты поиска в одной корневой папке во время операции FindItem.
ms.openlocfilehash: 3bbab325dff26139739c50ef519b215aea620a0b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457132"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="f0df0-103">Рутфолдер (Финдитемреспонсемессаже)</span><span class="sxs-lookup"><span data-stu-id="f0df0-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="f0df0-104">Элемент **рутфолдер** содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="f0df0-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="f0df0-105">**финдитемпаренттипе**</span><span class="sxs-lookup"><span data-stu-id="f0df0-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0df0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f0df0-106">Attributes and elements</span></span>

<span data-ttu-id="f0df0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f0df0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0df0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f0df0-108">Attributes</span></span>

|<span data-ttu-id="f0df0-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f0df0-109">**Attribute**</span></span>|<span data-ttu-id="f0df0-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0df0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f0df0-111">**индекседпагингоффсет**</span><span class="sxs-lookup"><span data-stu-id="f0df0-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="f0df0-112">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления разбиения по страницам.</span><span class="sxs-lookup"><span data-stu-id="f0df0-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="f0df0-113">**нумератороффсет**</span><span class="sxs-lookup"><span data-stu-id="f0df0-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="f0df0-114">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.</span><span class="sxs-lookup"><span data-stu-id="f0df0-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="f0df0-115">**абсолутеденоминатор**</span><span class="sxs-lookup"><span data-stu-id="f0df0-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="f0df0-116">Представляет следующий знаменатель, который будет использоваться для следующего запроса при выполнении дробного разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="f0df0-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="f0df0-117">**инклудесластитеминранже**</span><span class="sxs-lookup"><span data-stu-id="f0df0-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="f0df0-118">Указывает, содержат ли текущие результаты последний элемент в запросе, что не требуется для дальнейшей разбиения на страницы.</span><span class="sxs-lookup"><span data-stu-id="f0df0-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="f0df0-119">**тоталитемсинвиев**</span><span class="sxs-lookup"><span data-stu-id="f0df0-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="f0df0-120">Представляет общее число элементов, которые прошли ограничение.</span><span class="sxs-lookup"><span data-stu-id="f0df0-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="f0df0-121">В сгруппированной [операции FindItem](finditem-operation.md)атрибут **тоталитемсинвиев** возвращает общее число элементов в представлении, а также общее число групп.</span><span class="sxs-lookup"><span data-stu-id="f0df0-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f0df0-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f0df0-122">Child elements</span></span>

|<span data-ttu-id="f0df0-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0df0-123">**Element**</span></span>|<span data-ttu-id="f0df0-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0df0-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0df0-125">Items</span><span class="sxs-lookup"><span data-stu-id="f0df0-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="f0df0-126">Содержит массив найденных элементов, которые содержат условия поиска, указанные в запросе [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0df0-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="f0df0-127">Groups</span><span class="sxs-lookup"><span data-stu-id="f0df0-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="f0df0-128">Содержит коллекцию найденных групп, которые содержат критерии поиска и объединения, указанные в запросе [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0df0-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0df0-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f0df0-129">Parent elements</span></span>

|<span data-ttu-id="f0df0-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f0df0-130">**Element**</span></span>|<span data-ttu-id="f0df0-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f0df0-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0df0-132">финдитемреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="f0df0-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="f0df0-133">Содержит состояние и результат запроса [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="f0df0-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f0df0-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="f0df0-134">Remarks</span></span>

<span data-ttu-id="f0df0-135">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором установлен сервер Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f0df0-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0df0-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f0df0-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0df0-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f0df0-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0df0-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f0df0-138">Schema name</span></span>  <br/> |<span data-ttu-id="f0df0-139">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="f0df0-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0df0-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f0df0-140">Validation file</span></span>  <br/> |<span data-ttu-id="f0df0-141">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f0df0-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0df0-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f0df0-142">Can be empty</span></span>  <br/> |<span data-ttu-id="f0df0-143">False</span><span class="sxs-lookup"><span data-stu-id="f0df0-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0df0-144">См. также</span><span class="sxs-lookup"><span data-stu-id="f0df0-144">See also</span></span>



[<span data-ttu-id="f0df0-145">Операция FindItem</span><span class="sxs-lookup"><span data-stu-id="f0df0-145">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="f0df0-146">индекседпагингоффсет</span><span class="sxs-lookup"><span data-stu-id="f0df0-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="f0df0-147">нумератороффсет</span><span class="sxs-lookup"><span data-stu-id="f0df0-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="f0df0-148">абсолутеденоминатор</span><span class="sxs-lookup"><span data-stu-id="f0df0-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="f0df0-149">инклудесластитеминранже</span><span class="sxs-lookup"><span data-stu-id="f0df0-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="f0df0-150">тоталитемсинвиев</span><span class="sxs-lookup"><span data-stu-id="f0df0-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="f0df0-151">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="f0df0-151">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

