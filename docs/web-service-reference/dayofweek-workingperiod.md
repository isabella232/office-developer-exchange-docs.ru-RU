---
title: DayOfWeek (WorkingPeriod)
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
description: Элемент DayOfWeek содержит список рабочих дней, запланированный для пользователя почтового ящика.
ms.openlocfilehash: a6a68017291ba13f45b3970307669222d583fcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762000"
---
# <a name="dayofweek-workingperiod"></a><span data-ttu-id="bda98-103">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="bda98-103">DayOfWeek (WorkingPeriod)</span></span>

<span data-ttu-id="bda98-104">Элемент **DayOfWeek** содержит список рабочих дней, запланированный для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bda98-104">The **DayOfWeek** element contains the list of working days scheduled for the mailbox user.</span></span> 
  
- [<span data-ttu-id="bda98-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bda98-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="bda98-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="bda98-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)  
- [<span data-ttu-id="bda98-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="bda98-107">FreeBusyResponse</span></span>](freebusyresponse.md)  
- [<span data-ttu-id="bda98-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="bda98-108">FreeBusyView</span></span>](freebusyview.md)  
- [<span data-ttu-id="bda98-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="bda98-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)  
- [<span data-ttu-id="bda98-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="bda98-110">WorkingPeriodArray</span></span>](workingperiodarray.md) 
- [<span data-ttu-id="bda98-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="bda98-111">WorkingPeriod</span></span>](workingperiod.md)  
- [<span data-ttu-id="bda98-112">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="bda98-112">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

<span data-ttu-id="bda98-113">**DaysOfWeek**</span><span class="sxs-lookup"><span data-stu-id="bda98-113">**DaysOfWeek**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bda98-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bda98-114">Attributes and elements</span></span>

<span data-ttu-id="bda98-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bda98-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bda98-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bda98-116">Attributes</span></span>

<span data-ttu-id="bda98-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="bda98-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bda98-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bda98-118">Child elements</span></span>

<span data-ttu-id="bda98-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="bda98-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bda98-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bda98-120">Parent elements</span></span>

|<span data-ttu-id="bda98-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bda98-121">**Element**</span></span>|<span data-ttu-id="bda98-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bda98-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bda98-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="bda98-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="bda98-124">Содержит рабочей недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="bda98-124">Contains the work week days and hours of the mailbox user.</span></span><br/><br/><span data-ttu-id="bda98-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="bda98-125">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bda98-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="bda98-126">Text value</span></span>

<span data-ttu-id="bda98-127">Если пользователь почтового ящика не дней, задайте для представления рабочей недели, возвращается значение текста.</span><span class="sxs-lookup"><span data-stu-id="bda98-127">A text value is returned if the mailbox user has days set to represent the work week.</span></span> <span data-ttu-id="bda98-128">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="bda98-128">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="bda98-129">Воскресенье</span><span class="sxs-lookup"><span data-stu-id="bda98-129">Sunday</span></span>    
- <span data-ttu-id="bda98-130">Понедельник</span><span class="sxs-lookup"><span data-stu-id="bda98-130">Monday</span></span>    
- <span data-ttu-id="bda98-131">Вторник</span><span class="sxs-lookup"><span data-stu-id="bda98-131">Tuesday</span></span>    
- <span data-ttu-id="bda98-132">Среда</span><span class="sxs-lookup"><span data-stu-id="bda98-132">Wednesday</span></span>    
- <span data-ttu-id="bda98-133">Четверг</span><span class="sxs-lookup"><span data-stu-id="bda98-133">Thursday</span></span>    
- <span data-ttu-id="bda98-134">Пятница</span><span class="sxs-lookup"><span data-stu-id="bda98-134">Friday</span></span>    
- <span data-ttu-id="bda98-135">Суббота</span><span class="sxs-lookup"><span data-stu-id="bda98-135">Saturday</span></span> 
    
<span data-ttu-id="bda98-136">Текстовые значения будут возвращены в указанном порядке.</span><span class="sxs-lookup"><span data-stu-id="bda98-136">The text values will be returned in that order.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bda98-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="bda98-137">Remarks</span></span>

<span data-ttu-id="bda98-138">Обратите внимание на то, что разница между этот элемент и элемент доступности [DayOfWeek (часовой пояс)](dayofweek-timezone.md) — это тип важно.</span><span class="sxs-lookup"><span data-stu-id="bda98-138">It is important to note that the difference between this element and the Availability [DayOfWeek (TimeZone)](dayofweek-timezone.md) element is the type.</span></span> 
  
<span data-ttu-id="bda98-139">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bda98-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bda98-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bda98-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bda98-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bda98-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bda98-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bda98-142">Schema Name</span></span>  <br/> |<span data-ttu-id="bda98-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bda98-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="bda98-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bda98-144">Validation File</span></span>  <br/> |<span data-ttu-id="bda98-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bda98-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bda98-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bda98-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="bda98-147">False</span><span class="sxs-lookup"><span data-stu-id="bda98-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bda98-148">См. также</span><span class="sxs-lookup"><span data-stu-id="bda98-148">See also</span></span>

- [<span data-ttu-id="bda98-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="bda98-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="bda98-150">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="bda98-150">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="bda98-151">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="bda98-151">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)
