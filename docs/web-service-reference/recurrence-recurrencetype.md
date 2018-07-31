---
title: Recurrence (RecurrenceType)
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
ms.assetid: 3d1c2c1c-4103-47ce-ad3c-ad16ec6e9b12
description: Элемент повторения содержит шаблон повторения для элементов календаря и приглашения на собрания.
ms.openlocfilehash: d9c6009e11eb5b66cdd749b8e085935060f99ab7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353352"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="a53ce-103">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="a53ce-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="a53ce-104">Элемент **повторения** содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="a53ce-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeYearlyRecurrence/> 
      <NumberedRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <DailyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <EndDateRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteMonthlyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <NoEndRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NoEndRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <WeeklyRecurrence/> 
      <NumberedRecurrence/> 
</Recurrence>
```

```xml
<Recurrence>
      <AbsoluteYearlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

```xml
<Recurrence>
      <RelativeMonthlyRecurrence/> 
      <EndDateRecurrence/>
</Recurrence>
```

<span data-ttu-id="a53ce-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="a53ce-105">**RecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a53ce-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a53ce-106">Attributes and elements</span></span>

<span data-ttu-id="a53ce-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a53ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a53ce-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a53ce-108">Attributes</span></span>

<span data-ttu-id="a53ce-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a53ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a53ce-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a53ce-110">Child elements</span></span>

|<span data-ttu-id="a53ce-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a53ce-111">**Element**</span></span>|<span data-ttu-id="a53ce-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a53ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a53ce-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="a53ce-114">Описывает относительное ежегодно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="a53ce-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="a53ce-116">Представляет шаблон повторения ежегодно.</span><span class="sxs-lookup"><span data-stu-id="a53ce-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="a53ce-118">Описывает относительное ежемесячный шаблона повторения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="a53ce-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="a53ce-120">Представляет шаблон повторения ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="a53ce-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="a53ce-122">Описание частоты недели и дней, элемента календаря или задача повторяется.</span><span class="sxs-lookup"><span data-stu-id="a53ce-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="a53ce-124">Описывает период в днях, в котором повторяется элемента календаря или задач.</span><span class="sxs-lookup"><span data-stu-id="a53ce-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="a53ce-126">Описание шаблона повторения, который не имеет определенный срок.</span><span class="sxs-lookup"><span data-stu-id="a53ce-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="a53ce-127">Использование этого элемента исключает использование элементов [EndDateRecurrence](enddaterecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a53ce-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="a53ce-129">Описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="a53ce-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="a53ce-130">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a53ce-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="a53ce-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="a53ce-132">Описание, Дата начала и число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="a53ce-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="a53ce-133">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="a53ce-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a53ce-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a53ce-134">Parent elements</span></span>

|<span data-ttu-id="a53ce-135">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a53ce-135">**Element**</span></span>|<span data-ttu-id="a53ce-136">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a53ce-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a53ce-137">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="a53ce-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="a53ce-138">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="a53ce-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a53ce-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="a53ce-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="a53ce-140">Представляет приглашения на собрание в хранилище Exchange</span><span class="sxs-lookup"><span data-stu-id="a53ce-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a53ce-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="a53ce-141">Remarks</span></span>

<span data-ttu-id="a53ce-142">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="a53ce-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="a53ce-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a53ce-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a53ce-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a53ce-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a53ce-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a53ce-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a53ce-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a53ce-146">Schema name</span></span>  <br/> |<span data-ttu-id="a53ce-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a53ce-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="a53ce-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a53ce-148">Validation file</span></span>  <br/> |<span data-ttu-id="a53ce-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a53ce-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a53ce-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a53ce-150">Can be empty</span></span>  <br/> |<span data-ttu-id="a53ce-151">False</span><span class="sxs-lookup"><span data-stu-id="a53ce-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a53ce-152">См. также</span><span class="sxs-lookup"><span data-stu-id="a53ce-152">See also</span></span>

- [<span data-ttu-id="a53ce-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a53ce-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

