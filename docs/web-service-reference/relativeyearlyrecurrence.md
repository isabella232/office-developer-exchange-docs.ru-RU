---
title: RelativeYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeYearlyRecurrence
api_type:
- schema
ms.assetid: 25b67876-9979-4a30-a637-357ea10a93b8
description: Элемент RelativeYearlyRecurrence описывает относительное ежегодно повторяющейся.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835057"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="004bb-103">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="004bb-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="004bb-104">Элемент **RelativeYearlyRecurrence** описывает относительное ежегодно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="004bb-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="004bb-105">**RelativeYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="004bb-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="004bb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="004bb-106">Attributes and elements</span></span>

<span data-ttu-id="004bb-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="004bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="004bb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="004bb-108">Attributes</span></span>

<span data-ttu-id="004bb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="004bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="004bb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="004bb-110">Child elements</span></span>

|<span data-ttu-id="004bb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="004bb-111">**Element**</span></span>|<span data-ttu-id="004bb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="004bb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="004bb-113">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="004bb-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="004bb-114">Описывает дни недели, используемые в расписаниях повторов элемента.</span><span class="sxs-lookup"><span data-stu-id="004bb-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="004bb-115">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="004bb-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="004bb-116">Описывает неделю в месяц используется в относительный ежегодно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="004bb-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="004bb-117">Месяц (повторение элемента)</span><span class="sxs-lookup"><span data-stu-id="004bb-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="004bb-118">Описывает месяц, когда ежегодно повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="004bb-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="004bb-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="004bb-119">Parent elements</span></span>

|<span data-ttu-id="004bb-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="004bb-120">**Element**</span></span>|<span data-ttu-id="004bb-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="004bb-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="004bb-122">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="004bb-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="004bb-123">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="004bb-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="004bb-124">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="004bb-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="004bb-125">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="004bb-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="004bb-126">Стандартный</span><span class="sxs-lookup"><span data-stu-id="004bb-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="004bb-127">Представляет дату и время изменения времени с летнего времени на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="004bb-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="004bb-128">Переход на летнее</span><span class="sxs-lookup"><span data-stu-id="004bb-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="004bb-129">Представляет дату и время изменения времени с зимнего на летнее время.</span><span class="sxs-lookup"><span data-stu-id="004bb-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="004bb-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="004bb-130">Remarks</span></span>

<span data-ttu-id="004bb-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="004bb-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="004bb-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="004bb-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="004bb-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="004bb-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="004bb-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="004bb-134">Schema Name</span></span>  <br/> |<span data-ttu-id="004bb-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="004bb-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="004bb-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="004bb-136">Validation File</span></span>  <br/> |<span data-ttu-id="004bb-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="004bb-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="004bb-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="004bb-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="004bb-139">False</span><span class="sxs-lookup"><span data-stu-id="004bb-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="004bb-140">См. также</span><span class="sxs-lookup"><span data-stu-id="004bb-140">See also</span></span>



- [<span data-ttu-id="004bb-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="004bb-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

