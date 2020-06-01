---
title: Авторешение
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
description: Элемент "набор решений" содержит массив разрешений для неоднозначного имени.
ms.openlocfilehash: 483a096a7fcedbabe25758ebcaa31c83405a0ad4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467174"
---
# <a name="resolutionset"></a><span data-ttu-id="88d5b-103">Авторешение</span><span class="sxs-lookup"><span data-stu-id="88d5b-103">ResolutionSet</span></span>

<span data-ttu-id="88d5b-104">Элемент "набор **решений** " содержит массив разрешений для неоднозначного имени.</span><span class="sxs-lookup"><span data-stu-id="88d5b-104">The **ResolutionSet** element contains an array of resolutions for an ambiguous name.</span></span> 
  
[<span data-ttu-id="88d5b-105">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="88d5b-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="88d5b-106">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="88d5b-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="88d5b-107">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="88d5b-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="88d5b-108">Авторешение</span><span class="sxs-lookup"><span data-stu-id="88d5b-108">ResolutionSet</span></span>](resolutionset.md)
  
```xml
<ResolutionSet IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <Resolution/>
</ResolutionSet>
```

 <span data-ttu-id="88d5b-109">**аррайофресолутионтипе**</span><span class="sxs-lookup"><span data-stu-id="88d5b-109">**ArrayOfResolutionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="88d5b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="88d5b-110">Attributes and elements</span></span>

<span data-ttu-id="88d5b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="88d5b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="88d5b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="88d5b-112">Attributes</span></span>

|<span data-ttu-id="88d5b-113">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="88d5b-113">**Attribute**</span></span>|<span data-ttu-id="88d5b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88d5b-114">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="88d5b-115">**индекседпагингоффсет**</span><span class="sxs-lookup"><span data-stu-id="88d5b-115">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="88d5b-116">Представляет следующий индекс, который должен использоваться для следующего запроса при использовании индексированного представления страницы.</span><span class="sxs-lookup"><span data-stu-id="88d5b-116">Represents the next index that should be used for the next request when you are using an indexed page view.</span></span>  <br/> |
|<span data-ttu-id="88d5b-117">**нумератороффсет**</span><span class="sxs-lookup"><span data-stu-id="88d5b-117">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="88d5b-118">Представляет новое значение числителя, которое будет использоваться для следующего запроса при использовании представлений страницы дробей.</span><span class="sxs-lookup"><span data-stu-id="88d5b-118">Represents the new numerator value to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="88d5b-119">**абсолутеденоминатор**</span><span class="sxs-lookup"><span data-stu-id="88d5b-119">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="88d5b-120">Представляет следующий знаменатель, который будет использоваться для следующего запроса при использовании представлений страницы дробной части.</span><span class="sxs-lookup"><span data-stu-id="88d5b-120">Represents the next denominator to use for the next request when you are using fraction page views.</span></span>  <br/> |
|<span data-ttu-id="88d5b-121">**инклудесластитеминранже**</span><span class="sxs-lookup"><span data-stu-id="88d5b-121">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="88d5b-122">Этот атрибут будет иметь значение true, если текущие результаты содержат последний элемент в запросе, чтобы не требовалось дополнительное разбиение на страницы.</span><span class="sxs-lookup"><span data-stu-id="88d5b-122">This attribute will be true if the current results contain the last item in the query, so that additional paging is not needed.</span></span>  <br/> |
|<span data-ttu-id="88d5b-123">**тоталитемсинвиев**</span><span class="sxs-lookup"><span data-stu-id="88d5b-123">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="88d5b-124">Представляет общее число элементов в представлении.</span><span class="sxs-lookup"><span data-stu-id="88d5b-124">Represents the total number of items in the view.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="88d5b-125">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="88d5b-125">Child elements</span></span>

|<span data-ttu-id="88d5b-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88d5b-126">**Element**</span></span>|<span data-ttu-id="88d5b-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88d5b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88d5b-128">Resolution</span><span class="sxs-lookup"><span data-stu-id="88d5b-128">Resolution</span></span>](resolution.md) <br/> |<span data-ttu-id="88d5b-129">Содержит одну разрешенную сущность.</span><span class="sxs-lookup"><span data-stu-id="88d5b-129">Contains a single resolved entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="88d5b-130">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="88d5b-130">Parent elements</span></span>

|<span data-ttu-id="88d5b-131">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="88d5b-131">**Element**</span></span>|<span data-ttu-id="88d5b-132">**Описание**</span><span class="sxs-lookup"><span data-stu-id="88d5b-132">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="88d5b-133">ресолвенамесреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="88d5b-133">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md) <br/> |<span data-ttu-id="88d5b-134">Содержит состояние и результат запроса ResolveNames.</span><span class="sxs-lookup"><span data-stu-id="88d5b-134">Contains the status and result of a ResolveNames request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="88d5b-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="88d5b-135">Remarks</span></span>

<span data-ttu-id="88d5b-136">Элемент "набор **решений** " может содержать не более 100 разрешенных сущностей.</span><span class="sxs-lookup"><span data-stu-id="88d5b-136">A **ResolutionSet** element can contain a maximum of 100 resolved entities.</span></span> 
  
<span data-ttu-id="88d5b-137">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="88d5b-137">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="88d5b-138">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="88d5b-138">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="88d5b-139">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="88d5b-139">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="88d5b-140">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="88d5b-140">Schema Name</span></span>  <br/> |<span data-ttu-id="88d5b-141">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="88d5b-141">Messages schema</span></span>  <br/> |
|<span data-ttu-id="88d5b-142">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="88d5b-142">Validation File</span></span>  <br/> |<span data-ttu-id="88d5b-143">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="88d5b-143">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="88d5b-144">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="88d5b-144">Can be Empty</span></span>  <br/> |<span data-ttu-id="88d5b-145">False</span><span class="sxs-lookup"><span data-stu-id="88d5b-145">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="88d5b-146">См. также</span><span class="sxs-lookup"><span data-stu-id="88d5b-146">See also</span></span>



[<span data-ttu-id="88d5b-147">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="88d5b-147">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="88d5b-148">ресолвенамесреспонсе</span><span class="sxs-lookup"><span data-stu-id="88d5b-148">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
  
[<span data-ttu-id="88d5b-149">Операция ResolveNames</span><span class="sxs-lookup"><span data-stu-id="88d5b-149">ResolveNames operation</span></span>](resolvenames-operation.md)


- [<span data-ttu-id="88d5b-150">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="88d5b-150">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

