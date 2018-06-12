---
title: NumberOfMembersAvailable
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersAvailable
api_type:
- schema
ms.assetid: e367a278-1622-4b65-955f-2d4b2fc6e4d7
description: Элемент NumberOfMembersAvailable представляет число членов списка рассылки, которые доступны для предложенного собрания. Этот элемент представляет элементы, для которых состояние — бесплатными.
ms.openlocfilehash: 8669f61fbd640c160ad54739c5a15407b3dd470a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834641"
---
# <a name="numberofmembersavailable"></a><span data-ttu-id="59120-104">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="59120-104">NumberOfMembersAvailable</span></span>

<span data-ttu-id="59120-105">Элемент **NumberOfMembersAvailable** представляет число членов списка рассылки, которые доступны для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="59120-105">The **NumberOfMembersAvailable** element represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="59120-106">Этот элемент представляет элементы, для которых состояние — **бесплатными**.</span><span class="sxs-lookup"><span data-stu-id="59120-106">This element represents members for whom the status is **Free**.</span></span>
  
[<span data-ttu-id="59120-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="59120-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="59120-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="59120-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="59120-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="59120-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="59120-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="59120-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="59120-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="59120-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="59120-112">Предложения</span><span class="sxs-lookup"><span data-stu-id="59120-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="59120-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="59120-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="59120-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="59120-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="59120-115">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="59120-115">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md)
  
```xml
<NumberOfMembersAvailable>...</NumberOfMembersAvailable>
```

 <span data-ttu-id="59120-116">**int**</span><span class="sxs-lookup"><span data-stu-id="59120-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59120-117">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="59120-117">Attributes and elements</span></span>

<span data-ttu-id="59120-118">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="59120-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59120-119">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="59120-119">Attributes</span></span>

<span data-ttu-id="59120-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="59120-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59120-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="59120-121">Child elements</span></span>

<span data-ttu-id="59120-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="59120-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59120-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="59120-123">Parent elements</span></span>

|<span data-ttu-id="59120-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="59120-124">**Element**</span></span>|<span data-ttu-id="59120-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="59120-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59120-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="59120-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="59120-127">Содержит конфликта статистические сведения об количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в списке рассылки для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="59120-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="59120-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="59120-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="59120-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="59120-129">Remarks</span></span>

<span data-ttu-id="59120-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="59120-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59120-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="59120-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59120-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="59120-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59120-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="59120-133">Schema Name</span></span>  <br/> |<span data-ttu-id="59120-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="59120-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="59120-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="59120-135">Validation File</span></span>  <br/> |<span data-ttu-id="59120-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59120-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59120-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="59120-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="59120-138">False</span><span class="sxs-lookup"><span data-stu-id="59120-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59120-139">См. также</span><span class="sxs-lookup"><span data-stu-id="59120-139">See also</span></span>



[<span data-ttu-id="59120-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="59120-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="59120-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="59120-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="59120-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="59120-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

