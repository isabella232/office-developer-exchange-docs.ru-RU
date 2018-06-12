---
title: RootFolder (FindItemResponseMessage)
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
description: Элемент RootFolder содержит результаты поиска в одной корневой папке во время операции FindItem.
ms.openlocfilehash: ea17369ef4efc4112a738b430c8f0dbab3886341
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835254"
---
# <a name="rootfolder-finditemresponsemessage"></a><span data-ttu-id="03034-103">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="03034-103">RootFolder (FindItemResponseMessage)</span></span>

<span data-ttu-id="03034-104">Элемент **RootFolder** содержит результаты поиска в одной корневой папке во время [операции FindItem](finditem-operation.md).</span><span class="sxs-lookup"><span data-stu-id="03034-104">The **RootFolder** element contains the results of a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>
  
```xml
<RootFolder IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Items/>
   <Groups/>
</RootFolder>
```

 <span data-ttu-id="03034-105">**FindItemParentType**</span><span class="sxs-lookup"><span data-stu-id="03034-105">**FindItemParentType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03034-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="03034-106">Attributes and elements</span></span>

<span data-ttu-id="03034-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="03034-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03034-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="03034-108">Attributes</span></span>

|<span data-ttu-id="03034-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="03034-109">**Attribute**</span></span>|<span data-ttu-id="03034-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03034-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="03034-111">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="03034-111">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="03034-112">Представляет следующий индекс, который следует использовать для следующего запроса при использовании индексированного представления разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="03034-112">Represents the next index that should be used for the next request when using an indexed paging view.</span></span>  <br/> |
|<span data-ttu-id="03034-113">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="03034-113">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="03034-114">Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="03034-114">Represents the new numerator value to use for the next request when using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="03034-115">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="03034-115">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="03034-116">Представляет Далее делителя для использования в следующем запросе при выполнении дробная разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="03034-116">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="03034-117">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="03034-117">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="03034-118">Указывает, содержат ли текущие результаты последнего элемента в запросе, таким образом, что дальнейшей постраничного просмотра не требуется.</span><span class="sxs-lookup"><span data-stu-id="03034-118">Indicates whether the current results contain the last item in the query, such that further paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="03034-119">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="03034-119">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="03034-120">Представляет общее число элементов, которые ограничение игнорируется.</span><span class="sxs-lookup"><span data-stu-id="03034-120">Represents the total number of items that pass the restriction.</span></span> <span data-ttu-id="03034-121">В сгруппированных [операции FindItem](finditem-operation.md)атрибут **TotalItemsInView** возвращает общее число элементов в представлении, а также общее число групп.</span><span class="sxs-lookup"><span data-stu-id="03034-121">In a grouped [FindItem operation](finditem-operation.md), the **TotalItemsInView** attribute returns the total number of items in the view plus the total number of groups.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="03034-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="03034-122">Child elements</span></span>

|<span data-ttu-id="03034-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03034-123">**Element**</span></span>|<span data-ttu-id="03034-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03034-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03034-125">Элементы</span><span class="sxs-lookup"><span data-stu-id="03034-125">Items</span></span>](items.md) <br/> |<span data-ttu-id="03034-126">Содержит массив найденных элементов, у которых критерии поиска, определенные в запросе на [операции FindItem](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="03034-126">Contains an array of items found that have the search criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
|[<span data-ttu-id="03034-127">Группы</span><span class="sxs-lookup"><span data-stu-id="03034-127">Groups</span></span>](groups.md) <br/> |<span data-ttu-id="03034-128">Содержит коллекцию найдено групп, у которых поиска и объединение критериям, заданным в запрос [FindItem операции](finditem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="03034-128">Contains a collection of groups found that have the search and aggregation criteria identified in the [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="03034-129">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="03034-129">Parent elements</span></span>

|<span data-ttu-id="03034-130">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="03034-130">**Element**</span></span>|<span data-ttu-id="03034-131">**Описание**</span><span class="sxs-lookup"><span data-stu-id="03034-131">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03034-132">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="03034-132">FindItemResponseMessage</span></span>](finditemresponsemessage.md) <br/> |<span data-ttu-id="03034-133">Содержит состояние и результат [операции FindItem](finditem-operation.md) запроса.</span><span class="sxs-lookup"><span data-stu-id="03034-133">Contains the status and result of a [FindItem operation](finditem-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="03034-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="03034-134">Remarks</span></span>

<span data-ttu-id="03034-135">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором работает Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="03034-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03034-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="03034-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03034-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="03034-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03034-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="03034-138">Schema name</span></span>  <br/> |<span data-ttu-id="03034-139">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="03034-139">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03034-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="03034-140">Validation file</span></span>  <br/> |<span data-ttu-id="03034-141">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="03034-141">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03034-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="03034-142">Can be empty</span></span>  <br/> |<span data-ttu-id="03034-143">False</span><span class="sxs-lookup"><span data-stu-id="03034-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03034-144">См. также</span><span class="sxs-lookup"><span data-stu-id="03034-144">See also</span></span>



[<span data-ttu-id="03034-145">FindItem Operation</span><span class="sxs-lookup"><span data-stu-id="03034-145">FindItem operation</span></span>](finditem-operation.md)
  
[<span data-ttu-id="03034-146">IndexedPagingOffset</span><span class="sxs-lookup"><span data-stu-id="03034-146">IndexedPagingOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IndexedPagingOffset.aspx)
  
[<span data-ttu-id="03034-147">NumeratorOffset</span><span class="sxs-lookup"><span data-stu-id="03034-147">NumeratorOffset</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.NumeratorOffset.aspx)
  
[<span data-ttu-id="03034-148">AbsoluteDenominator</span><span class="sxs-lookup"><span data-stu-id="03034-148">AbsoluteDenominator</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.AbsoluteDenominator.aspx)
  
[<span data-ttu-id="03034-149">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="03034-149">IncludesLastItemInRange</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.IncludesLastItemInRange.aspx)
  
[<span data-ttu-id="03034-150">TotalItemsInView</span><span class="sxs-lookup"><span data-stu-id="03034-150">TotalItemsInView</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.FindItemParentType.TotalItemsInView.aspx)


[<span data-ttu-id="03034-151">Поиск элементов</span><span class="sxs-lookup"><span data-stu-id="03034-151">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

