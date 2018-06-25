---
title: SuggestionArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: Элемент SuggestionArray содержит массив предложений о собрании.
ms.openlocfilehash: d595ae77de293a1975e15102f3f2c3395e6da633
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840110"
---
# <a name="suggestionarray"></a><span data-ttu-id="7c68d-103">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7c68d-103">SuggestionArray</span></span>

<span data-ttu-id="7c68d-104">Элемент **SuggestionArray** содержит массив предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="7c68d-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="7c68d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7c68d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7c68d-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="7c68d-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7c68d-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="7c68d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="7c68d-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7c68d-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="7c68d-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="7c68d-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="7c68d-110">**ArrayOfSuggestion**</span><span class="sxs-lookup"><span data-stu-id="7c68d-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c68d-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7c68d-111">Attributes and elements</span></span>

<span data-ttu-id="7c68d-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7c68d-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c68d-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7c68d-113">Attributes</span></span>

<span data-ttu-id="7c68d-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="7c68d-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c68d-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7c68d-115">Child elements</span></span>

|<span data-ttu-id="7c68d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c68d-116">**Element**</span></span>|<span data-ttu-id="7c68d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c68d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c68d-118">Предложения</span><span class="sxs-lookup"><span data-stu-id="7c68d-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="7c68d-119">Представляет предложение одного собрания.</span><span class="sxs-lookup"><span data-stu-id="7c68d-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c68d-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7c68d-120">Parent elements</span></span>

|<span data-ttu-id="7c68d-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7c68d-121">**Element**</span></span>|<span data-ttu-id="7c68d-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7c68d-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c68d-123">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="7c68d-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="7c68d-124">Представляет один день, который содержит время предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="7c68d-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="7c68d-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7c68d-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c68d-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="7c68d-126">Remarks</span></span>

<span data-ttu-id="7c68d-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7c68d-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c68d-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7c68d-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c68d-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7c68d-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c68d-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7c68d-130">Schema Name</span></span>  <br/> |<span data-ttu-id="7c68d-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7c68d-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c68d-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7c68d-132">Validation File</span></span>  <br/> |<span data-ttu-id="7c68d-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7c68d-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c68d-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7c68d-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c68d-135">False</span><span class="sxs-lookup"><span data-stu-id="7c68d-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c68d-136">См. также</span><span class="sxs-lookup"><span data-stu-id="7c68d-136">See also</span></span>



[<span data-ttu-id="7c68d-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7c68d-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7c68d-138">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="7c68d-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7c68d-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="7c68d-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

