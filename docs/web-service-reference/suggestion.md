---
title: Предложение
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
description: Элемент предложение представляет одно предложение о собрании.
ms.openlocfilehash: 25821abd5463ddba86a487709c8d2f8d928a94cc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530382"
---
# <a name="suggestion"></a><span data-ttu-id="d79fe-103">Предложение</span><span class="sxs-lookup"><span data-stu-id="d79fe-103">Suggestion</span></span>

<span data-ttu-id="d79fe-104">Элемент **предложение** представляет одно предложение о собрании.</span><span class="sxs-lookup"><span data-stu-id="d79fe-104">The **Suggestion** element represents a single meeting suggestion.</span></span> 
  
[<span data-ttu-id="d79fe-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d79fe-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d79fe-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="d79fe-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="d79fe-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="d79fe-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="d79fe-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="d79fe-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="d79fe-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="d79fe-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="d79fe-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="d79fe-110">Suggestion</span></span>](suggestion.md)
  
```xml
<Suggestion>
   <MeetingTime>...</MeetingTime>
   <IsWorkTime>...</IsWorkTime>
   <SuggestionQuality>...</SuggestionQuality>
   <AttendeeConflictDataArray>...</AttendeeConflictDataArray>
</Suggestion>
```

 <span data-ttu-id="d79fe-111">**Предложение**</span><span class="sxs-lookup"><span data-stu-id="d79fe-111">**Suggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d79fe-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d79fe-112">Attributes and elements</span></span>

<span data-ttu-id="d79fe-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d79fe-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d79fe-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d79fe-114">Attributes</span></span>

<span data-ttu-id="d79fe-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d79fe-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d79fe-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d79fe-116">Child elements</span></span>

|<span data-ttu-id="d79fe-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d79fe-117">**Element**</span></span>|<span data-ttu-id="d79fe-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d79fe-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d79fe-119">митингтиме</span><span class="sxs-lookup"><span data-stu-id="d79fe-119">MeetingTime</span></span>](meetingtime.md) <br/> |<span data-ttu-id="d79fe-120">Представляет предполагаемое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="d79fe-120">Represents a suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="d79fe-121">исворктиме</span><span class="sxs-lookup"><span data-stu-id="d79fe-121">IsWorkTime</span></span>](isworktime.md) <br/> |<span data-ttu-id="d79fe-122">Указывает, приходится ли предложенное время проведения собрания на запланированное рабочее время.</span><span class="sxs-lookup"><span data-stu-id="d79fe-122">Represents whether the suggested meeting time occurs during scheduled work hours.</span></span>  <br/> |
|[<span data-ttu-id="d79fe-123">сугжестионкуалити</span><span class="sxs-lookup"><span data-stu-id="d79fe-123">SuggestionQuality</span></span>](suggestionquality.md) <br/> |<span data-ttu-id="d79fe-124">Представляет качество предложенного времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="d79fe-124">Represents the quality of the suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="d79fe-125">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="d79fe-125">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="d79fe-126">Содержит массив данных, описывающих конфликты между пользователями и ресурсами, а также предполагаемое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="d79fe-126">Contains an array of information that describes conflicts between users and resources and the suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d79fe-127">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d79fe-127">Parent elements</span></span>

|<span data-ttu-id="d79fe-128">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d79fe-128">**Element**</span></span>|<span data-ttu-id="d79fe-129">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d79fe-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d79fe-130">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="d79fe-130">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="d79fe-131">Содержит массив предложенного времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="d79fe-131">Contains an array of suggested meeting times.</span></span>  <br/> <span data-ttu-id="d79fe-132">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d79fe-132">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d79fe-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="d79fe-133">Remarks</span></span>

<span data-ttu-id="d79fe-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d79fe-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d79fe-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d79fe-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d79fe-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d79fe-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d79fe-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d79fe-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d79fe-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d79fe-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d79fe-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d79fe-139">Validation File</span></span>  <br/> |<span data-ttu-id="d79fe-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d79fe-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d79fe-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d79fe-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d79fe-142">False</span><span class="sxs-lookup"><span data-stu-id="d79fe-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d79fe-143">См. также</span><span class="sxs-lookup"><span data-stu-id="d79fe-143">See also</span></span>



[<span data-ttu-id="d79fe-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d79fe-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d79fe-145">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d79fe-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d79fe-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d79fe-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

