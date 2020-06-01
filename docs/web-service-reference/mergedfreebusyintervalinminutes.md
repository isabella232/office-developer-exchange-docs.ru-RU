---
title: мержедфрибусинтервалинминутес
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
description: Элемент Мержедфрибусинтервалинминутес представляет разницу во времени между двумя последовательными слотами в представлении Фрибусимержед.
ms.openlocfilehash: 6228ee5b66202634e6bb3b6c1ad6b8897a109d58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468791"
---
# <a name="mergedfreebusyintervalinminutes"></a><span data-ttu-id="8306c-103">мержедфрибусинтервалинминутес</span><span class="sxs-lookup"><span data-stu-id="8306c-103">MergedFreeBusyIntervalInMinutes</span></span>

<span data-ttu-id="8306c-104">Элемент **мержедфрибусинтервалинминутес** представляет разницу во времени между двумя последовательными слотами в представлении **фрибусимержед** .</span><span class="sxs-lookup"><span data-stu-id="8306c-104">The **MergedFreeBusyIntervalInMinutes** element represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span> 
  
[<span data-ttu-id="8306c-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="8306c-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="8306c-106">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="8306c-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="8306c-107">мержедфрибусинтервалинминутес</span><span class="sxs-lookup"><span data-stu-id="8306c-107">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md)
  
```xml
<MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
```

 <span data-ttu-id="8306c-108">**int**</span><span class="sxs-lookup"><span data-stu-id="8306c-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8306c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8306c-109">Attributes and elements</span></span>

<span data-ttu-id="8306c-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8306c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8306c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8306c-111">Attributes</span></span>

<span data-ttu-id="8306c-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8306c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8306c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8306c-113">Child elements</span></span>

<span data-ttu-id="8306c-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8306c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8306c-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8306c-115">Parent elements</span></span>

|<span data-ttu-id="8306c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8306c-116">**Element**</span></span>|<span data-ttu-id="8306c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8306c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8306c-118">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="8306c-118">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="8306c-119">Указывает тип сведений о доступности, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="8306c-119">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="8306c-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8306c-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8306c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8306c-121">Text value</span></span>

<span data-ttu-id="8306c-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="8306c-122">A text value is required.</span></span> <span data-ttu-id="8306c-123">Текстовое значение представляет время в минутах.</span><span class="sxs-lookup"><span data-stu-id="8306c-123">The text value represents time in minutes.</span></span> <span data-ttu-id="8306c-124">Значение по умолчанию  30 минут.</span><span class="sxs-lookup"><span data-stu-id="8306c-124">The default value is 30 minutes.</span></span> <span data-ttu-id="8306c-125">Шесть минут — это минимальный интервал и один день (1440 минут) — это максимальный интервал для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8306c-125">Six minutes is the minimum interval and one day (1440 minutes) is the maximum interval for this element.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8306c-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="8306c-126">Remarks</span></span>

<span data-ttu-id="8306c-127">Это значение используется только в том случае, если элемент [рекуестедвиев](requestedview.md) равен **мержедонли**, **фрибусимержед**или **детаиледмерже**.</span><span class="sxs-lookup"><span data-stu-id="8306c-127">This value is used only if the [RequestedView](requestedview.md) element is equal to **MergedOnly**, **FreeBusyMerged**, or **DetailedMerge**.</span></span> <span data-ttu-id="8306c-128">Это тип данных Integer.</span><span class="sxs-lookup"><span data-stu-id="8306c-128">This is an integer data type.</span></span> <span data-ttu-id="8306c-129">Поток, содержащий интервалы, заданные этим элементом, возвращается в элементе [мержедфрибуси](mergedfreebusy.md) .</span><span class="sxs-lookup"><span data-stu-id="8306c-129">The stream that contains the intervals defined by this element is returned in the [MergedFreeBusy](mergedfreebusy.md) element.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8306c-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8306c-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8306c-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8306c-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8306c-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8306c-132">Schema Name</span></span>  <br/> |<span data-ttu-id="8306c-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8306c-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="8306c-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8306c-134">Validation File</span></span>  <br/> |<span data-ttu-id="8306c-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8306c-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8306c-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8306c-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="8306c-137">False</span><span class="sxs-lookup"><span data-stu-id="8306c-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8306c-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8306c-138">See also</span></span>



[<span data-ttu-id="8306c-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8306c-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="8306c-140">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="8306c-140">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)


[<span data-ttu-id="8306c-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="8306c-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

