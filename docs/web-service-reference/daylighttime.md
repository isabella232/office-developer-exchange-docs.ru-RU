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
description: Элемент DaylightTime представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом смещения (UTC) в регионах, где наблюдается летнее время. Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.
ms.openlocfilehash: 350fcb4ce278f423c62fcc5ecaa160eda71e4a2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455655"
---
# <a name="daylighttime"></a><span data-ttu-id="cbc1b-104">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="cbc1b-104">DaylightTime</span></span>

<span data-ttu-id="cbc1b-105">Элемент **DaylightTime** представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (](bias-utc.md) UTC) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-105">The **DaylightTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="cbc1b-106">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-106">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span> 
  
- [<span data-ttu-id="cbc1b-107">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="cbc1b-107">TimeZone (Availability)</span></span>](timezone-availability.md) 
- [<span data-ttu-id="cbc1b-108">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="cbc1b-108">DaylightTime</span></span>](daylighttime.md)
  
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

<span data-ttu-id="cbc1b-109">**сериализаблетимезонетиме**</span><span class="sxs-lookup"><span data-stu-id="cbc1b-109">**SerializableTimeZoneTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cbc1b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cbc1b-110">Attributes and elements</span></span>

<span data-ttu-id="cbc1b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbc1b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cbc1b-112">Attributes</span></span>

<span data-ttu-id="cbc1b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbc1b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cbc1b-114">Child elements</span></span>

|<span data-ttu-id="cbc1b-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cbc1b-115">**Element**</span></span>|<span data-ttu-id="cbc1b-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cbc1b-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbc1b-117">Bias</span><span class="sxs-lookup"><span data-stu-id="cbc1b-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="cbc1b-118">Представляет смещение относительно времени в формате UTC, которое определено элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="cbc1b-119">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="cbc1b-120">Time</span><span class="sxs-lookup"><span data-stu-id="cbc1b-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="cbc1b-121">Представляет время перехода на зимнее и зимнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="cbc1b-122">дайордер</span><span class="sxs-lookup"><span data-stu-id="cbc1b-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="cbc1b-123">Представляет _n_th день недели, указанный в элементе [DayOfWeek (TimeZone)](dayofweek-timezone.md) , который представляет дату перехода со стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="cbc1b-124">Month</span><span class="sxs-lookup"><span data-stu-id="cbc1b-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="cbc1b-125">Представляет переходный месяц года от стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="cbc1b-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="cbc1b-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="cbc1b-127">Представляет день недели, когда происходит переход на зимнее и зимнее время и на летнее время.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="cbc1b-128">Год</span><span class="sxs-lookup"><span data-stu-id="cbc1b-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="cbc1b-129">Используется для определения часового пояса, который изменяется в зависимости от года.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-129">Used to define a time zone that changes depending on the year.</span></span> <span data-ttu-id="cbc1b-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-130">This element is optional.</span></span> <span data-ttu-id="cbc1b-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="cbc1b-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cbc1b-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cbc1b-132">Parent elements</span></span>

|<span data-ttu-id="cbc1b-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cbc1b-133">**Element**</span></span>|<span data-ttu-id="cbc1b-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cbc1b-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbc1b-135">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="cbc1b-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="cbc1b-136">Содержит элементы, определяющие сведения о часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-136">Contains elements that identify time zone information.</span></span><br/><br/><span data-ttu-id="cbc1b-137">Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-137">This element also contains information about the transition between standard time and daylight saving time.</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a><span data-ttu-id="cbc1b-138">Пример</span><span class="sxs-lookup"><span data-stu-id="cbc1b-138">Example</span></span>

<span data-ttu-id="cbc1b-139">Следующий частичный запрос GetUserAvailability представляет клиентское приложение в расположении, которое распознает летнее время.</span><span class="sxs-lookup"><span data-stu-id="cbc1b-139">The following partial GetUserAvailability request represents a client application in a location that recognizes daylight saving time.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="cbc1b-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cbc1b-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbc1b-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cbc1b-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbc1b-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cbc1b-142">Schema Name</span></span>  <br/> |<span data-ttu-id="cbc1b-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cbc1b-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbc1b-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cbc1b-144">Validation File</span></span>  <br/> |<span data-ttu-id="cbc1b-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cbc1b-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbc1b-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cbc1b-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="cbc1b-147">False</span><span class="sxs-lookup"><span data-stu-id="cbc1b-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbc1b-148">См. также</span><span class="sxs-lookup"><span data-stu-id="cbc1b-148">See also</span></span>

- [<span data-ttu-id="cbc1b-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cbc1b-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="cbc1b-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="cbc1b-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

