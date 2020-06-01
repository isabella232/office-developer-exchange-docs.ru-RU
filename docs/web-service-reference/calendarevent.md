---
title: календаревент
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
description: Элемент Календаревент представляет уникальное вхождение элемента календаря.
ms.openlocfilehash: 8bf37c907ed726e33dd2b1eff9add5d6235704da
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459078"
---
# <a name="calendarevent"></a><span data-ttu-id="f2457-103">календаревент</span><span class="sxs-lookup"><span data-stu-id="f2457-103">CalendarEvent</span></span>

<span data-ttu-id="f2457-104">Элемент **календаревент** представляет уникальное вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="f2457-104">The **CalendarEvent** element represents a unique calendar item occurrence.</span></span> 
  
[<span data-ttu-id="f2457-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f2457-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f2457-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="f2457-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f2457-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f2457-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f2457-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="f2457-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f2457-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="f2457-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="f2457-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="f2457-110">CalendarEvent</span></span>](calendarevent.md)
  
```xml
<CalendarEvent>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
   <BusyType>...</BusyType>
   <CalendarEventDetails>...</CalendarEventDetails>
</CalendarEvent>
```

 <span data-ttu-id="f2457-111">**календаревент**</span><span class="sxs-lookup"><span data-stu-id="f2457-111">**CalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f2457-112">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f2457-112">Attributes and elements</span></span>

<span data-ttu-id="f2457-113">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f2457-113">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f2457-114">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f2457-114">Attributes</span></span>

<span data-ttu-id="f2457-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f2457-115">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f2457-116">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f2457-116">Child elements</span></span>

|<span data-ttu-id="f2457-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f2457-117">**Element**</span></span>|<span data-ttu-id="f2457-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f2457-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2457-119">StartTime</span><span class="sxs-lookup"><span data-stu-id="f2457-119">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="f2457-120">Представляет начало события календаря.</span><span class="sxs-lookup"><span data-stu-id="f2457-120">Represents the start of a calendar event.</span></span> <span data-ttu-id="f2457-121">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="f2457-121">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f2457-122">EndTime</span><span class="sxs-lookup"><span data-stu-id="f2457-122">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="f2457-123">Представляет конец события календаря.</span><span class="sxs-lookup"><span data-stu-id="f2457-123">Represents the end of a calendar event.</span></span> <span data-ttu-id="f2457-124">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="f2457-124">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f2457-125">буситипе</span><span class="sxs-lookup"><span data-stu-id="f2457-125">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="f2457-126">Представляет состояние занятости, заданное для события календаря.</span><span class="sxs-lookup"><span data-stu-id="f2457-126">Represents the free/busy status set for a calendar event.</span></span> <span data-ttu-id="f2457-127">Это обязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="f2457-127">This is a required child element.</span></span>  <br/> |
|[<span data-ttu-id="f2457-128">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="f2457-128">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="f2457-129">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="f2457-129">Provides additional information for a calendar event.</span></span> <span data-ttu-id="f2457-130">Это необязательный дочерний элемент.</span><span class="sxs-lookup"><span data-stu-id="f2457-130">This is an optional child element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f2457-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f2457-131">Parent elements</span></span>

|<span data-ttu-id="f2457-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f2457-132">**Element**</span></span>|<span data-ttu-id="f2457-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f2457-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f2457-134">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="f2457-134">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="f2457-135">Содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f2457-135">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> <span data-ttu-id="f2457-136">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="f2457-136">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f2457-137">Примечания</span><span class="sxs-lookup"><span data-stu-id="f2457-137">Remarks</span></span>

<span data-ttu-id="f2457-138">Время встреч и собраний возвращается в часовом поясе клиента.</span><span class="sxs-lookup"><span data-stu-id="f2457-138">The appointment and meeting times are returned in the time zone of the client.</span></span> <span data-ttu-id="f2457-139">Все дочерние элементы перечислены в той последовательности, в которой они выполняются.</span><span class="sxs-lookup"><span data-stu-id="f2457-139">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="f2457-140">Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.</span><span class="sxs-lookup"><span data-stu-id="f2457-140">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="f2457-141">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f2457-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f2457-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f2457-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f2457-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f2457-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f2457-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f2457-144">Schema Name</span></span>  <br/> |<span data-ttu-id="f2457-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f2457-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="f2457-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f2457-146">Validation File</span></span>  <br/> |<span data-ttu-id="f2457-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f2457-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f2457-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f2457-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="f2457-149">False</span><span class="sxs-lookup"><span data-stu-id="f2457-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f2457-150">См. также</span><span class="sxs-lookup"><span data-stu-id="f2457-150">See also</span></span>



[<span data-ttu-id="f2457-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f2457-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f2457-152">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f2457-152">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f2457-153">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f2457-153">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

