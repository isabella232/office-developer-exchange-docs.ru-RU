---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: Элемент DaylightTime представляет смещение от времени относительно времени в формате UTC, представленный элемент Bias (UTC) в области, где наблюдается летнего времени. Этот элемент также содержит сведения о когда происходит переход на летнее время.
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761992"
---
# <a name="daylighttime"></a><span data-ttu-id="6d5e1-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="6d5e1-104">DaylightTime</span></span>

<span data-ttu-id="6d5e1-105">Элемент **DaylightTime** представляет смещение от времени относительно времени в формате UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="6d5e1-106">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="6d5e1-107">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="6d5e1-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="6d5e1-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="6d5e1-108">DaylightTime</span></span>](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
```

<span data-ttu-id="6d5e1-109">**SerializableTimeZoneTime**</span><span class="sxs-lookup"><span data-stu-id="6d5e1-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6d5e1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6d5e1-110">Attributes and elements</span></span>

<span data-ttu-id="6d5e1-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6d5e1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6d5e1-112">Attributes</span></span>

<span data-ttu-id="6d5e1-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6d5e1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6d5e1-114">Child elements</span></span>

|<span data-ttu-id="6d5e1-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d5e1-115">**Element**</span></span>|<span data-ttu-id="6d5e1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d5e1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d5e1-117">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="6d5e1-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="6d5e1-118">Представляет смещение из времени UTC, который идентифицируется средством элемент [Bias (UTC)](bias-utc.md) для зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="6d5e1-119">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="6d5e1-120">Time</span><span class="sxs-lookup"><span data-stu-id="6d5e1-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="6d5e1-121">Представляет время перехода между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6d5e1-122">DayOrder</span><span class="sxs-lookup"><span data-stu-id="6d5e1-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="6d5e1-123">Представляет _n_th вхождения день, указанный в элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который представляет дату перехода и зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6d5e1-124">Месяц</span><span class="sxs-lookup"><span data-stu-id="6d5e1-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="6d5e1-125">Представляет перехода месяц года между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="6d5e1-126">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="6d5e1-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="6d5e1-127">Представляет день недели, когда происходит переход на и с зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="6d5e1-128">Год</span><span class="sxs-lookup"><span data-stu-id="6d5e1-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="6d5e1-129">Используется для определения часового пояса, который изменяется в зависимости от года.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="6d5e1-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-130">This element is optional.</span></span> <span data-ttu-id="6d5e1-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6d5e1-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6d5e1-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6d5e1-132">Parent elements</span></span>

|<span data-ttu-id="6d5e1-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6d5e1-133">**Element**</span></span>|<span data-ttu-id="6d5e1-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6d5e1-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6d5e1-135">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="6d5e1-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="6d5e1-136">Содержит элементы, чтобы указать часовой пояс сведения.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="6d5e1-137">Этот элемент также содержит сведения о переходе между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="6d5e1-138">Пример</span><span class="sxs-lookup"><span data-stu-id="6d5e1-138">Example</span></span>

<span data-ttu-id="6d5e1-139">Следующие частичный запрос GetUserAvailability представляет клиентского приложения в расположение, распознаваемое летнего времени.</span><span class="sxs-lookup"><span data-stu-id="6d5e1-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="6d5e1-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6d5e1-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6d5e1-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6d5e1-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6d5e1-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6d5e1-142">Schema Name</span></span>  <br/> |<span data-ttu-id="6d5e1-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6d5e1-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="6d5e1-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6d5e1-144">Validation File</span></span>  <br/> |<span data-ttu-id="6d5e1-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6d5e1-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6d5e1-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6d5e1-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="6d5e1-147">False</span><span class="sxs-lookup"><span data-stu-id="6d5e1-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6d5e1-148">См. также</span><span class="sxs-lookup"><span data-stu-id="6d5e1-148">See also</span></span>

- [<span data-ttu-id="6d5e1-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6d5e1-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="6d5e1-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="6d5e1-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

