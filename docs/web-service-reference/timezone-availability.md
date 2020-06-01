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
description: Элемент TimeZone содержит элементы, определяющие сведения о часовом поясе. Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460276"
---
# <a name="timezone-availability"></a><span data-ttu-id="3b0de-104">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="3b0de-104">TimeZone (Availability)</span></span>

<span data-ttu-id="3b0de-105">Элемент **TimeZone** содержит элементы, определяющие сведения о часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="3b0de-105">The **TimeZone** element contains elements that identify time zone information.</span></span> <span data-ttu-id="3b0de-106">Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="3b0de-106">This element also contains information about the transition between standard time and daylight saving time.</span></span> 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 <span data-ttu-id="3b0de-107">**сериализаблетимезоне**</span><span class="sxs-lookup"><span data-stu-id="3b0de-107">**SerializableTimeZone**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b0de-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b0de-108">Attributes and elements</span></span>

<span data-ttu-id="3b0de-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3b0de-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b0de-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b0de-110">Attributes</span></span>

<span data-ttu-id="3b0de-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3b0de-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b0de-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b0de-112">Child elements</span></span>

|<span data-ttu-id="3b0de-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b0de-113">**Element**</span></span>|<span data-ttu-id="3b0de-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b0de-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b0de-115">Сдвиг (UTC)</span><span class="sxs-lookup"><span data-stu-id="3b0de-115">Bias (UTC)</span></span>](bias-utc.md) <br/> |<span data-ttu-id="3b0de-116">Представляет общее смещение от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="3b0de-116">Represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="3b0de-117">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="3b0de-117">This value is in minutes.</span></span>  <br/> |
|[<span data-ttu-id="3b0de-118">StandardTime</span><span class="sxs-lookup"><span data-stu-id="3b0de-118">StandardTime</span></span>](standardtime.md) <br/> |<span data-ttu-id="3b0de-119">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) .</span><span class="sxs-lookup"><span data-stu-id="3b0de-119">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element.</span></span> <span data-ttu-id="3b0de-120">Этот элемент также содержит сведения о переходе на зимнее время с летнего времени в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="3b0de-120">This element also contains information about the transition to standard time from daylight saving time in regions where daylight saving time is observed.</span></span>  <br/> |
|[<span data-ttu-id="3b0de-121">DaylightTime</span><span class="sxs-lookup"><span data-stu-id="3b0de-121">DaylightTime</span></span>](daylighttime.md) <br/> |<span data-ttu-id="3b0de-122">Представляет смещение относительно времени в формате UTC, представленного элементом [смещения (UTC)](bias-utc.md) в регионах, где наблюдается летнее время.</span><span class="sxs-lookup"><span data-stu-id="3b0de-122">Represents an offset from the time relative to UTC represented by the [Bias (UTC)](bias-utc.md) element in regions where daylight saving time is observed.</span></span> <span data-ttu-id="3b0de-123">Этот элемент также содержит сведения о том, когда происходит переход на летнее время из стандартного времени.</span><span class="sxs-lookup"><span data-stu-id="3b0de-123">This element also contains information about when the transition to daylight saving time from standard time occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b0de-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b0de-124">Parent elements</span></span>

|<span data-ttu-id="3b0de-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b0de-125">**Element**</span></span>|<span data-ttu-id="3b0de-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b0de-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b0de-127">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="3b0de-127">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="3b0de-128">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="3b0de-128">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="3b0de-129">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="3b0de-129">This is a root element.</span></span>  <br/> <span data-ttu-id="3b0de-130">Элемент **TimeZone** в сообщении жетусераваилабилитирекуест представляет часовой пояс, в котором указаны значения DateTime в запросе.</span><span class="sxs-lookup"><span data-stu-id="3b0de-130">The **TimeZone** element in the GetUserAvailabilityRequest message represents the time zone in which the DateTime values in the request are specified.</span></span> <span data-ttu-id="3b0de-131">Значения даты и времени, возвращаемые службой доступности, также находятся в этом часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="3b0de-131">The DateTime values returned by the Availability service are also in this time zone.</span></span>  <br/> <span data-ttu-id="3b0de-132">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="3b0de-132">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[<span data-ttu-id="3b0de-133">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="3b0de-133">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3b0de-134">Представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3b0de-134">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="3b0de-135">Элемент **TimeZone** в сообщении жетусераваилабилитиреспонсе представляет параметры часового пояса запрошенного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3b0de-135">The **TimeZone** element in the GetUserAvailabilityResponse message represents the time zone settings of the requested mailbox user.</span></span>  <br/> <span data-ttu-id="3b0de-136">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="3b0de-136">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b0de-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b0de-137">Remarks</span></span>

<span data-ttu-id="3b0de-138">Этот элемент является обязательным для элемента [жетусераваилабилитирекуест](getuseravailabilityrequest.md) .</span><span class="sxs-lookup"><span data-stu-id="3b0de-138">This element is required in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) element.</span></span> <span data-ttu-id="3b0de-139">Этот элемент происходит не более одного раза или по крайней мере ноль раз, когда родительский элемент является элементом [воркингхаурс](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="3b0de-139">This element occurs at most once or at least zero times when the parent element is the [WorkingHours](workinghours-ex15websvcsotherref.md) element.</span></span> 
  
## <a name="example"></a><span data-ttu-id="3b0de-140">Пример</span><span class="sxs-lookup"><span data-stu-id="3b0de-140">Example</span></span>

<span data-ttu-id="3b0de-141">В приведенном ниже примере показана часть XML-запроса, которая определяет смещение относительно времени в формате UTC 8 часов в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="3b0de-141">The following example shows part of an XML request that identifies an offset from UTC of 8 hours in the client application.</span></span>
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a><span data-ttu-id="3b0de-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3b0de-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b0de-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3b0de-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3b0de-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3b0de-144">Schema Name</span></span>  <br/> |<span data-ttu-id="3b0de-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3b0de-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="3b0de-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3b0de-146">Validation File</span></span>  <br/> |<span data-ttu-id="3b0de-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3b0de-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3b0de-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3b0de-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b0de-149">False</span><span class="sxs-lookup"><span data-stu-id="3b0de-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b0de-150">См. также</span><span class="sxs-lookup"><span data-stu-id="3b0de-150">See also</span></span>



[<span data-ttu-id="3b0de-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3b0de-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3b0de-152">Bias</span><span class="sxs-lookup"><span data-stu-id="3b0de-152">Bias</span></span>](bias.md)


[<span data-ttu-id="3b0de-153">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="3b0de-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

