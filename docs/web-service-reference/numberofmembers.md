---
title: NumberOfMembers
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembers
api_type:
- schema
ms.assetid: 845fb877-de49-4e26-8885-6f026edd9ee9
description: Элемент NumberOfMembers представляет число пользователей, ресурсов и помещения в список рассылки.
ms.openlocfilehash: 9777660b1a54bfb5afb6e569ba1009a1654bdef3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834635"
---
# <a name="numberofmembers"></a><span data-ttu-id="07651-103">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="07651-103">NumberOfMembers</span></span>

<span data-ttu-id="07651-104">Элемент **NumberOfMembers** представляет число пользователей, ресурсов и помещения в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="07651-104">The **NumberOfMembers** element represents the number of users, resources, and rooms in a distribution list.</span></span> 
  
[<span data-ttu-id="07651-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="07651-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="07651-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="07651-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="07651-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="07651-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="07651-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="07651-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="07651-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="07651-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="07651-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="07651-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="07651-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="07651-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="07651-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="07651-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="07651-113">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="07651-113">NumberOfMembers</span></span>](numberofmembers.md)
  
```xml
<NumberOfMembers>...</NumberOfMembers>
```

 <span data-ttu-id="07651-114">**int**</span><span class="sxs-lookup"><span data-stu-id="07651-114">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="07651-115">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07651-115">Attributes and elements</span></span>

<span data-ttu-id="07651-116">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="07651-116">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07651-117">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07651-117">Attributes</span></span>

<span data-ttu-id="07651-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="07651-118">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07651-119">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07651-119">Child elements</span></span>

<span data-ttu-id="07651-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="07651-120">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07651-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07651-121">Parent elements</span></span>

|<span data-ttu-id="07651-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07651-122">**Element**</span></span>|<span data-ttu-id="07651-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07651-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07651-124">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="07651-124">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="07651-125">Содержит конфликта статистические сведения об число доступных пользователей, число пользователей, имеющих конфликтов и количество пользователей, у которых нет сведений о доступности в списке рассылки для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="07651-125">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="07651-126">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="07651-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07651-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="07651-127">Remarks</span></span>

<span data-ttu-id="07651-128">Максимальное значение элемента **NumberOfMembers** равно 100.</span><span class="sxs-lookup"><span data-stu-id="07651-128">The maximum value of the **NumberOfMembers** element is 100.</span></span> 
  
<span data-ttu-id="07651-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="07651-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07651-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07651-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07651-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07651-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07651-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07651-132">Schema Name</span></span>  <br/> |<span data-ttu-id="07651-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="07651-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="07651-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07651-134">Validation File</span></span>  <br/> |<span data-ttu-id="07651-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07651-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07651-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07651-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="07651-137">False</span><span class="sxs-lookup"><span data-stu-id="07651-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07651-138">См. также</span><span class="sxs-lookup"><span data-stu-id="07651-138">See also</span></span>



[<span data-ttu-id="07651-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="07651-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="07651-140">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="07651-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="07651-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="07651-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

