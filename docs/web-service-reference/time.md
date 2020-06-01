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
description: Элемент Time представляет время перехода суток до стандартного и летнего времени.
ms.openlocfilehash: 97c89fbcbdb85fcdd4d32a1d44075ac42adef053
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460297"
---
# <a name="time"></a><span data-ttu-id="49a0f-103">Time</span><span class="sxs-lookup"><span data-stu-id="49a0f-103">Time</span></span>

<span data-ttu-id="49a0f-104">Элемент **time** представляет время перехода суток до стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="49a0f-104">The **Time** element represents the transition time of day to and from standard time and daylight saving time.</span></span> 
  
```xml
<Time>...</Time>
```

 <span data-ttu-id="49a0f-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="49a0f-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49a0f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49a0f-106">Attributes and elements</span></span>

<span data-ttu-id="49a0f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="49a0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49a0f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49a0f-108">Attributes</span></span>

<span data-ttu-id="49a0f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49a0f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49a0f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49a0f-110">Child elements</span></span>

<span data-ttu-id="49a0f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49a0f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49a0f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49a0f-112">Parent elements</span></span>

|<span data-ttu-id="49a0f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49a0f-113">**Element**</span></span>|<span data-ttu-id="49a0f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49a0f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49a0f-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="49a0f-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="49a0f-116">Представляет смещение относительно времени относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="49a0f-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="49a0f-117">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="49a0f-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/><br/>  <span data-ttu-id="49a0f-118">Ниже приведены выражения XPath для элемента [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="49a0f-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="49a0f-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="49a0f-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="49a0f-120">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="49a0f-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="49a0f-121">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="49a0f-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="49a0f-122">Ниже приведены выражения XPath для элемента [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="49a0f-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49a0f-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="49a0f-123">Text value</span></span>

<span data-ttu-id="49a0f-124">Текстовое значение представляет часы, минуты и секунды в следующем формате: чч: мм: СС.</span><span class="sxs-lookup"><span data-stu-id="49a0f-124">The text value represents hours, minutes, and seconds in the following format: hh:mm:ss.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49a0f-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="49a0f-125">Remarks</span></span>

<span data-ttu-id="49a0f-126">Когда элемент **time** встречается в элементе [DaylightTime](daylighttime.md) , он представляет время суток, когда происходит переход с летнего на зимнее время.</span><span class="sxs-lookup"><span data-stu-id="49a0f-126">When the **Time** element occurs in the [DaylightTime](daylighttime.md) element, it represents the time of day that the transition from daylight saving time to standard time occurs.</span></span> <span data-ttu-id="49a0f-127">Когда элемент [time](time.md) встречается в элементе [StandardTime](standardtime.md) , он представляет время суток, когда происходит переход со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="49a0f-127">When the [Time](time.md) element occurs in the [StandardTime](standardtime.md) element, it represents the time of day that the transition from standard time to daylight saving time occurs.</span></span> 
  
<span data-ttu-id="49a0f-128">Этот элемент имеет минимальное нулевое значение и максимальное число вхождений 1.</span><span class="sxs-lookup"><span data-stu-id="49a0f-128">This element has a minimum occurrence of zero and a maximum occurrence of one.</span></span>
  
## <a name="example"></a><span data-ttu-id="49a0f-129">Пример</span><span class="sxs-lookup"><span data-stu-id="49a0f-129">Example</span></span>

<span data-ttu-id="49a0f-130">Следующая часть запроса представляет время перехода в 2 часа утра.</span><span class="sxs-lookup"><span data-stu-id="49a0f-130">The following part of a request represents a transition time of 2 A.M.</span></span> <span data-ttu-id="49a0f-131">со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="49a0f-131">from standard time to daylight saving time.</span></span>
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

## <a name="element-information"></a><span data-ttu-id="49a0f-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49a0f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49a0f-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49a0f-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49a0f-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49a0f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="49a0f-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="49a0f-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="49a0f-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49a0f-136">Validation File</span></span>  <br/> |<span data-ttu-id="49a0f-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="49a0f-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49a0f-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49a0f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="49a0f-139">False</span><span class="sxs-lookup"><span data-stu-id="49a0f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49a0f-140">См. также</span><span class="sxs-lookup"><span data-stu-id="49a0f-140">See also</span></span>

- [<span data-ttu-id="49a0f-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="49a0f-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="49a0f-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="49a0f-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

