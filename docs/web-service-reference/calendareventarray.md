---
title: календаревентаррай
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
description: Элемент Календаревентаррай содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.
ms.openlocfilehash: 6badba2477a9d48c6d109740de454e2815d3c211
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463372"
---
# <a name="calendareventarray"></a><span data-ttu-id="4d250-103">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="4d250-103">CalendarEventArray</span></span>

<span data-ttu-id="4d250-104">Элемент **календаревентаррай** содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d250-104">The **CalendarEventArray** element contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span> 
  
[<span data-ttu-id="4d250-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="4d250-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="4d250-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="4d250-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="4d250-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="4d250-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="4d250-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="4d250-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="4d250-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="4d250-109">CalendarEventArray</span></span>](calendareventarray.md)
  
```xml
<CalendarEventArray>
   <CalendarEvent>...</CalendarEvent>
</CalendarEventArray>
```

 <span data-ttu-id="4d250-110">**аррайофкалендаревент**</span><span class="sxs-lookup"><span data-stu-id="4d250-110">**ArrayOfCalendarEvent**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d250-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d250-111">Attributes and elements</span></span>

<span data-ttu-id="4d250-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4d250-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d250-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d250-113">Attributes</span></span>

<span data-ttu-id="4d250-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d250-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d250-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d250-115">Child elements</span></span>

|<span data-ttu-id="4d250-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d250-116">**Element**</span></span>|<span data-ttu-id="4d250-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d250-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d250-118">календаревент</span><span class="sxs-lookup"><span data-stu-id="4d250-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="4d250-119">Представляет уникальное вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="4d250-119">Represents a unique calendar item occurrence.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d250-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d250-120">Parent elements</span></span>

|<span data-ttu-id="4d250-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d250-121">**Element**</span></span>|<span data-ttu-id="4d250-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d250-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d250-123">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="4d250-123">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="4d250-124">Содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="4d250-124">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="4d250-125">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="4d250-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d250-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="4d250-126">Remarks</span></span>

<span data-ttu-id="4d250-127">Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.</span><span class="sxs-lookup"><span data-stu-id="4d250-127">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span> <span data-ttu-id="4d250-128">Этот элемент включается, если для элемента [фрибусивиевтипе](freebusyviewtype.md) задано **значение FreeBusy**, **Фрибусимержед**, **Detailed**или **детаиледмержед**.</span><span class="sxs-lookup"><span data-stu-id="4d250-128">This element is included when the [FreeBusyViewType](freebusyviewtype.md) element is set to **FreeBusy**, **FreeBusyMerged**, **Detailed**, or **DetailedMerged**.</span></span> <span data-ttu-id="4d250-129">Этот элемент не включает никакие дочерние элементы, если в окне запрошенного времени нет элементов календаря.</span><span class="sxs-lookup"><span data-stu-id="4d250-129">This element does not include any child elements if no calendar items are present in the requested time window.</span></span> 
  
<span data-ttu-id="4d250-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4d250-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d250-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d250-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d250-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d250-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d250-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d250-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4d250-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4d250-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d250-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d250-135">Validation File</span></span>  <br/> |<span data-ttu-id="4d250-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4d250-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d250-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d250-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="4d250-138">False</span><span class="sxs-lookup"><span data-stu-id="4d250-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d250-139">См. также</span><span class="sxs-lookup"><span data-stu-id="4d250-139">See also</span></span>



[<span data-ttu-id="4d250-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="4d250-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="4d250-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="4d250-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="4d250-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="4d250-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

