---
title: CalendarEventArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventArray
api_type:
- schema
ms.assetid: a00f7f56-d7f1-429d-ae02-97043718c864
description: Элемент CalendarEventArray содержит набор вхождений элемента уникальный календаря, которые представляют доступности запрошенного пользователя.
ms.openlocfilehash: 2e56b7b2b94e12401ba708dfca94101064d625e1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761638"
---
# <a name="calendareventarray"></a><span data-ttu-id="4d53f-103">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="4d53f-103">CalendarEventArray</span></span>

<span data-ttu-id="4d53f-104">Элемент **CalendarEventArray** содержит набор вхождений элемента уникальный календаря, которые представляют доступности запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d53f-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="4d53f-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4d53f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4d53f-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="4d53f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="4d53f-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="4d53f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="4d53f-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="4d53f-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="4d53f-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="4d53f-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="4d53f-110">**ArrayOfCalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="4d53f-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d53f-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d53f-111">Attributes and elements</span></span>

<span data-ttu-id="4d53f-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4d53f-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d53f-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d53f-113">Attributes</span></span>

<span data-ttu-id="4d53f-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="4d53f-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d53f-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d53f-115">Child elements</span></span>

|<span data-ttu-id="4d53f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d53f-116">**Element**</span></span>|<span data-ttu-id="4d53f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d53f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d53f-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="4d53f-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="4d53f-119">Представляет вхождение элемента уникальный календаря.</span><span class="sxs-lookup"><span data-stu-id="4d53f-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d53f-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d53f-120">Parent elements</span></span>

|<span data-ttu-id="4d53f-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d53f-121">**Element**</span></span>|<span data-ttu-id="4d53f-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d53f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d53f-123">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="4d53f-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="4d53f-124">Содержит сведения о доступности для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d53f-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="4d53f-125">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="4d53f-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d53f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="4d53f-126">Remarks</span></span>

<span data-ttu-id="4d53f-127">Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="4d53f-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="4d53f-128">Этот элемент включен, если элемент [FreeBusyViewType](freebusyviewtype.md) задано значение **занятости**, **FreeBusyMerged**, **Detailed**или **DetailedMerged**.</span><span class="sxs-lookup"><span data-stu-id="4d53f-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="4d53f-129">Этот элемент не включает все дочерние элементы, если отсутствуют не элементы календаря в запрошенный временной интервал.</span><span class="sxs-lookup"><span data-stu-id="4d53f-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="4d53f-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4d53f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d53f-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d53f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d53f-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d53f-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d53f-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d53f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4d53f-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4d53f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d53f-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d53f-135">Validation File</span></span>  <br/> |<span data-ttu-id="4d53f-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4d53f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d53f-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d53f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d53f-138">False</span><span class="sxs-lookup"><span data-stu-id="4d53f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d53f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="4d53f-139">See also</span></span>



[<span data-ttu-id="4d53f-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4d53f-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4d53f-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="4d53f-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4d53f-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="4d53f-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

