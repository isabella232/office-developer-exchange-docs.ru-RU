---
title: Месяц
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
description: Элемент Month представляет перехода месяц года между зимнего и летнего времени.
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834476"
---
# <a name="month"></a><span data-ttu-id="75bd9-103">Месяц</span><span class="sxs-lookup"><span data-stu-id="75bd9-103">Month</span></span>

<span data-ttu-id="75bd9-104">Элемент **Month** представляет перехода месяц года между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="75bd9-104">The **Month** element represents the transition month of the year to and from standard time and daylight saving time.</span></span> 
  
```xml
<Month>...</Month>
```

 <span data-ttu-id="75bd9-105">**Короткие**</span><span class="sxs-lookup"><span data-stu-id="75bd9-105">**Short**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75bd9-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75bd9-106">Attributes and elements</span></span>

<span data-ttu-id="75bd9-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="75bd9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75bd9-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75bd9-108">Attributes</span></span>

<span data-ttu-id="75bd9-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="75bd9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75bd9-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75bd9-110">Child elements</span></span>

<span data-ttu-id="75bd9-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="75bd9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75bd9-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75bd9-112">Parent elements</span></span>

|<span data-ttu-id="75bd9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75bd9-113">**Element**</span></span>|<span data-ttu-id="75bd9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75bd9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75bd9-115">StandardTime</span><span class="sxs-lookup"><span data-stu-id="75bd9-115">StandardTime</span></span>](standardtime.md) <br/> | <span data-ttu-id="75bd9-116">Представляет смещение от времени относительно времени в формате UTC представленный элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="75bd9-116">Represents an offset from the time relative to Coordinated Universal Time (UTC) represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="75bd9-117">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="75bd9-117">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span> <br/> <br/>  <span data-ttu-id="75bd9-118">Ниже приведены выражения XPath в элемент [StandardTime](standardtime.md) .</span><span class="sxs-lookup"><span data-stu-id="75bd9-118">The following are the XPath expressions to the [StandardTime](standardtime.md) element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[<span data-ttu-id="75bd9-119">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="75bd9-119">DaylightTime</span></span>](daylighttime.md) <br/> | <span data-ttu-id="75bd9-120">Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="75bd9-120">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="75bd9-121">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="75bd9-121">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/><br/>  <span data-ttu-id="75bd9-122">Ниже приведены выражения XPath в элемент [DaylightTime](daylighttime.md) .</span><span class="sxs-lookup"><span data-stu-id="75bd9-122">The following are the XPath expressions to the [DaylightTime](daylighttime.md) element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75bd9-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75bd9-123">Text value</span></span>

<span data-ttu-id="75bd9-124">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="75bd9-124">A text value is required.</span></span> <span data-ttu-id="75bd9-125">Значение представляет порядковый номер ранг месяца появления и должно быть числом между 1 и 12.</span><span class="sxs-lookup"><span data-stu-id="75bd9-125">The value represents the ordinal rank of the month by occurrence and must be a number between 1 and 12.</span></span> <span data-ttu-id="75bd9-126">Это тип данных короткое целое число.</span><span class="sxs-lookup"><span data-stu-id="75bd9-126">This is a short integer data type.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75bd9-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="75bd9-127">Remarks</span></span>

<span data-ttu-id="75bd9-128">Элемент [StandardTime](standardtime.md) , который содержит элемент [DayOrder](dayorder.md) , который имеет значение 5, **месяц** , который имеет значение 10 и элемент [DayOfWeek (часовой пояс)](dayofweek-timezone.md) , который имеет значение воскресенье означает, что переход к летнее время выполняется на пятом воскресенье десятой месяца.</span><span class="sxs-lookup"><span data-stu-id="75bd9-128">A [StandardTime](standardtime.md) element that contains a [DayOrder](dayorder.md) element that has a value of 5, a **Month** element that has a value of 10, and a [DayOfWeek (TimeZone)](dayofweek-timezone.md) element that has a value of Sunday means that the transition from standard time to daylight saving time occurs on the fifth Sunday of the tenth month.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="75bd9-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="75bd9-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75bd9-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="75bd9-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="75bd9-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="75bd9-131">Schema Name</span></span>  <br/> |<span data-ttu-id="75bd9-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="75bd9-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="75bd9-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="75bd9-133">Validation File</span></span>  <br/> |<span data-ttu-id="75bd9-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="75bd9-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="75bd9-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="75bd9-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="75bd9-136">False</span><span class="sxs-lookup"><span data-stu-id="75bd9-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75bd9-137">См. также</span><span class="sxs-lookup"><span data-stu-id="75bd9-137">See also</span></span>

- [<span data-ttu-id="75bd9-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="75bd9-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="75bd9-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="75bd9-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

