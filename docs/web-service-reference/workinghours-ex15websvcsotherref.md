---
title: WorkingHours
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: Элемент WorkingHours представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.
ms.openlocfilehash: c53779422b87adebed370a1ed88e4e91c7a2dcaf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840520"
---
# <a name="workinghours"></a><span data-ttu-id="3774b-103">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3774b-103">WorkingHours</span></span>

<span data-ttu-id="3774b-104">Элемент **WorkingHours** представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="3774b-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="3774b-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3774b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="3774b-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="3774b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="3774b-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3774b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="3774b-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3774b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="3774b-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="3774b-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="3774b-110">**WorkingHours**</span><span class="sxs-lookup"><span data-stu-id="3774b-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3774b-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3774b-111">Attributes and elements</span></span>

<span data-ttu-id="3774b-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="3774b-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3774b-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3774b-113">Attributes</span></span>

<span data-ttu-id="3774b-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="3774b-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3774b-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3774b-115">Child elements</span></span>

|<span data-ttu-id="3774b-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3774b-116">**Element**</span></span>|<span data-ttu-id="3774b-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3774b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3774b-118">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="3774b-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="3774b-119">Содержит элементы, чтобы указать часовой пояс сведения.</span><span class="sxs-lookup"><span data-stu-id="3774b-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="3774b-120">Этот элемент также содержит сведения о переходе между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="3774b-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="3774b-121">Этот элемент является обязательным, если используется элемент **WorkingHours** .</span><span class="sxs-lookup"><span data-stu-id="3774b-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="3774b-122">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="3774b-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="3774b-123">Содержит работа периода сведения для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3774b-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="3774b-124">Этот элемент является обязательным, если используется элемент **WorkingHours** .</span><span class="sxs-lookup"><span data-stu-id="3774b-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3774b-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3774b-125">Parent elements</span></span>

|<span data-ttu-id="3774b-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3774b-126">**Element**</span></span>|<span data-ttu-id="3774b-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3774b-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3774b-128">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="3774b-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="3774b-129">Содержит сведения о доступности для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3774b-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="3774b-130">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="3774b-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3774b-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="3774b-131">Remarks</span></span>

<span data-ttu-id="3774b-132">Все дочерние элементы, перечислены в последовательности, в котором они изложены.</span><span class="sxs-lookup"><span data-stu-id="3774b-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="3774b-133">Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="3774b-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="3774b-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3774b-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3774b-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3774b-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3774b-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3774b-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3774b-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3774b-137">Schema Name</span></span>  <br/> |<span data-ttu-id="3774b-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3774b-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="3774b-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3774b-139">Validation File</span></span>  <br/> |<span data-ttu-id="3774b-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3774b-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3774b-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3774b-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="3774b-142">False</span><span class="sxs-lookup"><span data-stu-id="3774b-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3774b-143">См. также</span><span class="sxs-lookup"><span data-stu-id="3774b-143">See also</span></span>



[<span data-ttu-id="3774b-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="3774b-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="3774b-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="3774b-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="3774b-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="3774b-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

