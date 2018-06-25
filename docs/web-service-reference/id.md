---
title: ID
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ID
api_type:
- schema
ms.assetid: 8caf922f-56bd-466a-a68f-d6cb236f2eec
description: Элемент ID представляет идентификатор записи элемента календаря.
ms.openlocfilehash: bdfadcbe074135aca34a408e69ed4a69974eb5d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833855"
---
# <a name="id"></a><span data-ttu-id="d39a6-103">ID</span><span class="sxs-lookup"><span data-stu-id="d39a6-103">ID</span></span>

<span data-ttu-id="d39a6-104">Элемент **ID** представляет идентификатор записи элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="d39a6-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="d39a6-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d39a6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d39a6-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="d39a6-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d39a6-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="d39a6-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d39a6-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="d39a6-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="d39a6-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="d39a6-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="d39a6-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="d39a6-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="d39a6-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d39a6-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="d39a6-112">ИД</span><span class="sxs-lookup"><span data-stu-id="d39a6-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="d39a6-113">**string**</span><span class="sxs-lookup"><span data-stu-id="d39a6-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d39a6-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d39a6-114">Attributes and elements</span></span>

<span data-ttu-id="d39a6-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d39a6-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d39a6-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d39a6-116">Attributes</span></span>

<span data-ttu-id="d39a6-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="d39a6-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d39a6-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d39a6-118">Child elements</span></span>

<span data-ttu-id="d39a6-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="d39a6-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d39a6-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d39a6-120">Parent elements</span></span>

|<span data-ttu-id="d39a6-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d39a6-121">**Element**</span></span>|<span data-ttu-id="d39a6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d39a6-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d39a6-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="d39a6-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="d39a6-124">Дополнительные сведения для события календаря.</span><span class="sxs-lookup"><span data-stu-id="d39a6-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="d39a6-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="d39a6-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d39a6-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d39a6-126">Text value</span></span>

<span data-ttu-id="d39a6-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="d39a6-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="d39a6-128">Этот элемент является обязательным, если используется элемент [CalendarEventDetails](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="d39a6-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d39a6-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="d39a6-129">Remarks</span></span>

<span data-ttu-id="d39a6-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d39a6-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d39a6-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d39a6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d39a6-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d39a6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d39a6-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d39a6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="d39a6-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d39a6-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d39a6-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d39a6-135">Validation File</span></span>  <br/> |<span data-ttu-id="d39a6-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d39a6-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d39a6-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d39a6-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="d39a6-138">False</span><span class="sxs-lookup"><span data-stu-id="d39a6-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d39a6-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d39a6-139">See also</span></span>



[<span data-ttu-id="d39a6-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d39a6-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d39a6-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="d39a6-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d39a6-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d39a6-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

