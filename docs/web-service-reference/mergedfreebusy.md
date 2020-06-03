---
title: мержедфрибуси
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusy
api_type:
- schema
ms.assetid: ea45590d-476e-4b68-9fe8-ae392feadfea
description: Элемент Мержедфрибуси содержит Объединенный поток данных о занятости.
ms.openlocfilehash: a1483449534f0d886e3c97a23d28c5d78f865042
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468728"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="ed77e-103">мержедфрибуси</span><span class="sxs-lookup"><span data-stu-id="ed77e-103">MergedFreeBusy</span></span>

<span data-ttu-id="ed77e-104">Элемент **мержедфрибуси** содержит Объединенный поток данных о занятости.</span><span class="sxs-lookup"><span data-stu-id="ed77e-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="ed77e-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ed77e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ed77e-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="ed77e-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ed77e-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ed77e-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ed77e-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="ed77e-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ed77e-109">мержедфрибуси</span><span class="sxs-lookup"><span data-stu-id="ed77e-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="ed77e-110">**строка**</span><span class="sxs-lookup"><span data-stu-id="ed77e-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ed77e-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ed77e-111">Attributes and elements</span></span>

<span data-ttu-id="ed77e-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ed77e-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ed77e-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ed77e-113">Attributes</span></span>

<span data-ttu-id="ed77e-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ed77e-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ed77e-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ed77e-115">Child elements</span></span>

<span data-ttu-id="ed77e-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ed77e-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ed77e-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ed77e-117">Parent elements</span></span>

|<span data-ttu-id="ed77e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ed77e-118">**Element**</span></span>|<span data-ttu-id="ed77e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ed77e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ed77e-120">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="ed77e-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="ed77e-121">Содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="ed77e-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="ed77e-122">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ed77e-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ed77e-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ed77e-123">Text value</span></span>

<span data-ttu-id="ed77e-124">Текстовое значение предоставляется сервером, если для элемента [фрибусивиевтипе](freebusyviewtype.md) задано одно из следующих значений:</span><span class="sxs-lookup"><span data-stu-id="ed77e-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="ed77e-125">детаиледмержед</span><span class="sxs-lookup"><span data-stu-id="ed77e-125">DetailedMerged</span></span>
    
- <span data-ttu-id="ed77e-126">фрибусимержед</span><span class="sxs-lookup"><span data-stu-id="ed77e-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="ed77e-127">мержедонли</span><span class="sxs-lookup"><span data-stu-id="ed77e-127">MergedOnly</span></span>
    
<span data-ttu-id="ed77e-128">Текстовое значение — это поток сведений о занятости.</span><span class="sxs-lookup"><span data-stu-id="ed77e-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ed77e-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="ed77e-129">Remarks</span></span>

<span data-ttu-id="ed77e-130">Поток данных, предоставляемых этим элементом, определяется элементами [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) и [TimeWindow](timewindow.md) .</span><span class="sxs-lookup"><span data-stu-id="ed77e-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="ed77e-131">Элемент [TimeWindow](timewindow.md) определяет временной интервал, запрашиваемый для обеспечения доступности.</span><span class="sxs-lookup"><span data-stu-id="ed77e-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="ed77e-132">Элемент [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) определяет, как время из элемента [TimeWindow](timewindow.md) разбивается на интервалы, возвращаемые в элементе **мержедфрибуси** .</span><span class="sxs-lookup"><span data-stu-id="ed77e-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="ed77e-133">Каждое число в потоке **мержедфрибуси** представляет собой один интервал, заданный элементом [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) .</span><span class="sxs-lookup"><span data-stu-id="ed77e-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="ed77e-134">В следующей таблице перечислены возможные значения для отдельного интервала.</span><span class="sxs-lookup"><span data-stu-id="ed77e-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="ed77e-135">**Четырехзначные**</span><span class="sxs-lookup"><span data-stu-id="ed77e-135">**Digit**</span></span>|<span data-ttu-id="ed77e-136">**Доступность**</span><span class="sxs-lookup"><span data-stu-id="ed77e-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ed77e-137">нуль</span><span class="sxs-lookup"><span data-stu-id="ed77e-137">0</span></span>  <br/> |<span data-ttu-id="ed77e-138">Свободна</span><span class="sxs-lookup"><span data-stu-id="ed77e-138">Free</span></span>  <br/> |
|<span data-ttu-id="ed77e-139">1 </span><span class="sxs-lookup"><span data-stu-id="ed77e-139">1</span></span>  <br/> |<span data-ttu-id="ed77e-140">Занят</span><span class="sxs-lookup"><span data-stu-id="ed77e-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="ed77e-141">2</span><span class="sxs-lookup"><span data-stu-id="ed77e-141">2</span></span>  <br/> |<span data-ttu-id="ed77e-142">Занята</span><span class="sxs-lookup"><span data-stu-id="ed77e-142">Busy</span></span>  <br/> |
|<span data-ttu-id="ed77e-143">4</span><span class="sxs-lookup"><span data-stu-id="ed77e-143">3</span></span>  <br/> |<span data-ttu-id="ed77e-144">Отсутствие на работе (OOF)</span><span class="sxs-lookup"><span data-stu-id="ed77e-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="ed77e-145">4 </span><span class="sxs-lookup"><span data-stu-id="ed77e-145">4</span></span>  <br/> |<span data-ttu-id="ed77e-146">Нет данных</span><span class="sxs-lookup"><span data-stu-id="ed77e-146">No data</span></span>  <br/> |
   
<span data-ttu-id="ed77e-147">Например, запрос данных о занятости содержит элемент [TimeWindow](timewindow.md) , который представляет четыре часа и элемент [мержедфрибусинтервалинминутес](mergedfreebusyintervalinminutes.md) , представляющий 60 минут.</span><span class="sxs-lookup"><span data-stu-id="ed77e-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="ed77e-148">Если запрашиваемый календарь пользователя не работает в течение первых 60 минут, он занят в течение следующих 90 минут и незапланированный для конечной 90 минут в окне времени, поток **мержедфрибуси** будет равен 3220.</span><span class="sxs-lookup"><span data-stu-id="ed77e-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="ed77e-149">Если интервал содержит более одной классификации доступности, для классификации этого интервала используется самый высокий номер.</span><span class="sxs-lookup"><span data-stu-id="ed77e-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="ed77e-150">Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.</span><span class="sxs-lookup"><span data-stu-id="ed77e-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="ed77e-151">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ed77e-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ed77e-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ed77e-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ed77e-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ed77e-153">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ed77e-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ed77e-154">Schema Name</span></span>  <br/> |<span data-ttu-id="ed77e-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ed77e-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="ed77e-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ed77e-156">Validation File</span></span>  <br/> |<span data-ttu-id="ed77e-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ed77e-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ed77e-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ed77e-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="ed77e-159">False</span><span class="sxs-lookup"><span data-stu-id="ed77e-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ed77e-160">См. также</span><span class="sxs-lookup"><span data-stu-id="ed77e-160">See also</span></span>



[<span data-ttu-id="ed77e-161">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ed77e-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ed77e-162">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ed77e-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ed77e-163">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="ed77e-163">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

