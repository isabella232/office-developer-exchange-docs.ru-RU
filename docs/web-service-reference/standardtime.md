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
description: Элемент StandardTime представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом смещения (UTC). Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456404"
---
# <a name="standardtime"></a><span data-ttu-id="f8a9e-104">StandardTime</span><span class="sxs-lookup"><span data-stu-id="f8a9e-104">StandardTime</span></span>

<span data-ttu-id="f8a9e-105">Элемент **StandardTime** представляет смещение относительно времени относительно времени в формате UTC, которое представлено элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f8a9e-105">The **StandardTime** element represents an offset from the time relative to Coordinated Universal Time (UTC) that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="f8a9e-106">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-106">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> 
  
- [<span data-ttu-id="f8a9e-107">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="f8a9e-107">TimeZone (Availability)</span></span>](timezone-availability.md)
- [<span data-ttu-id="f8a9e-108">StandardTime</span><span class="sxs-lookup"><span data-stu-id="f8a9e-108">StandardTime</span></span>](standardtime.md)
  
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

 <span data-ttu-id="f8a9e-109">**сериализаблетимезонетиме**</span><span class="sxs-lookup"><span data-stu-id="f8a9e-109">**SerializableTimeZoneTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8a9e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f8a9e-110">Attributes and elements</span></span>

<span data-ttu-id="f8a9e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8a9e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f8a9e-112">Attributes</span></span>

<span data-ttu-id="f8a9e-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8a9e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f8a9e-114">Child elements</span></span>

|<span data-ttu-id="f8a9e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f8a9e-115">**Element**</span></span>|<span data-ttu-id="f8a9e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8a9e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8a9e-117">Bias</span><span class="sxs-lookup"><span data-stu-id="f8a9e-117">Bias</span></span>](bias.md) <br/> |<span data-ttu-id="f8a9e-118">Представляет смещение относительно времени в формате UTC, которое определено элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-118">Represents the offset from the UTC offset that is identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="f8a9e-119">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-119">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="f8a9e-120">Time</span><span class="sxs-lookup"><span data-stu-id="f8a9e-120">Time</span></span>](time.md) <br/> |<span data-ttu-id="f8a9e-121">Представляет время перехода на зимнее и зимнее время и обратно.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-121">Represents the transition time of day to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f8a9e-122">дайордер</span><span class="sxs-lookup"><span data-stu-id="f8a9e-122">DayOrder</span></span>](dayorder.md) <br/> |<span data-ttu-id="f8a9e-123">Представляет _n_th день недели, указанный в элементе [DayOfWeek (TimeZone)](dayofweek-timezone.md) , который представляет дату перехода со стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-123">Represents the  _n_th occurrence of the day that is specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f8a9e-124">Month</span><span class="sxs-lookup"><span data-stu-id="f8a9e-124">Month</span></span>](month.md) <br/> |<span data-ttu-id="f8a9e-125">Представляет переходный месяц года от стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-125">Represents the transition month of the year to and from standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="f8a9e-126">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="f8a9e-126">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="f8a9e-127">Представляет день недели, когда происходит переход на зимнее и зимнее время и на летнее время.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-127">Represents the day of the week when the transition to and from standard time and daylight saving time occurs.</span></span>  <br/> |
|[<span data-ttu-id="f8a9e-128">Год</span><span class="sxs-lookup"><span data-stu-id="f8a9e-128">Year</span></span>](year.md) <br/> |<span data-ttu-id="f8a9e-129">Определяет часовой пояс, который изменяется в зависимости от года.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-129">Defines a time zone that changes depending on the year.</span></span> <span data-ttu-id="f8a9e-130">Этот элемент является необязательным.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-130">This element is optional.</span></span> <span data-ttu-id="f8a9e-131">Этот элемент появился в Exchange Server 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f8a9e-131">This element was introduced in Microsoft Exchange Server 2007 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8a9e-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f8a9e-132">Parent elements</span></span>

|<span data-ttu-id="f8a9e-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f8a9e-133">**Element**</span></span>|<span data-ttu-id="f8a9e-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f8a9e-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8a9e-135">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="f8a9e-135">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="f8a9e-136">Содержит элементы, определяющие сведения о часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-136">Contains elements that identify time zone information.</span></span> <span data-ttu-id="f8a9e-137">Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-137">This element also contains information about the transition between standard time and daylight saving time.</span></span> <br/><br/><span data-ttu-id="f8a9e-138">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-138">The following are the XPath expressions to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8a9e-139">Примечания</span><span class="sxs-lookup"><span data-stu-id="f8a9e-139">Remarks</span></span>

<span data-ttu-id="f8a9e-140">Элемент **StandardTime** представляет время смещения, представленное элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f8a9e-140">The **StandardTime** element represents an offset time that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="f8a9e-141">Если дочерний элемент [сдвига](bias.md) равен 0, стандартное время равно смещению смещения относительно времени в формате UTC, которое представлено элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="f8a9e-141">When the child [Bias](bias.md) element equals 0, the standard time is equal to the bias offset from UTC that is represented by the [Bias (UTC)](bias-utc.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="f8a9e-142">Пример</span><span class="sxs-lookup"><span data-stu-id="f8a9e-142">Example</span></span>

<span data-ttu-id="f8a9e-143">В следующем примере показан регион, в котором наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-143">The following example shows a region where daylight saving time is observed.</span></span> <span data-ttu-id="f8a9e-144">Переход с летнего на зимнее время выполняется в 2 часа утра.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-144">The transition from daylight saving time to standard time is observed at 2 A.M.</span></span> <span data-ttu-id="f8a9e-145">в пятом воскресенье десятого месяца.</span><span class="sxs-lookup"><span data-stu-id="f8a9e-145">on the fifth Sunday of the tenth month.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="f8a9e-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f8a9e-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8a9e-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f8a9e-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8a9e-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f8a9e-148">Schema Name</span></span>  <br/> |<span data-ttu-id="f8a9e-149">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f8a9e-149">Types schema</span></span>  <br/> |
|<span data-ttu-id="f8a9e-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f8a9e-150">Validation File</span></span>  <br/> |<span data-ttu-id="f8a9e-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f8a9e-151">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8a9e-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f8a9e-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="f8a9e-153">False</span><span class="sxs-lookup"><span data-stu-id="f8a9e-153">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f8a9e-154">См. также</span><span class="sxs-lookup"><span data-stu-id="f8a9e-154">See also</span></span>

- [<span data-ttu-id="f8a9e-155">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f8a9e-155">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="f8a9e-156">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f8a9e-156">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

