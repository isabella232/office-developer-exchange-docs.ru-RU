---
title: дайордер
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
description: Элемент Дайордер представляет n-й экземпляр дня, указанного в элементе DayOfWeek (TimeZone), представляющий дату перехода со стандартного и летнего времени.
ms.openlocfilehash: 53a8cb979bdb7aefead5623b4680f4c1a4ef5509
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526965"
---
# <a name="dayorder"></a><span data-ttu-id="51cff-103">дайордер</span><span class="sxs-lookup"><span data-stu-id="51cff-103">DayOrder</span></span>

<span data-ttu-id="51cff-104">Элемент **дайордер** представляет _n_th вхождение дня, указанного в элементе [DayOfWeek (TimeZone)](dayofweek-timezone.md) , который представляет дату перехода со стандартного и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="51cff-104">The **DayOrder** element represents the  _n_th occurrence of the day specified in the [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that represents the date of transition from and to standard time and daylight saving time.</span></span> 
  
```xml
<DayOrder>...</DayOrder>
```

<span data-ttu-id="51cff-105">**сроки**</span><span class="sxs-lookup"><span data-stu-id="51cff-105">**short**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="51cff-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="51cff-106">Attributes and elements</span></span>

<span data-ttu-id="51cff-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="51cff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51cff-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="51cff-108">Attributes</span></span>

<span data-ttu-id="51cff-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51cff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51cff-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="51cff-110">Child elements</span></span>

<span data-ttu-id="51cff-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="51cff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51cff-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="51cff-112">Parent elements</span></span>

|<span data-ttu-id="51cff-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="51cff-113">**Element**</span></span>|<span data-ttu-id="51cff-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="51cff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51cff-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="51cff-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="51cff-116">Представляет смещение относительно времени относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="51cff-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span><br/><br/><span data-ttu-id="51cff-117">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="51cff-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="51cff-118">Ниже приведены выражения XPath для элемента [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="51cff-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="51cff-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="51cff-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="51cff-120">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="51cff-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="51cff-121">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="51cff-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span><br/><br/><span data-ttu-id="51cff-122">Ниже приведены выражения XPath для элемента [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="51cff-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51cff-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="51cff-123">Text value</span></span>

<span data-ttu-id="51cff-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="51cff-124">A text value is required.</span></span> <span data-ttu-id="51cff-125">Значение для элемента **дайордер** может быть от 1 до 5.</span><span class="sxs-lookup"><span data-stu-id="51cff-125">The value for the **DayOrder** element can be 1 through 5.</span></span> <span data-ttu-id="51cff-126">Максимальное значение этого элемента может быть равно 4 или 5, в зависимости от месяца и года.</span><span class="sxs-lookup"><span data-stu-id="51cff-126">The maximum value for this element can be either 4 or 5, depending on the month and year.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="51cff-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="51cff-127">Remarks</span></span>

<span data-ttu-id="51cff-128">Элемент [StandardTime](standardtime.md) , содержащий элемент **дайордер** , который имеет значение 5, элемент [Month](month.md) со значением 10, и элемент [DayOfWeek (TimeZone)](dayofweek-timezone.md) , имеющий значение воскресенье, означает, что переход со стандартного времени на летнее время приходится на пятое воскресенье десятого месяца.</span><span class="sxs-lookup"><span data-stu-id="51cff-128">A [StandardTime](standardtime.md) element that contains a **DayOrder** element that has a value of 5, a [Month](month.md) element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="51cff-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="51cff-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51cff-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="51cff-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="51cff-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="51cff-131">Schema Name</span></span>  <br/> |<span data-ttu-id="51cff-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="51cff-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="51cff-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="51cff-133">Validation File</span></span>  <br/> |<span data-ttu-id="51cff-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="51cff-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="51cff-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="51cff-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="51cff-136">False</span><span class="sxs-lookup"><span data-stu-id="51cff-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51cff-137">См. также</span><span class="sxs-lookup"><span data-stu-id="51cff-137">See also</span></span>

- [<span data-ttu-id="51cff-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="51cff-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="51cff-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="51cff-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

