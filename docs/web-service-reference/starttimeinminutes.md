---
title: StartTimeInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: Элемент StartTimeInMinutes представляет начала рабочего дня для пользователя почтового ящика.
ms.openlocfilehash: f3f1d26731d0406ff8a0fd45fc0243a9feabf886
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835558"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="dbbaa-103">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="dbbaa-103">StartTimeInMinutes</span></span>

<span data-ttu-id="dbbaa-104">Элемент **StartTimeInMinutes** представляет начала рабочего дня для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="dbbaa-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dbbaa-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="dbbaa-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="dbbaa-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="dbbaa-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="dbbaa-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="dbbaa-108">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="dbbaa-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="dbbaa-109">WorkingHours</span><span class="sxs-lookup"><span data-stu-id="dbbaa-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="dbbaa-110">WorkingPeriodArray</span><span class="sxs-lookup"><span data-stu-id="dbbaa-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="dbbaa-111">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="dbbaa-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="dbbaa-112">StartTimeInMinutes</span><span class="sxs-lookup"><span data-stu-id="dbbaa-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="dbbaa-113">**int**</span><span class="sxs-lookup"><span data-stu-id="dbbaa-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dbbaa-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dbbaa-114">Attributes and elements</span></span>

<span data-ttu-id="dbbaa-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dbbaa-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dbbaa-116">Attributes</span></span>

<span data-ttu-id="dbbaa-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dbbaa-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dbbaa-118">Child elements</span></span>

<span data-ttu-id="dbbaa-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dbbaa-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dbbaa-120">Parent elements</span></span>

|<span data-ttu-id="dbbaa-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dbbaa-121">**Element**</span></span>|<span data-ttu-id="dbbaa-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dbbaa-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dbbaa-123">WorkingPeriod</span><span class="sxs-lookup"><span data-stu-id="dbbaa-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="dbbaa-124">Содержит рабочей недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="dbbaa-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dbbaa-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dbbaa-126">Text value</span></span>

<span data-ttu-id="dbbaa-127">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-127">A text value is required.</span></span> <span data-ttu-id="dbbaa-128">Текстовое значение представляет начала рабочего дня, сколько минут, прошедшее с момента начала дня.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="dbbaa-129">Например время начала 8: 00</span><span class="sxs-lookup"><span data-stu-id="dbbaa-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="dbbaa-130">представлены 480 минут.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="dbbaa-131">Диапазон допустимых значений для этого элемента — 0 до 1440.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dbbaa-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="dbbaa-132">Remarks</span></span>

<span data-ttu-id="dbbaa-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dbbaa-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dbbaa-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dbbaa-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dbbaa-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dbbaa-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dbbaa-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dbbaa-136">Schema Name</span></span>  <br/> |<span data-ttu-id="dbbaa-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dbbaa-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="dbbaa-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dbbaa-138">Validation File</span></span>  <br/> |<span data-ttu-id="dbbaa-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dbbaa-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dbbaa-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dbbaa-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="dbbaa-141">False</span><span class="sxs-lookup"><span data-stu-id="dbbaa-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dbbaa-142">См. также</span><span class="sxs-lookup"><span data-stu-id="dbbaa-142">See also</span></span>

- [<span data-ttu-id="dbbaa-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="dbbaa-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="dbbaa-144">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="dbbaa-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="dbbaa-145">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="dbbaa-145">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

