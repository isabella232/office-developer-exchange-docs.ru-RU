---
title: MeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: Элемент MeetingTime представляет предложенного собрания.
ms.openlocfilehash: 1ea79be394124431aa1279ee94d5e5c6331d377b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834435"
---
# <a name="meetingtime"></a><span data-ttu-id="aaef7-103">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="aaef7-103">MeetingTime</span></span>

<span data-ttu-id="aaef7-104">Элемент **MeetingTime** представляет предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="aaef7-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="aaef7-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="aaef7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="aaef7-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="aaef7-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="aaef7-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="aaef7-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="aaef7-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="aaef7-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="aaef7-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="aaef7-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="aaef7-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="aaef7-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="aaef7-111">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="aaef7-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="aaef7-112">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="aaef7-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aaef7-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aaef7-113">Attributes and elements</span></span>

<span data-ttu-id="aaef7-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aaef7-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aaef7-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aaef7-115">Attributes</span></span>

<span data-ttu-id="aaef7-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="aaef7-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aaef7-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aaef7-117">Child elements</span></span>

<span data-ttu-id="aaef7-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="aaef7-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aaef7-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aaef7-119">Parent elements</span></span>

|<span data-ttu-id="aaef7-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aaef7-120">**Element**</span></span>|<span data-ttu-id="aaef7-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aaef7-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aaef7-122">Предложения</span><span class="sxs-lookup"><span data-stu-id="aaef7-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="aaef7-123">Представляет один предложения о времени на собрания.</span><span class="sxs-lookup"><span data-stu-id="aaef7-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="aaef7-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="aaef7-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aaef7-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aaef7-125">Text value</span></span>

<span data-ttu-id="aaef7-126">Текстовое значение, представляющее значение **даты и времени** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="aaef7-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aaef7-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="aaef7-127">Remarks</span></span>

<span data-ttu-id="aaef7-128">Элемент [MeetingTime](meetingtime.md) является обязательным дочерним элементом элемента [предложения](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="aaef7-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="aaef7-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aaef7-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="aaef7-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aaef7-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aaef7-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aaef7-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aaef7-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aaef7-132">Schema Name</span></span>  <br/> |<span data-ttu-id="aaef7-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aaef7-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="aaef7-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aaef7-134">Validation File</span></span>  <br/> |<span data-ttu-id="aaef7-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="aaef7-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aaef7-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aaef7-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="aaef7-137">False</span><span class="sxs-lookup"><span data-stu-id="aaef7-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aaef7-138">См. также</span><span class="sxs-lookup"><span data-stu-id="aaef7-138">See also</span></span>



[<span data-ttu-id="aaef7-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="aaef7-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="aaef7-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="aaef7-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="aaef7-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="aaef7-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

