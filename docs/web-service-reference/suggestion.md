---
title: Предложения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Suggestion
api_type:
- schema
ms.assetid: 040a5c8f-b62f-4d1d-9d2c-dc3c5e01481f
description: Элемент предложения представляет предложение одного собрания.
ms.openlocfilehash: 24e2db1e0eabe35f7c971b0f1dbcbd333358f171
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840109"
---
# <a name="suggestion"></a><span data-ttu-id="16a24-103">Предложения</span><span class="sxs-lookup"><span data-stu-id="16a24-103">Suggestion</span></span>

<span data-ttu-id="16a24-104">Элемент **предложения** представляет предложение одного собрания.</span><span class="sxs-lookup"><span data-stu-id="16a24-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="16a24-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="16a24-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="16a24-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="16a24-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="16a24-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="16a24-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="16a24-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="16a24-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="16a24-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="16a24-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="16a24-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="16a24-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="16a24-111">**Предложения**</span><span class="sxs-lookup"><span data-stu-id="16a24-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="16a24-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="16a24-112">Attributes and elements</span></span>

<span data-ttu-id="16a24-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="16a24-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16a24-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="16a24-114">Attributes</span></span>

<span data-ttu-id="16a24-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="16a24-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16a24-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="16a24-116">Child elements</span></span>

|<span data-ttu-id="16a24-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16a24-117">**Element**</span></span>|<span data-ttu-id="16a24-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16a24-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16a24-119">MeetingTime</span><span class="sxs-lookup"><span data-stu-id="16a24-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="16a24-120">Представляет предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="16a24-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="16a24-121">IsWorkTime</span><span class="sxs-lookup"><span data-stu-id="16a24-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="16a24-122">Представляет ли заданное время предложенного собрания во время запланированных трудозатрат.</span><span class="sxs-lookup"><span data-stu-id="16a24-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="16a24-123">SuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="16a24-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="16a24-124">Представляет качества предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="16a24-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="16a24-125">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="16a24-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="16a24-126">Содержит массив сведения, описывающие конфликты между пользователями и ресурсы и предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="16a24-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="16a24-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="16a24-127">Parent elements</span></span>

|<span data-ttu-id="16a24-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="16a24-128">**Element**</span></span>|<span data-ttu-id="16a24-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="16a24-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="16a24-130">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="16a24-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="16a24-131">Содержит массив раз предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="16a24-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="16a24-132">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="16a24-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="16a24-133">Замечания</span><span class="sxs-lookup"><span data-stu-id="16a24-133">Remarks</span></span>

<span data-ttu-id="16a24-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="16a24-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16a24-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="16a24-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16a24-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="16a24-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16a24-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="16a24-137">Schema Name</span></span>  <br/> |<span data-ttu-id="16a24-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="16a24-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="16a24-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="16a24-139">Validation File</span></span>  <br/> |<span data-ttu-id="16a24-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="16a24-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="16a24-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="16a24-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="16a24-142">False</span><span class="sxs-lookup"><span data-stu-id="16a24-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="16a24-143">См. также</span><span class="sxs-lookup"><span data-stu-id="16a24-143">See also</span></span>



[<span data-ttu-id="16a24-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="16a24-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="16a24-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="16a24-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="16a24-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="16a24-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

