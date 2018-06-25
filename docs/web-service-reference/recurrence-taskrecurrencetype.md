---
title: Повторение (TaskRecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: Элемент повторения содержит данные о повторении для повторяющихся задач.
ms.openlocfilehash: ae2bb35e89a0a50c7ca67cb0e580427150afb99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835006"
---
# <a name="recurrence-taskrecurrencetype"></a><span data-ttu-id="62ef6-103">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="62ef6-103">Recurrence (TaskRecurrenceType)</span></span>

<span data-ttu-id="62ef6-104">Элемент **повторения** содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="62ef6-104">The **Recurrence** element contains recurrence information for recurring tasks.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="62ef6-105">**TaskRecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="62ef6-105">**TaskRecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62ef6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="62ef6-106">Attributes and elements</span></span>

<span data-ttu-id="62ef6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="62ef6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62ef6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="62ef6-108">Attributes</span></span>

<span data-ttu-id="62ef6-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="62ef6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="62ef6-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="62ef6-110">Child elements</span></span>

|<span data-ttu-id="62ef6-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62ef6-111">**Element**</span></span>|<span data-ttu-id="62ef6-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62ef6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62ef6-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="62ef6-114">Описывает относительное ежегодный шаблон повторения для повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-114">Describes a relative yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="62ef6-116">Представляет шаблон повторения ежегодно повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-116">Represents a yearly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="62ef6-118">Описывает относительное ежемесячный шаблон повторения для повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-118">Describes a relative monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="62ef6-120">Представляет шаблон повторения ежемесячно для повторяющейся задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-120">Represents a monthly recurrence pattern for a recurring task.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="62ef6-122">Описание частоты в недели и дней, на которых повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-122">Describes the frequency, in weeks, and the days on which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="62ef6-124">Описывает период в днях, в которых повторения задачи.</span><span class="sxs-lookup"><span data-stu-id="62ef6-124">Describes the frequency, in days, in which a task recurs.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-125">DailyRegeneration</span><span class="sxs-lookup"><span data-stu-id="62ef6-125">DailyRegeneration</span></span>](dailyregeneration.md) <br/> |<span data-ttu-id="62ef6-126">Описывает через сколько дней после завершения текущей задачи следующее вхождение должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="62ef6-126">Describes how many days after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-127">WeeklyRegeneration</span><span class="sxs-lookup"><span data-stu-id="62ef6-127">WeeklyRegeneration</span></span>](weeklyregeneration.md) <br/> |<span data-ttu-id="62ef6-128">Описывает сколько недель после завершения текущей задачи следующее вхождение должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="62ef6-128">Describes how many weeks after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-129">MonthlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="62ef6-129">MonthlyRegeneration</span></span>](monthlyregeneration.md) <br/> |<span data-ttu-id="62ef6-130">Описывает число месяцев после завершения текущей задачи следующее вхождение должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="62ef6-130">Describes how many months after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-131">YearlyRegeneration</span><span class="sxs-lookup"><span data-stu-id="62ef6-131">YearlyRegeneration</span></span>](yearlyregeneration.md) <br/> |<span data-ttu-id="62ef6-132">Описывает сколько лет после завершения текущей задачи следующее вхождение должны быть выполнены.</span><span class="sxs-lookup"><span data-stu-id="62ef6-132">Describes how many years after the completion of the current task the next occurrence will be due.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-133">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-133">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="62ef6-134">Описание шаблона повторения, который не имеет определенный срок.</span><span class="sxs-lookup"><span data-stu-id="62ef6-134">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="62ef6-135">Использование этого элемента исключает использование элементов [EndDateRecurrence](enddaterecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="62ef6-135">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-136">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-136">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="62ef6-137">Описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="62ef6-137">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="62ef6-138">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="62ef6-138">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> <span data-ttu-id="62ef6-139">[EndDateRecurrence](enddaterecurrence.md) не может использоваться вместе с повторного создания шаблона.</span><span class="sxs-lookup"><span data-stu-id="62ef6-139">[EndDateRecurrence](enddaterecurrence.md) cannot be used together with a regeneration pattern.</span></span>  <br/> |
|[<span data-ttu-id="62ef6-140">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="62ef6-140">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="62ef6-141">Описание, Дата начала и число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="62ef6-141">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="62ef6-142">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="62ef6-142">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62ef6-143">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="62ef6-143">Parent elements</span></span>

|<span data-ttu-id="62ef6-144">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="62ef6-144">**Element**</span></span>|<span data-ttu-id="62ef6-145">**Описание**</span><span class="sxs-lookup"><span data-stu-id="62ef6-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62ef6-146">Задача</span><span class="sxs-lookup"><span data-stu-id="62ef6-146">Task</span></span>](task.md) <br/> |<span data-ttu-id="62ef6-147">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="62ef6-147">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="62ef6-148">Замечания</span><span class="sxs-lookup"><span data-stu-id="62ef6-148">Remarks</span></span>

<span data-ttu-id="62ef6-149">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="62ef6-149">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62ef6-150">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="62ef6-150">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62ef6-151">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="62ef6-151">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="62ef6-152">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="62ef6-152">Schema name</span></span>  <br/> |<span data-ttu-id="62ef6-153">Схема Types</span><span class="sxs-lookup"><span data-stu-id="62ef6-153">Types schema</span></span>  <br/> |
|<span data-ttu-id="62ef6-154">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="62ef6-154">Validation file</span></span>  <br/> |<span data-ttu-id="62ef6-155">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="62ef6-155">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="62ef6-156">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="62ef6-156">Can be empty</span></span>  <br/> |<span data-ttu-id="62ef6-157">False</span><span class="sxs-lookup"><span data-stu-id="62ef6-157">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62ef6-158">См. также</span><span class="sxs-lookup"><span data-stu-id="62ef6-158">See also</span></span>



- [<span data-ttu-id="62ef6-159">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="62ef6-159">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

