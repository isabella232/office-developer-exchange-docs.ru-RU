---
title: релативемонслирекурренце
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: Элемент Релативемонслирекурренце описывает относительный ежемесячный шаблон повторения.
ms.openlocfilehash: 90aa0e43684bfb09a3e13cf86ec96f680e80a714
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457510"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="887ab-103">релативемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="887ab-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="887ab-104">Элемент **релативемонслирекурренце** описывает относительный ежемесячный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="887ab-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="887ab-105">**релативемонслирекурренцепаттернтипе**</span><span class="sxs-lookup"><span data-stu-id="887ab-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="887ab-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="887ab-106">Attributes and elements</span></span>

<span data-ttu-id="887ab-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="887ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="887ab-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="887ab-108">Attributes</span></span>

<span data-ttu-id="887ab-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="887ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="887ab-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="887ab-110">Child elements</span></span>

|<span data-ttu-id="887ab-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="887ab-111">**Element**</span></span>|<span data-ttu-id="887ab-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="887ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887ab-113">Interval</span><span class="sxs-lookup"><span data-stu-id="887ab-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="887ab-114">Определяет интервал между двумя последовательными ежемесячными элементами повторяющегося шаблона.</span><span class="sxs-lookup"><span data-stu-id="887ab-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="887ab-115">Значение этого параметра — от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="887ab-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="887ab-116">DaysOfWeek (Дайофвиктипе)</span><span class="sxs-lookup"><span data-stu-id="887ab-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="887ab-117">Описывает дни недели, которые находятся в относительных ежемесячных расписаниях повторения.</span><span class="sxs-lookup"><span data-stu-id="887ab-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="887ab-118">дайофвикиндекс</span><span class="sxs-lookup"><span data-stu-id="887ab-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="887ab-119">Описывает неделю, которая используется в относительных ежемесячных расписаниях повторения.</span><span class="sxs-lookup"><span data-stu-id="887ab-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="887ab-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="887ab-120">Parent elements</span></span>

|<span data-ttu-id="887ab-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="887ab-121">**Element**</span></span>|<span data-ttu-id="887ab-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="887ab-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="887ab-123">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="887ab-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="887ab-124">Содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="887ab-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="887ab-125">Повторение (Таскрекурренцетипе)</span><span class="sxs-lookup"><span data-stu-id="887ab-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="887ab-126">Содержит сведения о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="887ab-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="887ab-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="887ab-127">Remarks</span></span>

<span data-ttu-id="887ab-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="887ab-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="887ab-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="887ab-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="887ab-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="887ab-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="887ab-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="887ab-131">Schema Name</span></span>  <br/> |<span data-ttu-id="887ab-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="887ab-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="887ab-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="887ab-133">Validation File</span></span>  <br/> |<span data-ttu-id="887ab-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="887ab-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="887ab-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="887ab-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="887ab-136">False</span><span class="sxs-lookup"><span data-stu-id="887ab-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="887ab-137">См. также</span><span class="sxs-lookup"><span data-stu-id="887ab-137">See also</span></span>



- [<span data-ttu-id="887ab-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="887ab-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

