---
title: виклирекурренце
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
description: Элемент Виклирекурренце описывает еженедельный шаблон повторения.
ms.openlocfilehash: 5006238590c4cd7556a92fb1fbe13292383412b8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530368"
---
# <a name="weeklyrecurrence"></a><span data-ttu-id="300db-103">виклирекурренце</span><span class="sxs-lookup"><span data-stu-id="300db-103">WeeklyRecurrence</span></span>

<span data-ttu-id="300db-104">Элемент **виклирекурренце** описывает еженедельный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="300db-104">The **WeeklyRecurrence** element describes a weekly recurrence pattern.</span></span> 
  
```XML
<WeeklyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <FirstDayOfWeek/>
</WeeklyRecurrence>
```

 <span data-ttu-id="300db-105">**виклирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="300db-105">**WeeklyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="300db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="300db-106">Attributes and elements</span></span>

<span data-ttu-id="300db-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="300db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="300db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="300db-108">Attributes</span></span>

<span data-ttu-id="300db-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="300db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="300db-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="300db-110">Child elements</span></span>

|<span data-ttu-id="300db-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="300db-111">**Element**</span></span>|<span data-ttu-id="300db-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="300db-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="300db-113">Interval</span><span class="sxs-lookup"><span data-stu-id="300db-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="300db-114">Определяет интервал (в неделях) между двумя последовательными еженедельными элементами расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="300db-114">Defines the interval, in weeks, between two consecutive weekly recurrence pattern items.</span></span> <span data-ttu-id="300db-115">Значение может находиться в диапазоне от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="300db-115">The value can be in the range from 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="300db-116">DaysOfWeek (Дайсофвиктипе)</span><span class="sxs-lookup"><span data-stu-id="300db-116">DaysOfWeek (DaysOfWeekType)</span></span>](daysofweek-daysofweektype.md) <br/> |<span data-ttu-id="300db-117">Описывает дни недели в расписании повторения.</span><span class="sxs-lookup"><span data-stu-id="300db-117">Describes which days of the week are in the weekly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="300db-118">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="300db-118">FirstDayOfWeek</span></span>](firstdayofweek.md) <br/> |<span data-ttu-id="300db-119">Указывает первый день недели.</span><span class="sxs-lookup"><span data-stu-id="300db-119">Specifies the first day of the week.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="300db-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="300db-120">Parent elements</span></span>

|<span data-ttu-id="300db-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="300db-121">**Element**</span></span>|<span data-ttu-id="300db-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="300db-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="300db-123">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="300db-123">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="300db-124">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="300db-124">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="300db-125">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="300db-125">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="300db-126">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="300db-126">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="300db-127">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="300db-127">Text value</span></span>

<span data-ttu-id="300db-128">Нет.</span><span class="sxs-lookup"><span data-stu-id="300db-128">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="300db-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="300db-129">Remarks</span></span>

<span data-ttu-id="300db-130">Сведения о смещении часового пояса теряются, если даты [начала](start.md) и [окончания](end-ex15websvcsotherref.md) повторяющегося элемента шаблона не имеют даты, равной первому появлению еженедельного расписания повторения.</span><span class="sxs-lookup"><span data-stu-id="300db-130">The time zone offset information is lost if the [Start](start.md) and [End ](end-ex15websvcsotherref.md) dates of the recurring master item do not have a date that is equal to the first occurrence of a weekly recurrence pattern.</span></span> 
  
<span data-ttu-id="300db-131">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="300db-131">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="300db-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="300db-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="300db-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="300db-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="300db-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="300db-134">Schema Name</span></span>  <br/> |<span data-ttu-id="300db-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="300db-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="300db-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="300db-136">Validation File</span></span>  <br/> |<span data-ttu-id="300db-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="300db-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="300db-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="300db-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="300db-139">False</span><span class="sxs-lookup"><span data-stu-id="300db-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="300db-140">См. также</span><span class="sxs-lookup"><span data-stu-id="300db-140">See also</span></span>



- [<span data-ttu-id="300db-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="300db-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

