---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: Элемент StandardTime представляет смещение от времени относительно времени в формате UTC, представленный в элемент Bias (UTC). Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.
ms.openlocfilehash: 726c31ffba06c1c437711b88444ec5eba45b520d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835546"
---
# <a name="standardtime"></a><span data-ttu-id="f99ff-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="f99ff-104">StandardTime</span></span>

<span data-ttu-id="f99ff-105">Элемент **StandardTime** представляет смещение от времени относительно времени в формате UTC, представленный в элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f99ff-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="f99ff-106">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="f99ff-107">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="f99ff-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="f99ff-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="f99ff-108">StandardTime</span></span>](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 <span data-ttu-id="f99ff-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="f99ff-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f99ff-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f99ff-110">Attributes and elements</span></span>

<span data-ttu-id="f99ff-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f99ff-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f99ff-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f99ff-112">Attributes</span></span>

<span data-ttu-id="f99ff-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="f99ff-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f99ff-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f99ff-114">Child elements</span></span>

|<span data-ttu-id="f99ff-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f99ff-115">**Element**</span></span>|<span data-ttu-id="f99ff-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f99ff-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f99ff-117">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="f99ff-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="f99ff-118">Представляет смещение из времени UTC, который идентифицируется средством элемент [Bias (UTC)](bias-utc.md) для зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="f99ff-119">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="f99ff-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="f99ff-120">Time</span><span class="sxs-lookup"><span data-stu-id="f99ff-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="f99ff-121">Представляет время перехода между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f99ff-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="f99ff-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="f99ff-123">Представляет _n_th вхождения день, указанный в элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который представляет дату перехода и зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f99ff-124">Месяц</span><span class="sxs-lookup"><span data-stu-id="f99ff-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="f99ff-125">Представляет перехода месяц года между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f99ff-126">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="f99ff-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="f99ff-127">Представляет день недели, когда происходит переход на и с зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="f99ff-128">Год</span><span class="sxs-lookup"><span data-stu-id="f99ff-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="f99ff-129">Определяет часовой пояс, который изменяется в зависимости от года.</span><span class="sxs-lookup"><span data-stu-id="f99ff-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="f99ff-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f99ff-130">This element is optional.</span></span> <span data-ttu-id="f99ff-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f99ff-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f99ff-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f99ff-132">Parent elements</span></span>

|<span data-ttu-id="f99ff-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f99ff-133">**Element**</span></span>|<span data-ttu-id="f99ff-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f99ff-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f99ff-135">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="f99ff-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="f99ff-136">Содержит элементы, чтобы указать часовой пояс сведения.</span><span class="sxs-lookup"><span data-stu-id="f99ff-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="f99ff-137">Этот элемент также содержит сведения о переходе между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="f99ff-138">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f99ff-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f99ff-139">Замечания</span><span class="sxs-lookup"><span data-stu-id="f99ff-139">Remarks</span></span>

<span data-ttu-id="f99ff-140">Элемент **StandardTime** представляет смещения времени, которая представляется элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f99ff-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="f99ff-141">Если дочерний элемент [Bias](bias.md) равно 0, стандартное время равно некоторым смещением от времени UTC, представленный в элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f99ff-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="f99ff-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f99ff-142">Example</span></span>

<span data-ttu-id="f99ff-143">В следующем примере показано область, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f99ff-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="f99ff-144">Наблюдаемое осуществляется переход на летнее время в 2: 00.</span><span class="sxs-lookup"><span data-stu-id="f99ff-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="f99ff-145">на пятом воскресенье десятой месяца.</span><span class="sxs-lookup"><span data-stu-id="f99ff-145">on the fifth Sunday of the tenth month.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="f99ff-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f99ff-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f99ff-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f99ff-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f99ff-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f99ff-148">Schema Name</span></span>  <br/> |<span data-ttu-id="f99ff-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f99ff-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="f99ff-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f99ff-150">Validation File</span></span>  <br/> |<span data-ttu-id="f99ff-151">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f99ff-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f99ff-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f99ff-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="f99ff-153">False</span><span class="sxs-lookup"><span data-stu-id="f99ff-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f99ff-154">См. также</span><span class="sxs-lookup"><span data-stu-id="f99ff-154">See also</span></span>

- [<span data-ttu-id="f99ff-155">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f99ff-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="f99ff-156">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f99ff-156">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

