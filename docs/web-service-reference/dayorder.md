---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: Элемент DayOrder представляет n-й вхождения день, заданный в элемент DayOfWeek (часовой пояс), который представляет дату перехода и зимнего и летнего времени.
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761998"
---
# <a name="dayorder"></a><span data-ttu-id="80196-103">DayOrder</span><span class="sxs-lookup"><span data-stu-id="80196-103">DayOrder</span></span>

<span data-ttu-id="80196-104">Элемент **DayOrder** представляет вхождение _n_th день, заданный в элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который представляет дату перехода и зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="80196-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="80196-105">**короткие**</span><span class="sxs-lookup"><span data-stu-id="80196-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="80196-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80196-106">Attributes and elements</span></span>

<span data-ttu-id="80196-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="80196-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80196-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80196-108">Attributes</span></span>

<span data-ttu-id="80196-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="80196-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80196-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80196-110">Child elements</span></span>

<span data-ttu-id="80196-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="80196-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80196-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80196-112">Parent elements</span></span>

|<span data-ttu-id="80196-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80196-113">**Element**</span></span>|<span data-ttu-id="80196-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80196-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80196-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="80196-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="80196-116">Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="80196-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="80196-117">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="80196-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="80196-118">Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) .</span><span class="sxs-lookup"><span data-stu-id="80196-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="80196-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="80196-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="80196-120">Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="80196-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="80196-121">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="80196-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="80196-122">Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .</span><span class="sxs-lookup"><span data-stu-id="80196-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80196-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="80196-123">Text value</span></span>

<span data-ttu-id="80196-124">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="80196-124">A text value is required.</span></span> <span data-ttu-id="80196-125">Значение для элемента **DayOrder** может быть от 1 до 5.</span><span class="sxs-lookup"><span data-stu-id="80196-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="80196-126">Максимальное значение для этого элемента может быть 4 и 5, в зависимости от того, месяц и год.</span><span class="sxs-lookup"><span data-stu-id="80196-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="80196-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="80196-127">Remarks</span></span>

<span data-ttu-id="80196-128">Элемент [StandardTime](standardtime.md) , который содержит элемент **DayOrder** , который имеет значение 5, [месяц](month.md) , который имеет значение 10 и элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который имеет значение воскресенье означает, что переход к летнее время выполняется на пятом воскресенье десятой месяца.</span><span class="sxs-lookup"><span data-stu-id="80196-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="80196-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="80196-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="80196-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="80196-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="80196-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="80196-131">Schema Name</span></span>  <br/> |<span data-ttu-id="80196-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="80196-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="80196-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="80196-133">Validation File</span></span>  <br/> |<span data-ttu-id="80196-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="80196-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="80196-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="80196-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="80196-136">False</span><span class="sxs-lookup"><span data-stu-id="80196-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="80196-137">См. также</span><span class="sxs-lookup"><span data-stu-id="80196-137">See also</span></span>

- [<span data-ttu-id="80196-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="80196-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="80196-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="80196-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

