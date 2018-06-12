---
title: Часовой пояс (доступность)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: Элемент TimeZone содержит элементы, чтобы указать часовой пояс сведения. Этот элемент также содержит сведения о переходе между зимнего и летнего времени.
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840205"
---
# <a name="timezone-availability"></a><span data-ttu-id="85f2c-104">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="85f2c-104">TimeZone (Availability)</span></span>

<span data-ttu-id="85f2c-105">Элемент **TimeZone** содержит элементы, чтобы указать часовой пояс сведения.</span><span class="sxs-lookup"><span data-stu-id="85f2c-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="85f2c-106">Этот элемент также содержит сведения о переходе между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="85f2c-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="85f2c-107">**SerializableTimeZone**</span><span class="sxs-lookup"><span data-stu-id="85f2c-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85f2c-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="85f2c-108">Attributes and elements</span></span>

<span data-ttu-id="85f2c-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="85f2c-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85f2c-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="85f2c-110">Attributes</span></span>

<span data-ttu-id="85f2c-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="85f2c-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85f2c-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="85f2c-112">Child elements</span></span>

|<span data-ttu-id="85f2c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85f2c-113">**Element**</span></span>|<span data-ttu-id="85f2c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85f2c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85f2c-115">Смещение (UTC)</span><span class="sxs-lookup"><span data-stu-id="85f2c-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="85f2c-116">Представляет общие смещение в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="85f2c-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="85f2c-117">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="85f2c-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="85f2c-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="85f2c-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="85f2c-119">Представляет смещение от времени относительно UTC, представленный в элемент [Bias (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="85f2c-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="85f2c-120">Этот элемент также содержит сведения о переходе стандартного времени на летнее время в областях, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="85f2c-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="85f2c-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="85f2c-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="85f2c-122">Представляет смещение от времени относительно UTC, представленный элемент [Bias (UTC)](bias-utc.md) в области, где наблюдается летнего времени.</span><span class="sxs-lookup"><span data-stu-id="85f2c-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="85f2c-123">Этот элемент также содержит сведения о когда происходит переход на летнее время.</span><span class="sxs-lookup"><span data-stu-id="85f2c-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85f2c-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="85f2c-124">Parent elements</span></span>

|<span data-ttu-id="85f2c-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85f2c-125">**Element**</span></span>|<span data-ttu-id="85f2c-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85f2c-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85f2c-127">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="85f2c-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="85f2c-128">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="85f2c-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="85f2c-129">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="85f2c-129">This is a root element.</span></span>  <br/> <span data-ttu-id="85f2c-130">Элемент **TimeZone** в сообщении GetUserAvailabilityRequest представляет часовой пояс, в котором указаны значения даты и времени в запросе.</span><span class="sxs-lookup"><span data-stu-id="85f2c-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="85f2c-131">Значения даты и времени, возвращаемые службы доступности могут также в данном часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="85f2c-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="85f2c-132">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="85f2c-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="85f2c-133">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="85f2c-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="85f2c-134">Представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="85f2c-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="85f2c-135">Элемент **TimeZone** в сообщении GetUserAvailabilityResponse представляет параметры часового пояса запрошенные почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="85f2c-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="85f2c-136">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="85f2c-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85f2c-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="85f2c-137">Remarks</span></span>

<span data-ttu-id="85f2c-138">Этот элемент является обязательным в элементе [GetUserAvailabilityRequest](getuseravailabilityrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="85f2c-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="85f2c-139">Этот элемент возникает только один раз или по крайней мере ноль раз при родительский элемент представляет собой элемент [WorkingHours](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="85f2c-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="85f2c-140">Пример</span><span class="sxs-lookup"><span data-stu-id="85f2c-140">Example</span></span>

<span data-ttu-id="85f2c-141">Следующий пример показывает часть запроса XML, который определяет смещение времени в формате UTC 8 часов в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="85f2c-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="85f2c-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="85f2c-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85f2c-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="85f2c-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85f2c-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="85f2c-144">Schema Name</span></span>  <br/> |<span data-ttu-id="85f2c-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="85f2c-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="85f2c-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="85f2c-146">Validation File</span></span>  <br/> |<span data-ttu-id="85f2c-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85f2c-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85f2c-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="85f2c-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="85f2c-149">False</span><span class="sxs-lookup"><span data-stu-id="85f2c-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85f2c-150">См. также</span><span class="sxs-lookup"><span data-stu-id="85f2c-150">See also</span></span>



[<span data-ttu-id="85f2c-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="85f2c-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="85f2c-152">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="85f2c-152">Bias</span></span>](bias.md)


[<span data-ttu-id="85f2c-153">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="85f2c-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

