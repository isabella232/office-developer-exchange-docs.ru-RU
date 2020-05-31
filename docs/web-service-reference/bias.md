---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: Элемент offset представляет смещение от смещения относительно всеобщего скоординированного времени (UTC), определенного элементом смещения (UTC) для стандартного времени и летнего времени. Это значение представлено в минутах.
ms.openlocfilehash: 770bf97b030ac1293595560bc269f54896e35a15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761563"
---
# <a name="bias"></a><span data-ttu-id="69080-104">Bias</span><span class="sxs-lookup"><span data-stu-id="69080-104">Bias</span></span>

<span data-ttu-id="69080-105">Элемент **offset** представляет смещение от смещения относительно всеобщего скоординированного времени (UTC), определенного элементом [смещения (UTC)](bias-utc.md) для стандартного времени и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="69080-105">The **Bias** element represents the offset from the Coordinated Universal Time (UTC) offset identified by the [Bias (UTC)](bias-utc.md) element for standard time and daylight saving time.</span></span> <span data-ttu-id="69080-106">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="69080-106">This value is in minutes.</span></span> 
  
```xml
<Bias>...</Bias>
```

<span data-ttu-id="69080-107">**int**</span><span class="sxs-lookup"><span data-stu-id="69080-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="69080-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69080-108">Attributes and elements</span></span>

<span data-ttu-id="69080-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="69080-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69080-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69080-110">Attributes</span></span>

<span data-ttu-id="69080-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="69080-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69080-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69080-112">Child elements</span></span>

<span data-ttu-id="69080-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="69080-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69080-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69080-114">Parent elements</span></span>

|<span data-ttu-id="69080-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69080-115">**Element**</span></span>|<span data-ttu-id="69080-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69080-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69080-117">StandardTime</span><span class="sxs-lookup"><span data-stu-id="69080-117">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="69080-118">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="69080-118">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="69080-119">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="69080-119">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span><br/><br/><span data-ttu-id="69080-120">Ниже приведены выражения XPath для элемента [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="69080-120">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="69080-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="69080-121">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="69080-122">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="69080-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="69080-123">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="69080-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/><span data-ttu-id="69080-124">Ниже приведены выражения XPath для элемента [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="69080-124">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span><br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69080-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="69080-125">Text value</span></span>

<span data-ttu-id="69080-126">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="69080-126">A text value is required.</span></span> <span data-ttu-id="69080-127">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="69080-127">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69080-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="69080-128">Remarks</span></span>

<span data-ttu-id="69080-129">Смещение, используемое для определения локального времени, может быть предоставлено только одним из элементов **смещения** .</span><span class="sxs-lookup"><span data-stu-id="69080-129">The offset used to determine the local time can only be provided by one of the **Bias** elements.</span></span> <span data-ttu-id="69080-130">Сумма значений элемента сдвига, предоставляемого элементом [DaylightTime](daylighttime.md) или элементом [StandardTime](standardtime.md) , кроме элемента [смещения (UTC)](bias-utc.md) , определяет местное время.</span><span class="sxs-lookup"><span data-stu-id="69080-130">The sum of the values of the Bias element provided by the [DaylightTime](daylighttime.md) element or the [StandardTime](standardtime.md) element plus the [Bias (UTC)](bias-utc.md) element identifies the local time.</span></span> 
  
## <a name="example"></a><span data-ttu-id="69080-131">Пример</span><span class="sxs-lookup"><span data-stu-id="69080-131">Example</span></span>

<span data-ttu-id="69080-132">В приведенном ниже примере показана часть XML-запроса, определяющая пользователя, который следит за переходом на летнее время, путем корректировки смещения относительно времени в формате UTC на-60 минут.</span><span class="sxs-lookup"><span data-stu-id="69080-132">The following example shows part of an XML request that identifies a user who observes daylight saving time by adjusting the offset from UTC by -60 minutes.</span></span> <span data-ttu-id="69080-133">Это позволяет эффективно отменять смещение 420 минут от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="69080-133">This effectively makes the bias 420 minutes from UTC.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="69080-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69080-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69080-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69080-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69080-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69080-136">Schema Name</span></span>  <br/> |<span data-ttu-id="69080-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="69080-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="69080-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69080-138">Validation File</span></span>  <br/> |<span data-ttu-id="69080-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="69080-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69080-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69080-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="69080-141">False</span><span class="sxs-lookup"><span data-stu-id="69080-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69080-142">См. также</span><span class="sxs-lookup"><span data-stu-id="69080-142">See also</span></span>

- [<span data-ttu-id="69080-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="69080-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="69080-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="69080-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

