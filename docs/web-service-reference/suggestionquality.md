---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: Элемент SuggestionQuality представляет качества предложенного собрания.
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840112"
---
# <a name="suggestionquality"></a><span data-ttu-id="eca8d-103">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="eca8d-103">SuggestionQuality</span></span>

<span data-ttu-id="eca8d-104">Элемент **SuggestionQuality** представляет качества предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="eca8d-104">The **SuggestionQuality** element represents the quality of the suggested meeting time.</span></span> 
  
[<span data-ttu-id="eca8d-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eca8d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="eca8d-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="eca8d-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="eca8d-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="eca8d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="eca8d-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="eca8d-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="eca8d-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="eca8d-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="eca8d-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="eca8d-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="eca8d-111">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="eca8d-111">SuggestionQuality</span></span>](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 <span data-ttu-id="eca8d-112">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="eca8d-112">**SuggestionQuality**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eca8d-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eca8d-113">Attributes and elements</span></span>

<span data-ttu-id="eca8d-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eca8d-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eca8d-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eca8d-115">Attributes</span></span>

<span data-ttu-id="eca8d-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="eca8d-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eca8d-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eca8d-117">Child elements</span></span>

<span data-ttu-id="eca8d-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="eca8d-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="eca8d-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eca8d-119">Parent elements</span></span>

|<span data-ttu-id="eca8d-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eca8d-120">**Element**</span></span>|<span data-ttu-id="eca8d-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eca8d-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eca8d-122">Предложения</span><span class="sxs-lookup"><span data-stu-id="eca8d-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="eca8d-123">Представляет один предложения о времени на собрания.</span><span class="sxs-lookup"><span data-stu-id="eca8d-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="eca8d-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="eca8d-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="eca8d-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="eca8d-125">Text value</span></span>

<span data-ttu-id="eca8d-126">Текстовое значение, представляющее значение **SuggestionQuality** является обязательным.</span><span class="sxs-lookup"><span data-stu-id="eca8d-126">A text value that represents a **SuggestionQuality** value is required.</span></span> <span data-ttu-id="eca8d-127">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="eca8d-127">The following are the possible values:</span></span> 
  
- <span data-ttu-id="eca8d-128">**Отличное** 100 процентов пользователей и ресурсов, доступных для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="eca8d-128">**Excellent** 100 percent of users and resources are available for the suggested meeting time.</span></span> 
    
- <span data-ttu-id="eca8d-129">**Хороший** Минимальный процент пользователей и ресурсы, доступные равно или больше, чем значение элемента [GoodThreshold](goodthreshold.md) плюс 50.</span><span class="sxs-lookup"><span data-stu-id="eca8d-129">**Good** The minimum percentage of users and resources available is equal to or greater than the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> 
    
- <span data-ttu-id="eca8d-130">**Обычное** Максимальный процент пользователей и ресурсы, доступные для предложенного собрания равно значение элемента [GoodThreshold](goodthreshold.md) плюс 50.</span><span class="sxs-lookup"><span data-stu-id="eca8d-130">**Fair** The maximum percentage of users and resources available for a suggested meeting time is equal to the [GoodThreshold](goodthreshold.md) element value plus 50.</span></span> <span data-ttu-id="eca8d-131">Минимальное значение для **Обычное** время собрания качества — 50 процентов.</span><span class="sxs-lookup"><span data-stu-id="eca8d-131">The minimum value for a **Fair** quality meeting time is 50 percent.</span></span> 
    
- <span data-ttu-id="eca8d-132">**Низкий** Меньше 50% пользователей и ресурсов, доступных для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="eca8d-132">**Poor** Less than 50 percent of the users and resources are available for the suggested meeting time.</span></span> 
    
## <a name="remarks"></a><span data-ttu-id="eca8d-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="eca8d-133">Remarks</span></span>

<span data-ttu-id="eca8d-134">Тип **SuggestionQuality** также является типом для [DayQuality](dayquality.md) и [MinimumSuggestionQuality](minimumsuggestionquality.md) элементов.</span><span class="sxs-lookup"><span data-stu-id="eca8d-134">The **SuggestionQuality** type is also the type for the [DayQuality](dayquality.md) and the [MinimumSuggestionQuality](minimumsuggestionquality.md) elements.</span></span> 
  
<span data-ttu-id="eca8d-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="eca8d-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eca8d-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eca8d-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eca8d-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eca8d-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eca8d-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eca8d-138">Schema Name</span></span>  <br/> |<span data-ttu-id="eca8d-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="eca8d-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="eca8d-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eca8d-140">Validation File</span></span>  <br/> |<span data-ttu-id="eca8d-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eca8d-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eca8d-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eca8d-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="eca8d-143">False</span><span class="sxs-lookup"><span data-stu-id="eca8d-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eca8d-144">См. также</span><span class="sxs-lookup"><span data-stu-id="eca8d-144">See also</span></span>



[<span data-ttu-id="eca8d-145">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eca8d-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="eca8d-146">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eca8d-146">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="eca8d-147">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="eca8d-147">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

