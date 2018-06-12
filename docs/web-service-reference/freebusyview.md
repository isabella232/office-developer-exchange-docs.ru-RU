---
title: FreeBusyView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: Элемент FreeBusyView содержит сведения о доступности для конкретного пользователя.
ms.openlocfilehash: d0d603f18642a94e841a1a6bb8e8849aa6b5b273
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762660"
---
# <a name="freebusyview"></a><span data-ttu-id="584af-103">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="584af-103">FreeBusyView</span></span>

<span data-ttu-id="584af-104">Элемент **FreeBusyView** содержит сведения о доступности для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="584af-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="584af-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="584af-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="584af-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="584af-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="584af-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="584af-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="584af-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="584af-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="584af-109">**FreeBusyView**</span><span class="sxs-lookup"><span data-stu-id="584af-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="584af-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="584af-110">Attributes and elements</span></span>

<span data-ttu-id="584af-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="584af-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="584af-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="584af-112">Attributes</span></span>

<span data-ttu-id="584af-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="584af-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="584af-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="584af-114">Child elements</span></span>

|<span data-ttu-id="584af-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="584af-115">**Element**</span></span>|<span data-ttu-id="584af-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="584af-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="584af-117">FreeBusyViewType</span><span class="sxs-lookup"><span data-stu-id="584af-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="584af-118">Представляет тип запрошенные сведения о доступности, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="584af-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="584af-119">MergedFreeBusy</span><span class="sxs-lookup"><span data-stu-id="584af-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="584af-120">Содержит объединенные занятости поток данных.</span><span class="sxs-lookup"><span data-stu-id="584af-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="584af-121">CalendarEventArray</span><span class="sxs-lookup"><span data-stu-id="584af-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="584af-122">Содержит набор вхождений элемента уникальный календаря, которые представляют доступности запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="584af-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="584af-123">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="584af-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="584af-124">Представляет параметры часового пояса и рабочие часы для запрошенного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="584af-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="584af-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="584af-125">Parent elements</span></span>

|<span data-ttu-id="584af-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="584af-126">**Element**</span></span>|<span data-ttu-id="584af-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="584af-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="584af-128">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="584af-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="584af-129">Содержит сведения о доступности для одного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="584af-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="584af-130">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="584af-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="584af-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="584af-131">Remarks</span></span>

<span data-ttu-id="584af-132">Все дочерние элементы, перечислены в последовательности, в котором они изложены.</span><span class="sxs-lookup"><span data-stu-id="584af-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="584af-133">Уровень детализации, представленные в этом элементе зависит от разрешения, предоставленные для инициатора запроса.</span><span class="sxs-lookup"><span data-stu-id="584af-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="584af-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="584af-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="584af-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="584af-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="584af-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="584af-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="584af-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="584af-137">Schema Name</span></span>  <br/> |<span data-ttu-id="584af-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="584af-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="584af-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="584af-139">Validation File</span></span>  <br/> |<span data-ttu-id="584af-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="584af-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="584af-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="584af-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="584af-142">False</span><span class="sxs-lookup"><span data-stu-id="584af-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="584af-143">См. также</span><span class="sxs-lookup"><span data-stu-id="584af-143">See also</span></span>



[<span data-ttu-id="584af-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="584af-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="584af-145">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="584af-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="584af-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="584af-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

