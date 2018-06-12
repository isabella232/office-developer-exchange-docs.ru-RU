---
title: Переходы между
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transitions
api_type:
- schema
ms.assetid: 26f38f1c-96a3-440e-805c-1437886d11c5
description: Переходы между элемент представляет массив переходы часового пояса.
ms.openlocfilehash: df7cacdef71c3fdfaa3ecadb486843ea30e6109d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840235"
---
# <a name="transitions"></a><span data-ttu-id="da769-103">Переходы между</span><span class="sxs-lookup"><span data-stu-id="da769-103">Transitions</span></span>

<span data-ttu-id="da769-104">**Переходы между** элемент представляет массив переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da769-104">The **Transitions** element represents an array of time zone transitions.</span></span> 
  
```xml
<Transitions Id="">
   <Transition/>
   <AbsoluteDateTransition/>
   <RecurringDayTransition/>
   <RecurringDateTransition/>
</Transitions>
```

 <span data-ttu-id="da769-105">**ArrayOfTransitionsType**</span><span class="sxs-lookup"><span data-stu-id="da769-105">**ArrayOfTransitionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da769-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da769-106">Attributes and elements</span></span>

<span data-ttu-id="da769-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="da769-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da769-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da769-108">Attributes</span></span>

|<span data-ttu-id="da769-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="da769-109">**Attribute**</span></span>|<span data-ttu-id="da769-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da769-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="da769-111">Id</span><span class="sxs-lookup"><span data-stu-id="da769-111">Id</span></span>  <br/> |<span data-ttu-id="da769-112">Представляет уникальный идентификатор определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da769-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="da769-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da769-113">Child elements</span></span>

|<span data-ttu-id="da769-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da769-114">**Element**</span></span>|<span data-ttu-id="da769-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da769-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da769-116">AbsoluteDateTransition</span><span class="sxs-lookup"><span data-stu-id="da769-116">AbsoluteDateTransition</span></span>](absolutedatetransition.md) <br/> |<span data-ttu-id="da769-117">Представляет переход часовой пояс, который создается в конкретный день и в определенное время.</span><span class="sxs-lookup"><span data-stu-id="da769-117">Represents a time zone transition that occurs on a specific date and at a specific time.</span></span>  <br/> |
|[<span data-ttu-id="da769-118">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="da769-118">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="da769-119">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="da769-119">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
|[<span data-ttu-id="da769-120">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="da769-120">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="da769-121">Представляет переход часового пояса, что происходит на указанном дня года.</span><span class="sxs-lookup"><span data-stu-id="da769-121">Represents a time zone transition that occurs on a specified day of the year.</span></span>  <br/> |
|[<span data-ttu-id="da769-122">Переход</span><span class="sxs-lookup"><span data-stu-id="da769-122">Transition</span></span>](transition.md) <br/> |<span data-ttu-id="da769-123">Представляет переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="da769-123">Represents a time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da769-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da769-124">Parent elements</span></span>

|<span data-ttu-id="da769-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da769-125">**Element**</span></span>|<span data-ttu-id="da769-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da769-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da769-127">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="da769-127">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="da769-128">Определяет часовой пояс для времени начала [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="da769-128">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="da769-129">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="da769-129">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="da769-130">Определяет часовой пояс для время окончания [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="da769-130">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="da769-131">Определение часового пояса</span><span class="sxs-lookup"><span data-stu-id="da769-131">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="da769-132">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="da769-132">Defines a time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da769-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="da769-133">Text value</span></span>

<span data-ttu-id="da769-134">Нет.</span><span class="sxs-lookup"><span data-stu-id="da769-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da769-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="da769-135">Remarks</span></span>

<span data-ttu-id="da769-136">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="da769-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da769-137">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da769-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da769-138">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da769-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da769-139">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da769-139">Schema Name</span></span>  <br/> |<span data-ttu-id="da769-140">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da769-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="da769-141">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da769-141">Validation File</span></span>  <br/> |<span data-ttu-id="da769-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da769-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da769-143">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da769-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="da769-144">False</span><span class="sxs-lookup"><span data-stu-id="da769-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da769-145">См. также</span><span class="sxs-lookup"><span data-stu-id="da769-145">See also</span></span>



- [<span data-ttu-id="da769-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="da769-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

