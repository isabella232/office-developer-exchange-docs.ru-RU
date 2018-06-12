---
title: IsWorkTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsWorkTime
api_type:
- schema
ms.assetid: 5243dd19-3593-4a81-bb2d-90496e04cb98
description: Элемент IsWorkTime представляет ли заданное время предложенного собрания во время запланированных трудозатрат.
ms.openlocfilehash: c687b29df226ebb28cdf01d3a2da62590f790924
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834135"
---
# <a name="isworktime"></a><span data-ttu-id="e2e09-103">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="e2e09-103">IsWorkTime</span></span>

<span data-ttu-id="e2e09-104">Элемент **IsWorkTime** представляет ли заданное время предложенного собрания во время запланированных трудозатрат.</span><span class="sxs-lookup"><span data-stu-id="e2e09-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="e2e09-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e2e09-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e2e09-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="e2e09-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="e2e09-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="e2e09-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="e2e09-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="e2e09-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="e2e09-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="e2e09-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="e2e09-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="e2e09-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="e2e09-111">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="e2e09-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="e2e09-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e2e09-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2e09-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2e09-113">Attributes and elements</span></span>

<span data-ttu-id="e2e09-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e2e09-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2e09-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2e09-115">Attributes</span></span>

<span data-ttu-id="e2e09-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2e09-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2e09-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2e09-117">Child elements</span></span>

<span data-ttu-id="e2e09-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2e09-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2e09-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2e09-119">Parent elements</span></span>

|<span data-ttu-id="e2e09-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2e09-120">**Element**</span></span>|<span data-ttu-id="e2e09-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2e09-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2e09-122">Предложения</span><span class="sxs-lookup"><span data-stu-id="e2e09-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="e2e09-123">Представляет один предложения о времени на собрания.</span><span class="sxs-lookup"><span data-stu-id="e2e09-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="e2e09-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e2e09-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2e09-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e2e09-125">Text value</span></span>

<span data-ttu-id="e2e09-126">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e2e09-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2e09-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="e2e09-127">Remarks</span></span>

<span data-ttu-id="e2e09-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e2e09-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2e09-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2e09-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2e09-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2e09-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2e09-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2e09-131">Schema Name</span></span>  <br/> |<span data-ttu-id="e2e09-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e2e09-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2e09-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2e09-133">Validation File</span></span>  <br/> |<span data-ttu-id="e2e09-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2e09-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2e09-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2e09-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2e09-136">False</span><span class="sxs-lookup"><span data-stu-id="e2e09-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2e09-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e2e09-137">See also</span></span>



[<span data-ttu-id="e2e09-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e2e09-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e2e09-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e2e09-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e2e09-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e2e09-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

