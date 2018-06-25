---
title: WeeklyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WeeklyRecurrence
api_type:
- schema
ms.assetid: 69c41dd5-597c-45bc-be3f-e2f2b5615aa3
description: Элемент WeeklyRecurrence описывает еженедельно повторяющейся.
ms.openlocfilehash: 78bc76dd63c6737786df02f336217dc8de9a3a67
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840505"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="b07c4-103">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="b07c4-103">WeeklyRecurrence</span></span>

<span data-ttu-id="b07c4-104">Элемент **WeeklyRecurrence** описывает еженедельно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="b07c4-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="b07c4-105">**WeeklyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="b07c4-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b07c4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b07c4-106">Attributes and elements</span></span>

<span data-ttu-id="b07c4-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="b07c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b07c4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b07c4-108">Attributes</span></span>

<span data-ttu-id="b07c4-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="b07c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b07c4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b07c4-110">Child elements</span></span>

|<span data-ttu-id="b07c4-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b07c4-111">**Element**</span></span>|<span data-ttu-id="b07c4-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b07c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b07c4-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="b07c4-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="b07c4-114">Задает интервал в недель между двумя последовательными еженедельно повторения шаблон элементов.</span><span class="sxs-lookup"><span data-stu-id="b07c4-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="b07c4-115">Значение может быть в диапазоне от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="b07c4-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="b07c4-116">DaysOfWeek (DaysOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="b07c4-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="b07c4-117">Описывается, какие дни недели, в неделю шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="b07c4-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="b07c4-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="b07c4-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="b07c4-119">Задает первый день недели.</span><span class="sxs-lookup"><span data-stu-id="b07c4-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b07c4-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b07c4-120">Parent elements</span></span>

|<span data-ttu-id="b07c4-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b07c4-121">**Element**</span></span>|<span data-ttu-id="b07c4-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b07c4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b07c4-123">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b07c4-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="b07c4-124">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="b07c4-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="b07c4-125">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="b07c4-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="b07c4-126">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="b07c4-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b07c4-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b07c4-127">Text value</span></span>

<span data-ttu-id="b07c4-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="b07c4-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b07c4-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="b07c4-129">Remarks</span></span>

<span data-ttu-id="b07c4-130">[Запуск](start.md) и [конечной](end-ex15websvcsotherref.md) дат повторяющегося элемента шаблона, у которых дата, равный первого появления еженедельно повторяющейся информации смещение часового пояса будут потеряны.</span><span class="sxs-lookup"><span data-stu-id="b07c4-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="b07c4-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b07c4-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b07c4-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b07c4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b07c4-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b07c4-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b07c4-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b07c4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="b07c4-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b07c4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="b07c4-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b07c4-136">Validation File</span></span>  <br/> |<span data-ttu-id="b07c4-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="b07c4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b07c4-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b07c4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="b07c4-139">False</span><span class="sxs-lookup"><span data-stu-id="b07c4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b07c4-140">См. также</span><span class="sxs-lookup"><span data-stu-id="b07c4-140">See also</span></span>



- [<span data-ttu-id="b07c4-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b07c4-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

