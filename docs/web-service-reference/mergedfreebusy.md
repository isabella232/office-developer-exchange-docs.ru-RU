---
title: MergedFreeBusy
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
description: Элемент MergedFreeBusy содержит объединенные занятости поток данных.
ms.openlocfilehash: 542b9fae0c36b0236bd806e8a9117753968e812c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834449"
---
# <a name="mergedfreebusy"></a><span data-ttu-id="f24b9-103">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="f24b9-103">MergedFreeBusy</span></span>

<span data-ttu-id="f24b9-104">Элемент **MergedFreeBusy** содержит объединенные занятости поток данных.</span><span class="sxs-lookup"><span data-stu-id="f24b9-104">The **MergedFreeBusy** element contains the merged free/busy stream of data.</span></span> 
  
[<span data-ttu-id="f24b9-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f24b9-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f24b9-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="f24b9-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f24b9-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="f24b9-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f24b9-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f24b9-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f24b9-109">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="f24b9-109">MergedFreeBusy</span></span>](mergedfreebusy.md)
  
```xml
<MergedFreeBusy>...</MergedFreeBusy>
```

 <span data-ttu-id="f24b9-110">**string**</span><span class="sxs-lookup"><span data-stu-id="f24b9-110">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f24b9-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f24b9-111">Attributes and elements</span></span>

<span data-ttu-id="f24b9-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f24b9-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f24b9-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f24b9-113">Attributes</span></span>

<span data-ttu-id="f24b9-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="f24b9-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f24b9-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f24b9-115">Child elements</span></span>

<span data-ttu-id="f24b9-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="f24b9-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f24b9-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f24b9-117">Parent elements</span></span>

|<span data-ttu-id="f24b9-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f24b9-118">**Element**</span></span>|<span data-ttu-id="f24b9-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f24b9-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f24b9-120">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="f24b9-120">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="f24b9-121">Содержит сведения о доступности для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="f24b9-121">Contains availability information for a specific user.</span></span>  <br/> <span data-ttu-id="f24b9-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="f24b9-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f24b9-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f24b9-123">Text value</span></span>

<span data-ttu-id="f24b9-124">Сервер предоставляет текстовое значение, если значение для элемента [FreeBusyViewType](freebusyviewtype.md) — это один из следующих:</span><span class="sxs-lookup"><span data-stu-id="f24b9-124">A text value is provided by the server if the value for the [FreeBusyViewType](freebusyviewtype.md) element is one of the following:</span></span> 
  
- <span data-ttu-id="f24b9-125">DetailedMerged</span><span class="sxs-lookup"><span data-stu-id="f24b9-125">DetailedMerged</span></span>
    
- <span data-ttu-id="f24b9-126">FreeBusyMerged</span><span class="sxs-lookup"><span data-stu-id="f24b9-126">FreeBusyMerged</span></span>
    
- <span data-ttu-id="f24b9-127">MergedOnly</span><span class="sxs-lookup"><span data-stu-id="f24b9-127">MergedOnly</span></span>
    
<span data-ttu-id="f24b9-128">Текстовое значение представляет собой поток сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="f24b9-128">The text value is a stream of free/busy information.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f24b9-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="f24b9-129">Remarks</span></span>

<span data-ttu-id="f24b9-130">Поток данных, представленные в этом элементе определяется элементов [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) и [значение TimeWindow](timewindow.md) .</span><span class="sxs-lookup"><span data-stu-id="f24b9-130">The stream of data provided by this element is defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) and [TimeWindow](timewindow.md) elements.</span></span> <span data-ttu-id="f24b9-131">Элемент [значение TimeWindow](timewindow.md) определяет период времени, запрос для обеспечения доступности.</span><span class="sxs-lookup"><span data-stu-id="f24b9-131">The [TimeWindow](timewindow.md) element defines the time span queried for availability.</span></span> <span data-ttu-id="f24b9-132">Элемент [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) определяет, как время из элемента [значение TimeWindow](timewindow.md) разбивается на интервалы, возвращаемых в элементе **MergedFreeBusy** .</span><span class="sxs-lookup"><span data-stu-id="f24b9-132">The [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element defines how the time from the [TimeWindow](timewindow.md) element is broken into intervals returned in the **MergedFreeBusy** element.</span></span> <span data-ttu-id="f24b9-133">Каждый номер в потоке **MergedFreeBusy** представляет один интервал, определенные в элементе [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) .</span><span class="sxs-lookup"><span data-stu-id="f24b9-133">Each number in the **MergedFreeBusy** stream represents a single interval defined by the [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element.</span></span> <span data-ttu-id="f24b9-134">В следующей таблице перечислены возможные значения для отдельных интервала.</span><span class="sxs-lookup"><span data-stu-id="f24b9-134">The following table lists the possible values for an individual interval.</span></span> 
  
|<span data-ttu-id="f24b9-135">**Цифры**</span><span class="sxs-lookup"><span data-stu-id="f24b9-135">**Digit**</span></span>|<span data-ttu-id="f24b9-136">**Доступность**</span><span class="sxs-lookup"><span data-stu-id="f24b9-136">**Availability**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f24b9-137">0</span><span class="sxs-lookup"><span data-stu-id="f24b9-137">0</span></span>  <br/> |<span data-ttu-id="f24b9-138">Свободна</span><span class="sxs-lookup"><span data-stu-id="f24b9-138">Free</span></span>  <br/> |
|<span data-ttu-id="f24b9-139">1</span><span class="sxs-lookup"><span data-stu-id="f24b9-139">1</span></span>  <br/> |<span data-ttu-id="f24b9-140">Под вопросом</span><span class="sxs-lookup"><span data-stu-id="f24b9-140">Tentative</span></span>  <br/> |
|<span data-ttu-id="f24b9-141">2</span><span class="sxs-lookup"><span data-stu-id="f24b9-141">2</span></span>  <br/> |<span data-ttu-id="f24b9-142">Занята</span><span class="sxs-lookup"><span data-stu-id="f24b9-142">Busy</span></span>  <br/> |
|<span data-ttu-id="f24b9-143">3</span><span class="sxs-lookup"><span data-stu-id="f24b9-143">3</span></span>  <br/> |<span data-ttu-id="f24b9-144">Нет на месте (OOF)</span><span class="sxs-lookup"><span data-stu-id="f24b9-144">Out of Office (OOF)</span></span>  <br/> |
|<span data-ttu-id="f24b9-145">4</span><span class="sxs-lookup"><span data-stu-id="f24b9-145">4</span></span>  <br/> |<span data-ttu-id="f24b9-146">Нет данных</span><span class="sxs-lookup"><span data-stu-id="f24b9-146">No data</span></span>  <br/> |
   
<span data-ttu-id="f24b9-147">Например запрос на данные о доступности включает в себя элемент [значение TimeWindow](timewindow.md) , представляющий четырех часов и [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) элемент, представляющий 60 минут.</span><span class="sxs-lookup"><span data-stu-id="f24b9-147">For example, a request for free/busy data includes a [TimeWindow](timewindow.md) element that represents four hours and a [MergedFreeBusyIntervalInMinutes](mergedfreebusyintervalinminutes.md) element that represents 60 minutes.</span></span> <span data-ttu-id="f24b9-148">Если календарь запрошенного пользователя об отсутствии на работе для первого 60 минут, «занят» для следующих 90 минут и незапланированной для окончательного 90 минут в окне времени в потоке **MergedFreeBusy** будет 3220.</span><span class="sxs-lookup"><span data-stu-id="f24b9-148">If the requested user's calendar is OOF for the first 60 minutes, busy for the following 90 minutes, and unscheduled for the final 90 minutes in the time window, the **MergedFreeBusy** stream will be 3220.</span></span> <span data-ttu-id="f24b9-149">Если интервал содержит более одного классификации доступности, самое большое число используется для классификации этого интервала.</span><span class="sxs-lookup"><span data-stu-id="f24b9-149">If an interval contains more than one availability classification, the highest number is used to classify that interval.</span></span> 
  
<span data-ttu-id="f24b9-150">Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="f24b9-150">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="f24b9-151">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f24b9-151">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f24b9-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f24b9-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f24b9-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f24b9-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f24b9-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f24b9-154">Schema Name</span></span>  <br/> |<span data-ttu-id="f24b9-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f24b9-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="f24b9-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f24b9-156">Validation File</span></span>  <br/> |<span data-ttu-id="f24b9-157">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f24b9-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f24b9-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f24b9-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="f24b9-159">False</span><span class="sxs-lookup"><span data-stu-id="f24b9-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f24b9-160">См. также</span><span class="sxs-lookup"><span data-stu-id="f24b9-160">See also</span></span>



[<span data-ttu-id="f24b9-161">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f24b9-161">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f24b9-162">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="f24b9-162">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f24b9-163">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f24b9-163">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

