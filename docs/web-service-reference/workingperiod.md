---
title: WorkingPeriod
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriod
api_type:
- schema
ms.assetid: 3b4e48af-9880-42b9-a0dc-dae7ac43c264
description: Элемент WorkingPeriod содержит рабочей недели дни и часы пользователя почтового ящика.
ms.openlocfilehash: 0f2707bede5e49174ed62a35ba704e39c0c48e9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840532"
---
# <a name="workingperiod"></a><span data-ttu-id="2adb9-103">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="2adb9-103">WorkingPeriod</span></span>

<span data-ttu-id="2adb9-104">Элемент **WorkingPeriod** содержит рабочей недели дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2adb9-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="2adb9-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2adb9-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="2adb9-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="2adb9-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="2adb9-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="2adb9-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="2adb9-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="2adb9-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="2adb9-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="2adb9-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="2adb9-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="2adb9-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="2adb9-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="2adb9-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="2adb9-112">**WorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="2adb9-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2adb9-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2adb9-113">Attributes and elements</span></span>

<span data-ttu-id="2adb9-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2adb9-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2adb9-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2adb9-115">Attributes</span></span>

<span data-ttu-id="2adb9-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="2adb9-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2adb9-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2adb9-117">Child elements</span></span>

|<span data-ttu-id="2adb9-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2adb9-118">**Element**</span></span>|<span data-ttu-id="2adb9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2adb9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2adb9-120">DayOfWeek (WorkingPeriod)</span><span class="sxs-lookup"><span data-stu-id="2adb9-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="2adb9-121">Содержит список рабочих дней, запланированный для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2adb9-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="2adb9-122">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="2adb9-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="2adb9-123">Представляет начала рабочего дня для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2adb9-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="2adb9-124">EndTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="2adb9-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="2adb9-125">Представляет окончания рабочего дня для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2adb9-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2adb9-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2adb9-126">Parent elements</span></span>

|<span data-ttu-id="2adb9-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2adb9-127">**Element**</span></span>|<span data-ttu-id="2adb9-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2adb9-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2adb9-129">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="2adb9-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="2adb9-130">Содержит работа периода сведения для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="2adb9-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="2adb9-131">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="2adb9-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2adb9-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="2adb9-132">Remarks</span></span>

<span data-ttu-id="2adb9-133">Все дочерние элементы, перечислены в последовательности, в котором они изложены.</span><span class="sxs-lookup"><span data-stu-id="2adb9-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="2adb9-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2adb9-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2adb9-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2adb9-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2adb9-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2adb9-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2adb9-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2adb9-137">Schema Name</span></span>  <br/> |<span data-ttu-id="2adb9-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="2adb9-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="2adb9-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2adb9-139">Validation File</span></span>  <br/> |<span data-ttu-id="2adb9-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2adb9-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2adb9-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2adb9-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="2adb9-142">False</span><span class="sxs-lookup"><span data-stu-id="2adb9-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2adb9-143">См. также</span><span class="sxs-lookup"><span data-stu-id="2adb9-143">See also</span></span>



[<span data-ttu-id="2adb9-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="2adb9-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="2adb9-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="2adb9-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="2adb9-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="2adb9-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

