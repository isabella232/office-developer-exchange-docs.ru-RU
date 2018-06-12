---
title: MergedFreeBusyIntervalInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MergedFreeBusyIntervalInMinutes
api_type:
- schema
ms.assetid: 481cdbc6-d5aa-49fa-a3fa-9d119d3dca99
description: Элемент MergedFreeBusyIntervalInMinutes представляет разницу между двумя последовательными разъемов FreeBusyMerged представления.
ms.openlocfilehash: 99c8c69424a0a9d9594005fdf6b2ceba53e6288a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834451"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="1955f-103">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="1955f-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="1955f-104">Элемент **MergedFreeBusyIntervalInMinutes** представляет разницу между двумя последовательными разъемов **FreeBusyMerged** представления.</span><span class="sxs-lookup"><span data-stu-id="1955f-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="1955f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="1955f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="1955f-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="1955f-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="1955f-107">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="1955f-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="1955f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="1955f-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1955f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1955f-109">Attributes and elements</span></span>

<span data-ttu-id="1955f-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1955f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1955f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1955f-111">Attributes</span></span>

<span data-ttu-id="1955f-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="1955f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1955f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1955f-113">Child elements</span></span>

<span data-ttu-id="1955f-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="1955f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1955f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1955f-115">Parent elements</span></span>

|<span data-ttu-id="1955f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1955f-116">**Element**</span></span>|<span data-ttu-id="1955f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1955f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1955f-118">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="1955f-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="1955f-119">Указывает тип сведений о доступности, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="1955f-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="1955f-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="1955f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1955f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1955f-121">Text value</span></span>

<span data-ttu-id="1955f-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="1955f-122">A text value is required.</span></span> <span data-ttu-id="1955f-123">Текстовое значение представляет время в минутах.</span><span class="sxs-lookup"><span data-stu-id="1955f-123">The text value represents time in minutes.</span></span> <span data-ttu-id="1955f-124">Значение по умолчанию — 30 минут.</span><span class="sxs-lookup"><span data-stu-id="1955f-124">The default value is 30 minutes.</span></span> <span data-ttu-id="1955f-125">Шесть минут — минимальный интервал и один день (1440 минут) — это максимальный интервал для данного элемента.</span><span class="sxs-lookup"><span data-stu-id="1955f-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1955f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="1955f-126">Remarks</span></span>

<span data-ttu-id="1955f-127">Это значение используется только в том случае, если элемент [RequestedView](requestedview.md) равен **MergedOnly**, **FreeBusyMerged**или **DetailedMerge**.</span><span class="sxs-lookup"><span data-stu-id="1955f-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="1955f-128">Это тип данных integer.</span><span class="sxs-lookup"><span data-stu-id="1955f-128">This is an integer data type.</span></span> <span data-ttu-id="1955f-129">Поток, содержащий интервалы, определенные этим элементом, возвращается в элементе [MergedFreeBusy](mergedfreebusy.md) .</span><span class="sxs-lookup"><span data-stu-id="1955f-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1955f-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1955f-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1955f-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1955f-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1955f-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1955f-132">Schema Name</span></span>  <br/> |<span data-ttu-id="1955f-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1955f-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="1955f-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1955f-134">Validation File</span></span>  <br/> |<span data-ttu-id="1955f-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1955f-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1955f-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1955f-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="1955f-137">False</span><span class="sxs-lookup"><span data-stu-id="1955f-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1955f-138">См. также</span><span class="sxs-lookup"><span data-stu-id="1955f-138">See also</span></span>



[<span data-ttu-id="1955f-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1955f-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1955f-140">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="1955f-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="1955f-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="1955f-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

