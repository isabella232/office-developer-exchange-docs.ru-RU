---
title: DayOfWeek (часовой пояс)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: Элемент DayOfWeek представляет день недели, на котором происходит переход часового пояса.
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761993"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="e4c94-103">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="e4c94-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="e4c94-104">Элемент **DayOfWeek** представляет день недели, на котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e4c94-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="e4c94-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="e4c94-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e4c94-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4c94-106">Attributes and elements</span></span>

<span data-ttu-id="e4c94-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e4c94-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4c94-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4c94-108">Attributes</span></span>

<span data-ttu-id="e4c94-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4c94-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4c94-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4c94-110">Child elements</span></span>

<span data-ttu-id="e4c94-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e4c94-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4c94-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4c94-112">Parent elements</span></span>

|<span data-ttu-id="e4c94-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4c94-113">**Element**</span></span>|<span data-ttu-id="e4c94-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4c94-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c94-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="e4c94-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="e4c94-116">Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="e4c94-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="e4c94-117">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="e4c94-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="e4c94-118">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e4c94-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="e4c94-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="e4c94-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="e4c94-120">Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="e4c94-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="e4c94-121">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="e4c94-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="e4c94-122">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e4c94-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="e4c94-123">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="e4c94-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="e4c94-124">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="e4c94-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4c94-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4c94-125">Text value</span></span>

<span data-ttu-id="e4c94-126">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e4c94-126">A text value is required.</span></span> <span data-ttu-id="e4c94-127">Текстовое значение представлено перечислением, который имеет следующие возможные значения:</span><span class="sxs-lookup"><span data-stu-id="e4c94-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="e4c94-128">Воскресенье</span><span class="sxs-lookup"><span data-stu-id="e4c94-128">Sunday</span></span>    
- <span data-ttu-id="e4c94-129">Понедельник</span><span class="sxs-lookup"><span data-stu-id="e4c94-129">Monday</span></span>    
- <span data-ttu-id="e4c94-130">Вторник</span><span class="sxs-lookup"><span data-stu-id="e4c94-130">Tuesday</span></span>    
- <span data-ttu-id="e4c94-131">Среда</span><span class="sxs-lookup"><span data-stu-id="e4c94-131">Wednesday</span></span>    
- <span data-ttu-id="e4c94-132">Четверг</span><span class="sxs-lookup"><span data-stu-id="e4c94-132">Thursday</span></span>    
- <span data-ttu-id="e4c94-133">Пятница</span><span class="sxs-lookup"><span data-stu-id="e4c94-133">Friday</span></span>    
- <span data-ttu-id="e4c94-134">Суббота</span><span class="sxs-lookup"><span data-stu-id="e4c94-134">Saturday</span></span>    
- <span data-ttu-id="e4c94-135">День</span><span class="sxs-lookup"><span data-stu-id="e4c94-135">Day</span></span>    
- <span data-ttu-id="e4c94-136">День недели</span><span class="sxs-lookup"><span data-stu-id="e4c94-136">Weekday</span></span>   
- <span data-ttu-id="e4c94-137">WeekendDay</span><span class="sxs-lookup"><span data-stu-id="e4c94-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e4c94-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="e4c94-138">Remarks</span></span>

<span data-ttu-id="e4c94-139">Элемент [StandardTime](standardtime.md) , который содержит элемент [DayOrder](dayorder.md) , который имеет значение 5, [месяц](month.md) , который имеет значение 10 и элемент **DayOfWeek** , который имеет значение воскресенье означает, что переход на летнее экономии времени происходящее в пятый воскресенье десятой месяца.</span><span class="sxs-lookup"><span data-stu-id="e4c94-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="e4c94-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4c94-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4c94-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4c94-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4c94-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4c94-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4c94-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4c94-143">Schema Name</span></span>  <br/> |<span data-ttu-id="e4c94-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4c94-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4c94-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4c94-145">Validation File</span></span>  <br/> |<span data-ttu-id="e4c94-146">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4c94-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4c94-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4c94-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4c94-148">False</span><span class="sxs-lookup"><span data-stu-id="e4c94-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4c94-149">См. также</span><span class="sxs-lookup"><span data-stu-id="e4c94-149">See also</span></span>

- [<span data-ttu-id="e4c94-150">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e4c94-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e4c94-151">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e4c94-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

