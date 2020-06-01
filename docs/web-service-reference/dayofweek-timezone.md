---
title: DayOfWeek (TimeZone)
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
description: Элемент DayOfWeek представляет день недели, в который происходит переход часового пояса.
ms.openlocfilehash: 7bc05f417268ccfb20adae12e2694d8360023ab2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457846"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="e4871-103">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="e4871-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="e4871-104">Элемент **DayOfWeek** представляет день недели, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e4871-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="e4871-105">**дайофвиктипе**</span><span class="sxs-lookup"><span data-stu-id="e4871-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e4871-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4871-106">Attributes and elements</span></span>

<span data-ttu-id="e4871-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e4871-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4871-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4871-108">Attributes</span></span>

<span data-ttu-id="e4871-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4871-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4871-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4871-110">Child elements</span></span>

<span data-ttu-id="e4871-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4871-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4871-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4871-112">Parent elements</span></span>

|<span data-ttu-id="e4871-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4871-113">**Element**</span></span>|<span data-ttu-id="e4871-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4871-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4871-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="e4871-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="e4871-116">Представляет смещение относительно времени относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="e4871-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="e4871-117">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="e4871-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="e4871-118">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e4871-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="e4871-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="e4871-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="e4871-120">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="e4871-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="e4871-121">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="e4871-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="e4871-122">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e4871-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="e4871-123">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="e4871-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="e4871-124">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="e4871-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4871-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4871-125">Text value</span></span>

<span data-ttu-id="e4871-126">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="e4871-126">A text value is required.</span></span> <span data-ttu-id="e4871-127">Текстовое значение представлено перечислением со следующими возможными значениями:</span><span class="sxs-lookup"><span data-stu-id="e4871-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="e4871-128">Воскресеньям</span><span class="sxs-lookup"><span data-stu-id="e4871-128">Sunday</span></span>    
- <span data-ttu-id="e4871-129">Понедельник</span><span class="sxs-lookup"><span data-stu-id="e4871-129">Monday</span></span>    
- <span data-ttu-id="e4871-130">Вторник</span><span class="sxs-lookup"><span data-stu-id="e4871-130">Tuesday</span></span>    
- <span data-ttu-id="e4871-131">Среда</span><span class="sxs-lookup"><span data-stu-id="e4871-131">Wednesday</span></span>    
- <span data-ttu-id="e4871-132">Четверг</span><span class="sxs-lookup"><span data-stu-id="e4871-132">Thursday</span></span>    
- <span data-ttu-id="e4871-133">Пятница</span><span class="sxs-lookup"><span data-stu-id="e4871-133">Friday</span></span>    
- <span data-ttu-id="e4871-134">Суббота</span><span class="sxs-lookup"><span data-stu-id="e4871-134">Saturday</span></span>    
- <span data-ttu-id="e4871-135">Day</span><span class="sxs-lookup"><span data-stu-id="e4871-135">Day</span></span>    
- <span data-ttu-id="e4871-136">День недели</span><span class="sxs-lookup"><span data-stu-id="e4871-136">Weekday</span></span>   
- <span data-ttu-id="e4871-137">викенддай</span><span class="sxs-lookup"><span data-stu-id="e4871-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="e4871-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4871-138">Remarks</span></span>

<span data-ttu-id="e4871-139">Элемент [StandardTime](standardtime.md) , содержащий элемент [дайордер](dayorder.md) , который имеет значение 5, элемент [Month](month.md) со значением 10, а элемент **DayOfWeek** со значением Sunday означает, что переход со стандартного времени на летнее время происходит в пятое воскресенье десятого месяца.</span><span class="sxs-lookup"><span data-stu-id="e4871-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="e4871-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e4871-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4871-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e4871-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4871-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e4871-142">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4871-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e4871-143">Schema Name</span></span>  <br/> |<span data-ttu-id="e4871-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e4871-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4871-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e4871-145">Validation File</span></span>  <br/> |<span data-ttu-id="e4871-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e4871-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4871-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e4871-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4871-148">False</span><span class="sxs-lookup"><span data-stu-id="e4871-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4871-149">См. также</span><span class="sxs-lookup"><span data-stu-id="e4871-149">See also</span></span>

- [<span data-ttu-id="e4871-150">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e4871-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e4871-151">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e4871-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

