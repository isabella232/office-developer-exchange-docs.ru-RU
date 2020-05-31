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
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761993"
---
# <a name="dayofweek-timezone"></a><span data-ttu-id="dac38-103">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="dac38-103">DayOfWeek (TimeZone)</span></span>

<span data-ttu-id="dac38-104">Элемент **DayOfWeek** представляет день недели, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="dac38-104">The **DayOfWeek** element represents the day of the week on which the time zone transition occurs.</span></span> 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

<span data-ttu-id="dac38-105">**дайофвиктипе**</span><span class="sxs-lookup"><span data-stu-id="dac38-105">**DayOfWeekType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dac38-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dac38-106">Attributes and elements</span></span>

<span data-ttu-id="dac38-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dac38-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dac38-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dac38-108">Attributes</span></span>

<span data-ttu-id="dac38-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dac38-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dac38-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dac38-110">Child elements</span></span>

<span data-ttu-id="dac38-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="dac38-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dac38-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dac38-112">Parent elements</span></span>

|<span data-ttu-id="dac38-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dac38-113">**Element**</span></span>|<span data-ttu-id="dac38-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dac38-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dac38-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="dac38-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="dac38-116">Представляет смещение относительно времени относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="dac38-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="dac38-117">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="dac38-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="dac38-118">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="dac38-118">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="dac38-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="dac38-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="dac38-120">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="dac38-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="dac38-121">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="dac38-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="dac38-122">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="dac38-122">The following are the XPath expressions to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[<span data-ttu-id="dac38-123">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="dac38-123">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="dac38-124">Представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="dac38-124">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dac38-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dac38-125">Text value</span></span>

<span data-ttu-id="dac38-126">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="dac38-126">A text value is required.</span></span> <span data-ttu-id="dac38-127">Текстовое значение представлено перечислением со следующими возможными значениями:</span><span class="sxs-lookup"><span data-stu-id="dac38-127">The text value is represented by an enumeration that has the following possible values:</span></span>
  
- <span data-ttu-id="dac38-128">Воскресеньям</span><span class="sxs-lookup"><span data-stu-id="dac38-128">Sunday</span></span>    
- <span data-ttu-id="dac38-129">Понедельник</span><span class="sxs-lookup"><span data-stu-id="dac38-129">Monday</span></span>    
- <span data-ttu-id="dac38-130">Вторник</span><span class="sxs-lookup"><span data-stu-id="dac38-130">Tuesday</span></span>    
- <span data-ttu-id="dac38-131">Среда</span><span class="sxs-lookup"><span data-stu-id="dac38-131">Wednesday</span></span>    
- <span data-ttu-id="dac38-132">Четверг</span><span class="sxs-lookup"><span data-stu-id="dac38-132">Thursday</span></span>    
- <span data-ttu-id="dac38-133">Пятница</span><span class="sxs-lookup"><span data-stu-id="dac38-133">Friday</span></span>    
- <span data-ttu-id="dac38-134">Суббота</span><span class="sxs-lookup"><span data-stu-id="dac38-134">Saturday</span></span>    
- <span data-ttu-id="dac38-135">Day</span><span class="sxs-lookup"><span data-stu-id="dac38-135">Day</span></span>    
- <span data-ttu-id="dac38-136">День недели</span><span class="sxs-lookup"><span data-stu-id="dac38-136">Weekday</span></span>   
- <span data-ttu-id="dac38-137">викенддай</span><span class="sxs-lookup"><span data-stu-id="dac38-137">WeekendDay</span></span>
    
## <a name="remarks"></a><span data-ttu-id="dac38-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="dac38-138">Remarks</span></span>

<span data-ttu-id="dac38-139">Элемент [StandardTime](standardtime.md) , содержащий элемент [дайордер](dayorder.md) , который имеет значение 5, элемент [Month](month.md) со значением 10, а элемент **DayOfWeek** со значением Sunday означает, что переход со стандартного времени на летнее время происходит в пятое воскресенье десятого месяца.</span><span class="sxs-lookup"><span data-stu-id="dac38-139">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a [Month](month.md) element that has a value of 10, and a **DayOfWeek** element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
<span data-ttu-id="dac38-140">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="dac38-140">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dac38-141">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dac38-141">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dac38-142">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dac38-142">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dac38-143">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dac38-143">Schema Name</span></span>  <br/> |<span data-ttu-id="dac38-144">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dac38-144">Types schema</span></span>  <br/> |
|<span data-ttu-id="dac38-145">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dac38-145">Validation File</span></span>  <br/> |<span data-ttu-id="dac38-146">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dac38-146">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dac38-147">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dac38-147">Can be Empty</span></span>  <br/> |<span data-ttu-id="dac38-148">False</span><span class="sxs-lookup"><span data-stu-id="dac38-148">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dac38-149">См. также</span><span class="sxs-lookup"><span data-stu-id="dac38-149">See also</span></span>

- [<span data-ttu-id="dac38-150">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dac38-150">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="dac38-151">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="dac38-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

