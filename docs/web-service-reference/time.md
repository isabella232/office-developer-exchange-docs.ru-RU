---
title: Time
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: Элемент времени представляет время перехода между зимнего и летнего времени.
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840164"
---
# <a name="time"></a><span data-ttu-id="94364-103">Время</span><span class="sxs-lookup"><span data-stu-id="94364-103">Time</span></span>

<span data-ttu-id="94364-104">Элемент **времени** представляет время перехода между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="94364-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="94364-105">**string**</span><span class="sxs-lookup"><span data-stu-id="94364-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="94364-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="94364-106">Attributes and elements</span></span>

<span data-ttu-id="94364-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="94364-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="94364-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="94364-108">Attributes</span></span>

<span data-ttu-id="94364-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="94364-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="94364-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="94364-110">Child elements</span></span>

<span data-ttu-id="94364-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="94364-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="94364-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="94364-112">Parent elements</span></span>

|<span data-ttu-id="94364-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="94364-113">**Element**</span></span>|<span data-ttu-id="94364-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="94364-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="94364-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="94364-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="94364-116">Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="94364-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="94364-117">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="94364-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="94364-118">Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) .</span><span class="sxs-lookup"><span data-stu-id="94364-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="94364-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="94364-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="94364-120">Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="94364-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="94364-121">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="94364-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="94364-122">Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .</span><span class="sxs-lookup"><span data-stu-id="94364-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="94364-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="94364-123">Text value</span></span>

<span data-ttu-id="94364-124">Текстовое значение представляет часов, минут и секунд в следующем формате: ЧЧ.</span><span class="sxs-lookup"><span data-stu-id="94364-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="94364-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="94364-125">Remarks</span></span>

<span data-ttu-id="94364-126">При появлении элемента **времени** в элемент [DaylightTime](daylighttime.md) представляет время дня, осуществляется переход на летнее время происходит.</span><span class="sxs-lookup"><span data-stu-id="94364-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="94364-127">При появлении элемента [времени](time.md) в элемент [StandardTime](standardtime.md) представляет время дня, происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="94364-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="94364-128">Этот элемент имеет минимальные вхождения нулевой и максимальное одно вхождение.</span><span class="sxs-lookup"><span data-stu-id="94364-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="94364-129">Пример</span><span class="sxs-lookup"><span data-stu-id="94364-129">Example</span></span>

<span data-ttu-id="94364-130">Следующие части запроса, представляющий время перехода от 2: 00.</span><span class="sxs-lookup"><span data-stu-id="94364-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="94364-131">из стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="94364-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="94364-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="94364-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="94364-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="94364-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="94364-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="94364-134">Schema Name</span></span>  <br/> |<span data-ttu-id="94364-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="94364-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="94364-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="94364-136">Validation File</span></span>  <br/> |<span data-ttu-id="94364-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="94364-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="94364-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="94364-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="94364-139">False</span><span class="sxs-lookup"><span data-stu-id="94364-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="94364-140">См. также</span><span class="sxs-lookup"><span data-stu-id="94364-140">See also</span></span>

- [<span data-ttu-id="94364-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="94364-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="94364-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="94364-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

