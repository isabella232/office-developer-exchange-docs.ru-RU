---
title: WorkingPeriodArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriodArray
api_type:
- schema
ms.assetid: 3a3f6393-eacc-4734-b6c9-b67023fe2830
description: Элемент WorkingPeriodArray содержит работа периода сведения для пользователя почтового ящика.
ms.openlocfilehash: 02712f05dc3373a532d769f476341b78ad25a79c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840531"
---
# <a name="workingperiodarray"></a><span data-ttu-id="b83c1-103">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="b83c1-103">WorkingPeriodArray</span></span>

<span data-ttu-id="b83c1-104">Элемент **WorkingPeriodArray** содержит работа периода сведения для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b83c1-104">The **WorkingPeriodArray** element contains working period information for the mailbox user.</span></span> 
  
[<span data-ttu-id="b83c1-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b83c1-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b83c1-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b83c1-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b83c1-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b83c1-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b83c1-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b83c1-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b83c1-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="b83c1-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="b83c1-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="b83c1-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
```xml
<WorkingPeriodArray>
   <WorkingPeriod>...</WorkingPeriod>
</WorkingPeriodArray>
```

 <span data-ttu-id="b83c1-111">**ArrayOfWorkingPeriod**</span><span class="sxs-lookup"><span data-stu-id="b83c1-111">**ArrayOfWorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b83c1-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b83c1-112">Attributes and elements</span></span>

<span data-ttu-id="b83c1-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b83c1-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b83c1-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b83c1-114">Attributes</span></span>

<span data-ttu-id="b83c1-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="b83c1-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b83c1-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b83c1-116">Child elements</span></span>

|<span data-ttu-id="b83c1-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b83c1-117">**Element**</span></span>|<span data-ttu-id="b83c1-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b83c1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b83c1-119">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="b83c1-119">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="b83c1-120">Содержит рабочей недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="b83c1-120">Contains the work week days and hours of the mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b83c1-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b83c1-121">Parent elements</span></span>

|<span data-ttu-id="b83c1-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b83c1-122">**Element**</span></span>|<span data-ttu-id="b83c1-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b83c1-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b83c1-124">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="b83c1-124">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="b83c1-125">Представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="b83c1-125">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> <span data-ttu-id="b83c1-126">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b83c1-126">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b83c1-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="b83c1-127">Remarks</span></span>

<span data-ttu-id="b83c1-128">Этот элемент является обязательным, если используется элемент [WorkingHours](workinghours-ex15websvcsotherref.md) .</span><span class="sxs-lookup"><span data-stu-id="b83c1-128">This element is required if the [WorkingHours](workinghours-ex15websvcsotherref.md) element is used.</span></span> <span data-ttu-id="b83c1-129">Все дочерние элементы, перечислены в последовательности, в котором они изложены.</span><span class="sxs-lookup"><span data-stu-id="b83c1-129">All the child elements are listed in the sequence in which they occur.</span></span> 
  
<span data-ttu-id="b83c1-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b83c1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b83c1-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b83c1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b83c1-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b83c1-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b83c1-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b83c1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b83c1-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b83c1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b83c1-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b83c1-135">Validation File</span></span>  <br/> |<span data-ttu-id="b83c1-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b83c1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b83c1-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b83c1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b83c1-138">False</span><span class="sxs-lookup"><span data-stu-id="b83c1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b83c1-139">См. также</span><span class="sxs-lookup"><span data-stu-id="b83c1-139">See also</span></span>



[<span data-ttu-id="b83c1-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b83c1-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b83c1-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b83c1-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b83c1-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b83c1-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

