---
title: Расположение (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: Элемент Location представляет поля расположения элемента календаря.
ms.openlocfilehash: 3678bd94851633fcca9817c020106670b57d110c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834245"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="e5c98-103">Расположение (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="e5c98-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="e5c98-104">Элемент **Location** представляет поля расположения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="e5c98-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="e5c98-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5c98-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e5c98-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="e5c98-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="e5c98-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="e5c98-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="e5c98-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="e5c98-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="e5c98-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="e5c98-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="e5c98-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="e5c98-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="e5c98-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="e5c98-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="e5c98-112">Расположение (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="e5c98-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="e5c98-113">**string**</span><span class="sxs-lookup"><span data-stu-id="e5c98-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e5c98-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e5c98-114">Attributes and elements</span></span>

<span data-ttu-id="e5c98-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e5c98-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e5c98-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e5c98-116">Attributes</span></span>

<span data-ttu-id="e5c98-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="e5c98-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e5c98-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e5c98-118">Child elements</span></span>

<span data-ttu-id="e5c98-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="e5c98-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e5c98-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e5c98-120">Parent elements</span></span>

|<span data-ttu-id="e5c98-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e5c98-121">**Element**</span></span>|<span data-ttu-id="e5c98-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e5c98-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e5c98-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="e5c98-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="e5c98-124">Дополнительные сведения для события календаря.</span><span class="sxs-lookup"><span data-stu-id="e5c98-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="e5c98-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="e5c98-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e5c98-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e5c98-126">Text value</span></span>

<span data-ttu-id="e5c98-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="e5c98-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="e5c98-128">Этот элемент может содержать пустую строку.</span><span class="sxs-lookup"><span data-stu-id="e5c98-128">This element can contain an empty string.</span></span> <span data-ttu-id="e5c98-129">Этот элемент является обязательным, если используется элемент [CalendarEventDetails](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="e5c98-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e5c98-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="e5c98-130">Remarks</span></span>

<span data-ttu-id="e5c98-131">Этот элемент сопоставляет PR_Location MAPI, именованное свойство.</span><span class="sxs-lookup"><span data-stu-id="e5c98-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="e5c98-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e5c98-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e5c98-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e5c98-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e5c98-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e5c98-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e5c98-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e5c98-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e5c98-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e5c98-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e5c98-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e5c98-137">Validation File</span></span>  <br/> |<span data-ttu-id="e5c98-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e5c98-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e5c98-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e5c98-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e5c98-140">False</span><span class="sxs-lookup"><span data-stu-id="e5c98-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e5c98-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e5c98-141">See also</span></span>



[<span data-ttu-id="e5c98-142">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e5c98-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e5c98-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="e5c98-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e5c98-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e5c98-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

