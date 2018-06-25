---
title: IsMeeting (CalendarEventDetails)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeeting
api_type:
- schema
ms.assetid: dd6900e4-e4a3-471a-909d-7240ebec501b
description: Элемент IsMeeting указывает, является ли событие календаря собрания или встречи.
ms.openlocfilehash: f3f6e0cc5fbfe29e5a818d69794cbaf5b6855962
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834046"
---
# <a name="ismeeting-calendareventdetails"></a><span data-ttu-id="b41af-103">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="b41af-103">IsMeeting (CalendarEventDetails)</span></span>

<span data-ttu-id="b41af-104">Элемент **IsMeeting** указывает, является ли событие календаря собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="b41af-104">The **IsMeeting** element indicates whether the calendar event is a meeting or an appointment.</span></span> 
  
[<span data-ttu-id="b41af-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b41af-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b41af-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="b41af-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b41af-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="b41af-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b41af-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="b41af-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b41af-109">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="b41af-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="b41af-110">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="b41af-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="b41af-111">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="b41af-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="b41af-112">IsMeeting (CalendarEventDetails)</span><span class="sxs-lookup"><span data-stu-id="b41af-112">IsMeeting (CalendarEventDetails)</span></span>](ismeeting-calendareventdetails.md)
  
```xml
<IsMeeting>true or false</IsMeeting>
```

 <span data-ttu-id="b41af-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b41af-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b41af-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b41af-114">Attributes and elements</span></span>

<span data-ttu-id="b41af-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b41af-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b41af-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b41af-116">Attributes</span></span>

<span data-ttu-id="b41af-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="b41af-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b41af-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b41af-118">Child elements</span></span>

<span data-ttu-id="b41af-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="b41af-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b41af-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b41af-120">Parent elements</span></span>

|<span data-ttu-id="b41af-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b41af-121">**Element**</span></span>|<span data-ttu-id="b41af-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b41af-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b41af-123">CalendarEventDetails</span><span class="sxs-lookup"><span data-stu-id="b41af-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="b41af-124">Дополнительные сведения для события календаря.</span><span class="sxs-lookup"><span data-stu-id="b41af-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="b41af-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="b41af-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b41af-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b41af-126">Text value</span></span>

<span data-ttu-id="b41af-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="b41af-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="b41af-128">Этот элемент является обязательным, если используется элемент [CalendarEventDetails](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="b41af-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b41af-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="b41af-129">Remarks</span></span>

<span data-ttu-id="b41af-130">Различие между собрания и встречи является собрания элемента календаря, который включает в себя участников; Встреча — элемента календаря, который не включает участников.</span><span class="sxs-lookup"><span data-stu-id="b41af-130">The difference between a meeting and an appointment is that a meeting is a calendar item that includes attendees; an appointment is a calendar item that does not include attendees.</span></span>
  
<span data-ttu-id="b41af-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b41af-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b41af-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b41af-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b41af-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b41af-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b41af-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b41af-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b41af-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b41af-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b41af-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b41af-136">Validation File</span></span>  <br/> |<span data-ttu-id="b41af-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b41af-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b41af-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b41af-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b41af-139">False</span><span class="sxs-lookup"><span data-stu-id="b41af-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b41af-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b41af-140">See also</span></span>



[<span data-ttu-id="b41af-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b41af-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b41af-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="b41af-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b41af-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b41af-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

