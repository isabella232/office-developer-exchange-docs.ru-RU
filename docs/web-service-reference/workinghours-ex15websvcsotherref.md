---
title: воркингхаурс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingHours
api_type:
- schema
ms.assetid: bbe97777-f728-46c5-b2aa-565112c24f3a
description: Элемент Воркингхаурс представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.
ms.openlocfilehash: 9cb21e72f7024b96b4b5f252a8a3b85bb704e67c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468343"
---
# <a name="workinghours"></a><span data-ttu-id="c1ff2-103">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="c1ff2-103">WorkingHours</span></span>

<span data-ttu-id="c1ff2-104">Элемент **воркингхаурс** представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-104">The **WorkingHours** element represents the time zone settings and working hours for the requested mailbox user.</span></span> 
  
[<span data-ttu-id="c1ff2-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c1ff2-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="c1ff2-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="c1ff2-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="c1ff2-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c1ff2-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="c1ff2-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="c1ff2-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="c1ff2-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="c1ff2-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
```xml
<WorkingHours>
   <TimeZone>...</TimeZone>
   <WorkingPeriodArray>...</WorkingPeriodArray>
</WorkingHours>
```

 <span data-ttu-id="c1ff2-110">**воркингхаурс**</span><span class="sxs-lookup"><span data-stu-id="c1ff2-110">**WorkingHours**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c1ff2-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c1ff2-111">Attributes and elements</span></span>

<span data-ttu-id="c1ff2-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c1ff2-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c1ff2-113">Attributes</span></span>

<span data-ttu-id="c1ff2-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c1ff2-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c1ff2-115">Child elements</span></span>

|<span data-ttu-id="c1ff2-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1ff2-116">**Element**</span></span>|<span data-ttu-id="c1ff2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1ff2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1ff2-118">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="c1ff2-118">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="c1ff2-119">Содержит элементы, определяющие сведения о часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-119">Contains elements that identify time zone information.</span></span> <span data-ttu-id="c1ff2-120">Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-120">This element also contains information about the transition between standard time and daylight saving time.</span></span> <span data-ttu-id="c1ff2-121">Этот элемент является обязательным, если используется элемент **воркингхаурс** .</span><span class="sxs-lookup"><span data-stu-id="c1ff2-121">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
|[<span data-ttu-id="c1ff2-122">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="c1ff2-122">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="c1ff2-123">Содержит сведения о рабочем периоде для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-123">Contains working period information for the mailbox user.</span></span> <span data-ttu-id="c1ff2-124">Этот элемент является обязательным, если используется элемент **воркингхаурс** .</span><span class="sxs-lookup"><span data-stu-id="c1ff2-124">This element is required if the **WorkingHours** element is used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c1ff2-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c1ff2-125">Parent elements</span></span>

|<span data-ttu-id="c1ff2-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c1ff2-126">**Element**</span></span>|<span data-ttu-id="c1ff2-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c1ff2-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c1ff2-128">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="c1ff2-128">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="c1ff2-129">Содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-129">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="c1ff2-130">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="c1ff2-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c1ff2-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="c1ff2-131">Remarks</span></span>

<span data-ttu-id="c1ff2-132">Все дочерние элементы перечислены в той последовательности, в которой они выполняются.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="c1ff2-133">Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="c1ff2-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c1ff2-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c1ff2-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c1ff2-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c1ff2-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c1ff2-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c1ff2-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c1ff2-137">Schema Name</span></span>  <br/> |<span data-ttu-id="c1ff2-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c1ff2-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="c1ff2-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c1ff2-139">Validation File</span></span>  <br/> |<span data-ttu-id="c1ff2-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c1ff2-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c1ff2-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c1ff2-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="c1ff2-142">False</span><span class="sxs-lookup"><span data-stu-id="c1ff2-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c1ff2-143">См. также</span><span class="sxs-lookup"><span data-stu-id="c1ff2-143">See also</span></span>



[<span data-ttu-id="c1ff2-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c1ff2-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="c1ff2-145">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c1ff2-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="c1ff2-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="c1ff2-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

