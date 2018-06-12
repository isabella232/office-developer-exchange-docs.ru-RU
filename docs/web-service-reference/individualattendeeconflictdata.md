---
title: IndividualAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: Элемент IndividualAttendeeConflictData содержит пользователя или состояния занятости контакта для временной интервал, что происходит в то же время, как время предложенного собрания, определенный в элементе предложения.
ms.openlocfilehash: 0bd164e08a6f3685415452b7c82a4220cf69d792
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833930"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="d3e91-103">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="d3e91-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="d3e91-104">Элемент **IndividualAttendeeConflictData** содержит пользователя или состояния занятости контакта для временной интервал, что происходит в то же время, как время предложенного собрания, определенный в элементе [предложения](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="d3e91-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="d3e91-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d3e91-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d3e91-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="d3e91-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="d3e91-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="d3e91-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="d3e91-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="d3e91-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="d3e91-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="d3e91-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="d3e91-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="d3e91-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="d3e91-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="d3e91-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="d3e91-112">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="d3e91-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="d3e91-113">**IndividualAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="d3e91-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3e91-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3e91-114">Attributes and elements</span></span>

<span data-ttu-id="d3e91-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d3e91-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3e91-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3e91-116">Attributes</span></span>

<span data-ttu-id="d3e91-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3e91-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3e91-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3e91-118">Child elements</span></span>

|<span data-ttu-id="d3e91-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3e91-119">**Element**</span></span>|<span data-ttu-id="d3e91-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3e91-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3e91-121">BusyType</span><span class="sxs-lookup"><span data-stu-id="d3e91-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="d3e91-122">Представляет состояния занятости пользователя для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="d3e91-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3e91-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3e91-123">Parent elements</span></span>

|<span data-ttu-id="d3e91-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3e91-124">**Element**</span></span>|<span data-ttu-id="d3e91-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3e91-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3e91-126">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="d3e91-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="d3e91-127">Содержит массив данных конфликта участников, определенный в [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="d3e91-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="d3e91-128">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d3e91-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3e91-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3e91-129">Remarks</span></span>

<span data-ttu-id="d3e91-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d3e91-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3e91-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3e91-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3e91-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3e91-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3e91-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3e91-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d3e91-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3e91-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3e91-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3e91-135">Validation File</span></span>  <br/> |<span data-ttu-id="d3e91-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3e91-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3e91-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3e91-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3e91-138">False</span><span class="sxs-lookup"><span data-stu-id="d3e91-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3e91-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d3e91-139">See also</span></span>



[<span data-ttu-id="d3e91-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d3e91-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d3e91-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d3e91-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d3e91-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d3e91-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

