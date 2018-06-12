---
title: CalendarEvent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEvent
api_type:
- schema
ms.assetid: 91958c01-1fcb-4ac0-8601-5e5b434c988a
description: Элемент CalendarEvent представляет вхождение элемента уникальный календаря.
ms.openlocfilehash: f7fff7ba511ca12813dd4c2d694e89c97589ba31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761637"
---
# <a name="calendarevent"></a><span data-ttu-id="eecaa-103">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="eecaa-103">CalendarEvent</span></span>

<span data-ttu-id="eecaa-104">Элемент **CalendarEvent** представляет вхождение элемента уникальный календаря.</span><span class="sxs-lookup"><span data-stu-id="eecaa-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="eecaa-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eecaa-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="eecaa-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="eecaa-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="eecaa-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="eecaa-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="eecaa-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="eecaa-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="eecaa-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="eecaa-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="eecaa-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="eecaa-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="eecaa-111">**CalendarEvent**</span><span class="sxs-lookup"><span data-stu-id="eecaa-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eecaa-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="eecaa-112">Attributes and elements</span></span>

<span data-ttu-id="eecaa-113">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="eecaa-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eecaa-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="eecaa-114">Attributes</span></span>

<span data-ttu-id="eecaa-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="eecaa-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eecaa-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="eecaa-116">Child elements</span></span>

|<span data-ttu-id="eecaa-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eecaa-117">**Element**</span></span>|<span data-ttu-id="eecaa-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eecaa-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eecaa-119">Время начала</span><span class="sxs-lookup"><span data-stu-id="eecaa-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="eecaa-120">Представляет начало события календаря.</span><span class="sxs-lookup"><span data-stu-id="eecaa-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="eecaa-121">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="eecaa-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="eecaa-122">Время окончания</span><span class="sxs-lookup"><span data-stu-id="eecaa-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="eecaa-123">Представляет конец события календаря.</span><span class="sxs-lookup"><span data-stu-id="eecaa-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="eecaa-124">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="eecaa-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="eecaa-125">BusyType</span><span class="sxs-lookup"><span data-stu-id="eecaa-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="eecaa-126">Представляет состояние сведений о доступности для события календаря.</span><span class="sxs-lookup"><span data-stu-id="eecaa-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="eecaa-127">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="eecaa-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="eecaa-128">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="eecaa-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="eecaa-129">Дополнительные сведения для события календаря.</span><span class="sxs-lookup"><span data-stu-id="eecaa-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="eecaa-130">Это необязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="eecaa-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eecaa-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="eecaa-131">Parent elements</span></span>

|<span data-ttu-id="eecaa-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eecaa-132">**Element**</span></span>|<span data-ttu-id="eecaa-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eecaa-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eecaa-134">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="eecaa-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="eecaa-135">Содержит набор вхождений элемента уникальный календаря, которые представляют доступности запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="eecaa-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="eecaa-136">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="eecaa-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eecaa-137">Замечания</span><span class="sxs-lookup"><span data-stu-id="eecaa-137">Remarks</span></span>

<span data-ttu-id="eecaa-138">Время встречи и собрания возвращается в часовом поясе клиента.</span><span class="sxs-lookup"><span data-stu-id="eecaa-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="eecaa-139">Все дочерние элементы, перечислены в последовательности, в котором они изложены.</span><span class="sxs-lookup"><span data-stu-id="eecaa-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="eecaa-140">Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="eecaa-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="eecaa-141">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="eecaa-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eecaa-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="eecaa-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eecaa-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="eecaa-143">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eecaa-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="eecaa-144">Schema Name</span></span>  <br/> |<span data-ttu-id="eecaa-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="eecaa-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="eecaa-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="eecaa-146">Validation File</span></span>  <br/> |<span data-ttu-id="eecaa-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="eecaa-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="eecaa-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="eecaa-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="eecaa-149">False</span><span class="sxs-lookup"><span data-stu-id="eecaa-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eecaa-150">См. также</span><span class="sxs-lookup"><span data-stu-id="eecaa-150">See also</span></span>



[<span data-ttu-id="eecaa-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="eecaa-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="eecaa-152">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="eecaa-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="eecaa-153">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="eecaa-153">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

