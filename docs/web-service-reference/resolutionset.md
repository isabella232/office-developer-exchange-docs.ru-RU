---
title: ResolutionSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolutionSet
api_type:
- schema
ms.assetid: 43d5b876-0e87-4414-9b1d-bff1c1ec825c
description: Элемент ResolutionSet содержит массив способы решения для разрешения неоднозначных псевдонимов.
ms.openlocfilehash: ad7bd31c85051e8c80aea25aa9e6f2914cf0ad01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835160"
---
# <a name="resolutionset"></a><span data-ttu-id="88f2e-103">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="88f2e-103">ResolutionSet</span></span>

<span data-ttu-id="88f2e-104">Элемент **ResolutionSet** содержит массив способы решения для разрешения неоднозначных псевдонимов.</span><span class="sxs-lookup"><span data-stu-id="88f2e-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="88f2e-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="88f2e-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="88f2e-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="88f2e-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="88f2e-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88f2e-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="88f2e-108">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="88f2e-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="88f2e-109">**ArrayOfResolutionType**</span><span class="sxs-lookup"><span data-stu-id="88f2e-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88f2e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88f2e-110">Attributes and elements</span></span>

<span data-ttu-id="88f2e-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="88f2e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88f2e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88f2e-112">Attributes</span></span>

|<span data-ttu-id="88f2e-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="88f2e-113">**Attribute**</span></span>|<span data-ttu-id="88f2e-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88f2e-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88f2e-115">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="88f2e-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="88f2e-116">Представляет следующий индекс, который необходимо использовать для следующего запроса при использовании индексированного страницы представления.</span><span class="sxs-lookup"><span data-stu-id="88f2e-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="88f2e-117">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="88f2e-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="88f2e-118">Представляет новое значение перечислителя использовать для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="88f2e-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="88f2e-119">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="88f2e-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="88f2e-120">Представляет Далее делителя будет использоваться для следующего запроса при использовании просмотров страниц дроби.</span><span class="sxs-lookup"><span data-stu-id="88f2e-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="88f2e-121">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="88f2e-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="88f2e-122">Этот атрибут будет значение true, если текущие результаты содержат последнего элемента в запросе, не требуются дополнительные разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="88f2e-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="88f2e-123">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="88f2e-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="88f2e-124">Представляет общее число элементов в представлении.</span><span class="sxs-lookup"><span data-stu-id="88f2e-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88f2e-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88f2e-125">Child elements</span></span>

|<span data-ttu-id="88f2e-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88f2e-126">**Element**</span></span>|<span data-ttu-id="88f2e-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88f2e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88f2e-128">Решение</span><span class="sxs-lookup"><span data-stu-id="88f2e-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="88f2e-129">Содержит одного объекта разрешения.</span><span class="sxs-lookup"><span data-stu-id="88f2e-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88f2e-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88f2e-130">Parent elements</span></span>

|<span data-ttu-id="88f2e-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88f2e-131">**Element**</span></span>|<span data-ttu-id="88f2e-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88f2e-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88f2e-133">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="88f2e-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="88f2e-134">Содержит состояние и результат запроса ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="88f2e-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88f2e-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="88f2e-135">Remarks</span></span>

<span data-ttu-id="88f2e-136">Элемент **ResolutionSet** может содержать не более 100 разрешить сущности.</span><span class="sxs-lookup"><span data-stu-id="88f2e-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="88f2e-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="88f2e-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88f2e-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88f2e-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88f2e-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88f2e-139">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88f2e-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88f2e-140">Schema Name</span></span>  <br/> |<span data-ttu-id="88f2e-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="88f2e-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="88f2e-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88f2e-142">Validation File</span></span>  <br/> |<span data-ttu-id="88f2e-143">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="88f2e-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88f2e-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88f2e-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="88f2e-145">False</span><span class="sxs-lookup"><span data-stu-id="88f2e-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88f2e-146">См. также</span><span class="sxs-lookup"><span data-stu-id="88f2e-146">See also</span></span>



[<span data-ttu-id="88f2e-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="88f2e-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="88f2e-148">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="88f2e-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="88f2e-149">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="88f2e-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="88f2e-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="88f2e-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

