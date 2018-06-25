---
title: IsRecurring (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: 42323940-0ccb-4a05-86e4-262bde5e41b0
description: Элемент IsRecurring указывает, является ли событие календаря экземпляр повторяющегося элемента календаря или элемента одного календаря.
ms.openlocfilehash: 87a168dc48bdd5ba2ea9398dd84f696e7729db44
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834103"
---
# <a name="isrecurring-calendareventdetails"></a><span data-ttu-id="d6dea-103">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="d6dea-103">IsRecurring (CalendarEventDetails)</span></span>

<span data-ttu-id="d6dea-104">Элемент **IsRecurring** указывает, является ли событие календаря экземпляр повторяющегося элемента календаря или элемента одного календаря.</span><span class="sxs-lookup"><span data-stu-id="d6dea-104">The **IsRecurring** element indicates whether the calendar event is an instance of a recurring calendar item or a single calendar item.</span></span> 
  
[<span data-ttu-id="d6dea-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d6dea-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d6dea-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d6dea-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d6dea-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d6dea-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d6dea-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d6dea-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d6dea-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="d6dea-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="d6dea-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="d6dea-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="d6dea-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d6dea-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="d6dea-112">IsRecurring (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="d6dea-112">IsRecurring (CalendarEventDetails)</span></span>](isrecurring-calendareventdetails.md)
  
```xml
<IsRecurring>true or false</IsRecurring>
```

 <span data-ttu-id="d6dea-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="d6dea-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6dea-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d6dea-114">Attributes and elements</span></span>

<span data-ttu-id="d6dea-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d6dea-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6dea-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d6dea-116">Attributes</span></span>

<span data-ttu-id="d6dea-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="d6dea-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6dea-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d6dea-118">Child elements</span></span>

<span data-ttu-id="d6dea-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="d6dea-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d6dea-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d6dea-120">Parent elements</span></span>

|<span data-ttu-id="d6dea-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6dea-121">**Element**</span></span>|<span data-ttu-id="d6dea-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6dea-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6dea-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d6dea-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="d6dea-124">Дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="d6dea-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="d6dea-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d6dea-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d6dea-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d6dea-126">Text value</span></span>

<span data-ttu-id="d6dea-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="d6dea-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="d6dea-128">Этот элемент является обязательным, если используется элемент [CalendarEventDetails](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d6dea-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d6dea-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="d6dea-129">Remarks</span></span>

<span data-ttu-id="d6dea-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d6dea-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d6dea-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d6dea-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6dea-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d6dea-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d6dea-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d6dea-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d6dea-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d6dea-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d6dea-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d6dea-135">Validation File</span></span>  <br/> |<span data-ttu-id="d6dea-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d6dea-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d6dea-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d6dea-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6dea-138">False</span><span class="sxs-lookup"><span data-stu-id="d6dea-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6dea-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d6dea-139">See also</span></span>



[<span data-ttu-id="d6dea-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d6dea-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d6dea-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d6dea-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d6dea-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d6dea-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

