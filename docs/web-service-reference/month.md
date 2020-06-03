---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: Элемент month представляет переходный месяц года до зимнего времени и летнего времени.
ms.openlocfilehash: f102dca4ed9e833b9742844cfd612c81dfd05e70
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468623"
---
# <a name="month"></a><span data-ttu-id="7cf82-103">Month</span><span class="sxs-lookup"><span data-stu-id="7cf82-103">Month</span></span>

<span data-ttu-id="7cf82-104">Элемент **Month** представляет переходный месяц года до зимнего времени и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="7cf82-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="7cf82-105">**Сроки**</span><span class="sxs-lookup"><span data-stu-id="7cf82-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7cf82-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7cf82-106">Attributes and elements</span></span>

<span data-ttu-id="7cf82-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7cf82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7cf82-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7cf82-108">Attributes</span></span>

<span data-ttu-id="7cf82-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7cf82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7cf82-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7cf82-110">Child elements</span></span>

<span data-ttu-id="7cf82-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7cf82-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7cf82-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7cf82-112">Parent elements</span></span>

|<span data-ttu-id="7cf82-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7cf82-113">**Element**</span></span>|<span data-ttu-id="7cf82-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7cf82-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7cf82-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="7cf82-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="7cf82-116">Представляет смещение относительно времени относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="7cf82-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="7cf82-117">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="7cf82-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="7cf82-118">Ниже приведены выражения XPath для элемента [StandardTime](standardtime.md) :</span><span class="sxs-lookup"><span data-stu-id="7cf82-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="7cf82-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="7cf82-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="7cf82-120">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="7cf82-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="7cf82-121">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="7cf82-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="7cf82-122">Ниже приведены выражения XPath для элемента [DaylightTime](daylighttime.md) :</span><span class="sxs-lookup"><span data-stu-id="7cf82-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7cf82-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="7cf82-123">Text value</span></span>

<span data-ttu-id="7cf82-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="7cf82-124">A text value is required.</span></span> <span data-ttu-id="7cf82-125">Значение представляет порядковый номер месяца по порядку повторения и должно быть числом от 1 до 12.</span><span class="sxs-lookup"><span data-stu-id="7cf82-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="7cf82-126">Это тип данных Short Integer.</span><span class="sxs-lookup"><span data-stu-id="7cf82-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7cf82-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="7cf82-127">Remarks</span></span>

<span data-ttu-id="7cf82-128">Элемент [StandardTime](standardtime.md) , содержащий элемент [дайордер](dayorder.md) , который имеет значение 5, элемент **Month** со значением 10, и элемент [DayOfWeek (TimeZone)](dayofweek-timezone.md) , имеющий значение воскресенье, означает, что переход со стандартного времени на летнее время приходится на пятое воскресенье десятого месяца.</span><span class="sxs-lookup"><span data-stu-id="7cf82-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="7cf82-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7cf82-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7cf82-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7cf82-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7cf82-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7cf82-131">Schema Name</span></span>  <br/> |<span data-ttu-id="7cf82-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7cf82-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="7cf82-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7cf82-133">Validation File</span></span>  <br/> |<span data-ttu-id="7cf82-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="7cf82-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7cf82-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7cf82-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="7cf82-136">False</span><span class="sxs-lookup"><span data-stu-id="7cf82-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7cf82-137">См. также</span><span class="sxs-lookup"><span data-stu-id="7cf82-137">See also</span></span>

- [<span data-ttu-id="7cf82-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7cf82-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="7cf82-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="7cf82-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

