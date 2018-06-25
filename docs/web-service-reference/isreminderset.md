---
title: IsReminderSet
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReminderSet
api_type:
- schema
ms.assetid: 6aea4cb7-ca14-4949-8e7f-660b565f6556
description: Элемент IsReminderSet указывает, установил ли напоминания для событий календаря.
ms.openlocfilehash: 589178072baca652bff2779e64a212fb90478247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834100"
---
# <a name="isreminderset"></a><span data-ttu-id="89367-103">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="89367-103">IsReminderSet</span></span>

<span data-ttu-id="89367-104">Элемент **IsReminderSet** указывает, установил ли напоминания для событий календаря.</span><span class="sxs-lookup"><span data-stu-id="89367-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="89367-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="89367-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="89367-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="89367-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="89367-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="89367-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="89367-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="89367-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="89367-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="89367-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="89367-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="89367-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="89367-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="89367-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="89367-112">IsReminderSet</span><span class="sxs-lookup"><span data-stu-id="89367-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="89367-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="89367-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="89367-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="89367-114">Attributes and elements</span></span>

<span data-ttu-id="89367-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="89367-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="89367-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="89367-116">Attributes</span></span>

<span data-ttu-id="89367-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="89367-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="89367-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="89367-118">Child elements</span></span>

<span data-ttu-id="89367-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="89367-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="89367-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="89367-120">Parent elements</span></span>

|<span data-ttu-id="89367-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="89367-121">**Element**</span></span>|<span data-ttu-id="89367-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="89367-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="89367-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="89367-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="89367-124">Дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="89367-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="89367-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="89367-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="89367-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="89367-126">Text value</span></span>

<span data-ttu-id="89367-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="89367-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="89367-128">Этот элемент является обязательным, если элемент [CalendarEventDetails](calendareventdetails.md) используется в том случае, если элемент [IsPrivate](isprivate.md) не установлен в **значение true**.</span><span class="sxs-lookup"><span data-stu-id="89367-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="89367-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="89367-129">Remarks</span></span>

<span data-ttu-id="89367-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="89367-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="89367-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="89367-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="89367-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="89367-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="89367-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="89367-133">Schema Name</span></span>  <br/> |<span data-ttu-id="89367-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="89367-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="89367-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="89367-135">Validation File</span></span>  <br/> |<span data-ttu-id="89367-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="89367-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="89367-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="89367-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="89367-138">False</span><span class="sxs-lookup"><span data-stu-id="89367-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="89367-139">См. также</span><span class="sxs-lookup"><span data-stu-id="89367-139">See also</span></span>



[<span data-ttu-id="89367-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="89367-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="89367-141">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="89367-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="89367-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="89367-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

