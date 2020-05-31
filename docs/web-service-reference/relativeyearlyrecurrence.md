---
title: релативэйеарлирекурренце
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
description: Элемент Релативэйеарлирекурренце описывает относительный ежегодный шаблон повторения.
ms.openlocfilehash: ce8d2b134ce1fa34cbce8bd2fa921cab18d908a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835057"
---
# <a name="relativeyearlyrecurrence"></a><span data-ttu-id="bd95c-103">релативэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="bd95c-103">RelativeYearlyRecurrence</span></span>

<span data-ttu-id="bd95c-104">Элемент **релативэйеарлирекурренце** описывает относительный ежегодный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="bd95c-104">The **RelativeYearlyRecurrence** element describes a relative yearly recurrence pattern.</span></span> 
  
```xml
<RelativeYearlyRecurrence>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
   <Month/>
</RelativeYearlyRecurrence>
```

 <span data-ttu-id="bd95c-105">**релативэйеарлирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="bd95c-105">**RelativeYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bd95c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bd95c-106">Attributes and elements</span></span>

<span data-ttu-id="bd95c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bd95c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bd95c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bd95c-108">Attributes</span></span>

<span data-ttu-id="bd95c-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bd95c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bd95c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bd95c-110">Child elements</span></span>

|<span data-ttu-id="bd95c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd95c-111">**Element**</span></span>|<span data-ttu-id="bd95c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd95c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd95c-113">DaysOfWeek (Дайофвиктипе)</span><span class="sxs-lookup"><span data-stu-id="bd95c-113">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="bd95c-114">Описывает дни недели, которые используются в шаблонах повторения элементов.</span><span class="sxs-lookup"><span data-stu-id="bd95c-114">Describes the days of the week that are used in item recurrence patterns.</span></span>  <br/> |
|[<span data-ttu-id="bd95c-115">дайофвикиндекс</span><span class="sxs-lookup"><span data-stu-id="bd95c-115">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="bd95c-116">Описывает, какая неделя месяца используется в качестве относительного ежегодного повторения.</span><span class="sxs-lookup"><span data-stu-id="bd95c-116">Describes which week in a month is used in a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="bd95c-117">Month (повторение элемента)</span><span class="sxs-lookup"><span data-stu-id="bd95c-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="bd95c-118">Описывает месяц, когда происходит ежегодно повторяющийся элемент.</span><span class="sxs-lookup"><span data-stu-id="bd95c-118">Describes the month when a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bd95c-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bd95c-119">Parent elements</span></span>

|<span data-ttu-id="bd95c-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bd95c-120">**Element**</span></span>|<span data-ttu-id="bd95c-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bd95c-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bd95c-122">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="bd95c-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="bd95c-123">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="bd95c-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="bd95c-124">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="bd95c-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="bd95c-125">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="bd95c-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="bd95c-126">Standard</span><span class="sxs-lookup"><span data-stu-id="bd95c-126">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="bd95c-127">Представляет дату и время изменения времени с летнего на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="bd95c-127">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="bd95c-128">Переход</span><span class="sxs-lookup"><span data-stu-id="bd95c-128">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="bd95c-129">Представляет дату и время изменения времени со стандартного времени на летнее.</span><span class="sxs-lookup"><span data-stu-id="bd95c-129">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bd95c-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="bd95c-130">Remarks</span></span>

<span data-ttu-id="bd95c-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bd95c-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bd95c-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bd95c-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bd95c-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bd95c-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bd95c-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bd95c-134">Schema Name</span></span>  <br/> |<span data-ttu-id="bd95c-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bd95c-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="bd95c-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bd95c-136">Validation File</span></span>  <br/> |<span data-ttu-id="bd95c-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bd95c-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bd95c-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bd95c-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="bd95c-139">False</span><span class="sxs-lookup"><span data-stu-id="bd95c-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bd95c-140">См. также</span><span class="sxs-lookup"><span data-stu-id="bd95c-140">See also</span></span>



- [<span data-ttu-id="bd95c-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bd95c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

