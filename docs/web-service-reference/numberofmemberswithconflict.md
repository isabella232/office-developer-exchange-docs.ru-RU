---
title: NumberOfMembersWithConflict
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithConflict
api_type:
- schema
ms.assetid: e61154f7-d262-43ec-b2bf-1ba6804b28dc
description: Элемент NumberOfMembersWithConflict представляет число членов списка рассылки, конфликт с временем предложенного собрания. Этот элемент представляет работников, которые имеют состояние «занят», об отсутствии на работе или под вопросом.
ms.openlocfilehash: 227783b4bed32686e8e098f88498fe8ebb25e3cc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834634"
---
# <a name="numberofmemberswithconflict"></a><span data-ttu-id="febde-104">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="febde-104">NumberOfMembersWithConflict</span></span>

<span data-ttu-id="febde-105">Элемент **NumberOfMembersWithConflict** представляет число членов списка рассылки, конфликт с временем предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="febde-105">The **NumberOfMembersWithConflict** element represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="febde-106">Этот элемент представляет работников, которые имеют состояние **«занят»**, **об отсутствии на работе**или **под вопросом**.</span><span class="sxs-lookup"><span data-stu-id="febde-106">This element represents members who have a status of **Busy**, **OOF**, or **Tentative**.</span></span>
  
[<span data-ttu-id="febde-107">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="febde-107">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="febde-108">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="febde-108">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="febde-109">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="febde-109">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="febde-110">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="febde-110">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="febde-111">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="febde-111">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="febde-112">Предложения</span><span class="sxs-lookup"><span data-stu-id="febde-112">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="febde-113">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="febde-113">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="febde-114">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="febde-114">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
[<span data-ttu-id="febde-115">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="febde-115">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md)
  
```xml
<NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
```

 <span data-ttu-id="febde-116">**int**</span><span class="sxs-lookup"><span data-stu-id="febde-116">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="febde-117">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="febde-117">Attributes and elements</span></span>

<span data-ttu-id="febde-118">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="febde-118">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="febde-119">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="febde-119">Attributes</span></span>

<span data-ttu-id="febde-120">Нет.</span><span class="sxs-lookup"><span data-stu-id="febde-120">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="febde-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="febde-121">Child elements</span></span>

<span data-ttu-id="febde-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="febde-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="febde-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="febde-123">Parent elements</span></span>

|<span data-ttu-id="febde-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="febde-124">**Element**</span></span>|<span data-ttu-id="febde-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="febde-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="febde-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="febde-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="febde-127">Содержит конфликта статистические сведения об количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в списке рассылки для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="febde-127">Contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> <span data-ttu-id="febde-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="febde-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="febde-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="febde-129">Remarks</span></span>

<span data-ttu-id="febde-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="febde-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="febde-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="febde-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="febde-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="febde-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="febde-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="febde-133">Schema Name</span></span>  <br/> |<span data-ttu-id="febde-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="febde-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="febde-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="febde-135">Validation File</span></span>  <br/> |<span data-ttu-id="febde-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="febde-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="febde-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="febde-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="febde-138">False</span><span class="sxs-lookup"><span data-stu-id="febde-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="febde-139">См. также</span><span class="sxs-lookup"><span data-stu-id="febde-139">See also</span></span>



[<span data-ttu-id="febde-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="febde-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="febde-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="febde-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="febde-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="febde-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

