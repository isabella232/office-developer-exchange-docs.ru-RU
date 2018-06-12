---
title: Тема (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: 05e955b5-8e90-4043-b06b-6ce523eaed9b
description: Элемент темы — Тема элемента календаря.
ms.openlocfilehash: 5303a7568e017999f2be69c50588832748b5668a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835610"
---
# <a name="subject-calendareventdetails"></a><span data-ttu-id="c819a-103">Тема (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="c819a-103">Subject (CalendarEventDetails)</span></span>

<span data-ttu-id="c819a-104">Элемент **темы** — Тема элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c819a-104">The **Subject** element represents the subject of a calendar item.</span></span> 
  
[<span data-ttu-id="c819a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c819a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c819a-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="c819a-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="c819a-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="c819a-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="c819a-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="c819a-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="c819a-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="c819a-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="c819a-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="c819a-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="c819a-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="c819a-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="c819a-112">Тема (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="c819a-112">Subject (CalendarEventDetails)</span></span>](subject-calendareventdetails.md)
  
```xml
<Subject/>
```

 <span data-ttu-id="c819a-113">**string**</span><span class="sxs-lookup"><span data-stu-id="c819a-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c819a-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c819a-114">Attributes and elements</span></span>

<span data-ttu-id="c819a-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c819a-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c819a-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c819a-116">Attributes</span></span>

<span data-ttu-id="c819a-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="c819a-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c819a-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c819a-118">Child elements</span></span>

<span data-ttu-id="c819a-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="c819a-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c819a-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c819a-120">Parent elements</span></span>

|<span data-ttu-id="c819a-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c819a-121">**Element**</span></span>|<span data-ttu-id="c819a-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c819a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c819a-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="c819a-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="c819a-124">Дополнительные сведения для события календаря.</span><span class="sxs-lookup"><span data-stu-id="c819a-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="c819a-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c819a-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c819a-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c819a-126">Text value</span></span>

<span data-ttu-id="c819a-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="c819a-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="c819a-128">Этот элемент не будет возвращен, если значение элемента [IsPrivate](isprivate.md) значение **true**.</span><span class="sxs-lookup"><span data-stu-id="c819a-128">This element will not be returned if the [IsPrivate](isprivate.md) element value is equal to **true**.</span></span> <span data-ttu-id="c819a-129">Этот элемент может содержать пустую строку.</span><span class="sxs-lookup"><span data-stu-id="c819a-129">This element can contain an empty string.</span></span> <span data-ttu-id="c819a-130">Этот элемент является обязательным, если используется элемент [CalendarEventDetails](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="c819a-130">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c819a-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="c819a-131">Remarks</span></span>

<span data-ttu-id="c819a-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c819a-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c819a-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c819a-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c819a-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c819a-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c819a-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c819a-135">Schema Name</span></span>  <br/> |<span data-ttu-id="c819a-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c819a-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="c819a-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c819a-137">Validation File</span></span>  <br/> |<span data-ttu-id="c819a-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c819a-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c819a-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c819a-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="c819a-140">False</span><span class="sxs-lookup"><span data-stu-id="c819a-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c819a-141">См. также</span><span class="sxs-lookup"><span data-stu-id="c819a-141">See also</span></span>



[<span data-ttu-id="c819a-142">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c819a-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c819a-143">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c819a-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c819a-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="c819a-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

