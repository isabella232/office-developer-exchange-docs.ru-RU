---
title: DayOfWeek (Воркингпериод)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: Элемент DayOfWeek содержит список рабочих дней, запланированных для пользователя почтового ящика.
ms.openlocfilehash: 06d4a7d5541b3b71fcbf9be9beb7512d06853283
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457447"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="578fc-103">DayOfWeek (Воркингпериод)</span><span class="sxs-lookup"><span data-stu-id="578fc-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="578fc-104">Элемент **DayOfWeek** содержит список рабочих дней, запланированных для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="578fc-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="578fc-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="578fc-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="578fc-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="578fc-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="578fc-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="578fc-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="578fc-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="578fc-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="578fc-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="578fc-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="578fc-110">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="578fc-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="578fc-111">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="578fc-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="578fc-112">DayOfWeek (Воркингпериод)</span><span class="sxs-lookup"><span data-stu-id="578fc-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="578fc-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="578fc-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="578fc-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="578fc-114">Attributes and elements</span></span>

<span data-ttu-id="578fc-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="578fc-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="578fc-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="578fc-116">Attributes</span></span>

<span data-ttu-id="578fc-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="578fc-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="578fc-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="578fc-118">Child elements</span></span>

<span data-ttu-id="578fc-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="578fc-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="578fc-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="578fc-120">Parent elements</span></span>

|<span data-ttu-id="578fc-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="578fc-121">**Element**</span></span>|<span data-ttu-id="578fc-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="578fc-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="578fc-123">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="578fc-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="578fc-124">Содержит рабочие недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="578fc-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="578fc-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="578fc-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="578fc-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="578fc-126">Text value</span></span>

<span data-ttu-id="578fc-127">Текстовое значение возвращается, если у пользователя почтового ящика есть дни, настроенные для представления рабочей недели.</span><span class="sxs-lookup"><span data-stu-id="578fc-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="578fc-128">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="578fc-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="578fc-129">Воскресеньям</span><span class="sxs-lookup"><span data-stu-id="578fc-129">Sunday</span></span>    
- <span data-ttu-id="578fc-130">Понедельник</span><span class="sxs-lookup"><span data-stu-id="578fc-130">Monday</span></span>    
- <span data-ttu-id="578fc-131">Вторник</span><span class="sxs-lookup"><span data-stu-id="578fc-131">Tuesday</span></span>    
- <span data-ttu-id="578fc-132">Среда</span><span class="sxs-lookup"><span data-stu-id="578fc-132">Wednesday</span></span>    
- <span data-ttu-id="578fc-133">Четверг</span><span class="sxs-lookup"><span data-stu-id="578fc-133">Thursday</span></span>    
- <span data-ttu-id="578fc-134">Пятница</span><span class="sxs-lookup"><span data-stu-id="578fc-134">Friday</span></span>    
- <span data-ttu-id="578fc-135">Суббота</span><span class="sxs-lookup"><span data-stu-id="578fc-135">Saturday</span></span> 
    
<span data-ttu-id="578fc-136">Текстовые значения будут возвращены в указанном порядке.</span><span class="sxs-lookup"><span data-stu-id="578fc-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="578fc-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="578fc-137">Remarks</span></span>

<span data-ttu-id="578fc-138">Важно отметить, что разница между этим элементом и элементом доступности [DayOfWeek (TimeZone)](dayofweek-timezone.md) — это тип.</span><span class="sxs-lookup"><span data-stu-id="578fc-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="578fc-139">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="578fc-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="578fc-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="578fc-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="578fc-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="578fc-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="578fc-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="578fc-142">Schema Name</span></span>  <br/> |<span data-ttu-id="578fc-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="578fc-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="578fc-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="578fc-144">Validation File</span></span>  <br/> |<span data-ttu-id="578fc-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="578fc-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="578fc-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="578fc-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="578fc-147">False</span><span class="sxs-lookup"><span data-stu-id="578fc-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="578fc-148">См. также</span><span class="sxs-lookup"><span data-stu-id="578fc-148">See also</span></span>

- [<span data-ttu-id="578fc-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="578fc-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="578fc-150">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="578fc-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="578fc-151">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="578fc-151">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

