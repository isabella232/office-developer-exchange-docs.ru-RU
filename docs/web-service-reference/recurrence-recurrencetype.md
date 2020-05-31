---
title: Повторение (RecurrenceType)
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
description: Элемент периодичности содержит шаблон повторения для элементов календаря и приглашений на собрание.
ms.openlocfilehash: d9c6009e11eb5b66cdd749b8e085935060f99ab7
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353352"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="dc401-103">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="dc401-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="dc401-104">Элемент **периодичности** содержит шаблон повторения для элементов календаря и приглашений на собрание.</span><span class="sxs-lookup"><span data-stu-id="dc401-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
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

<span data-ttu-id="dc401-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="dc401-105">**RecurrenceType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="dc401-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dc401-106">Attributes and elements</span></span>

<span data-ttu-id="dc401-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="dc401-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dc401-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dc401-108">Attributes</span></span>

<span data-ttu-id="dc401-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="dc401-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dc401-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dc401-110">Child elements</span></span>

|<span data-ttu-id="dc401-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dc401-111">**Element**</span></span>|<span data-ttu-id="dc401-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dc401-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc401-113">релативэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="dc401-114">Описывает относительный ежегодный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="dc401-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dc401-115">абсолутэйеарлирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="dc401-116">Представляет шаблон ежегодного повторения.</span><span class="sxs-lookup"><span data-stu-id="dc401-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dc401-117">релативемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="dc401-118">Описывает относительный месячный шаблон повторения для повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="dc401-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="dc401-119">абсолутемонслирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="dc401-120">Представляет ежемесячный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="dc401-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="dc401-121">виклирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="dc401-122">Описывает частоту в неделях и дни, в которые повторяется элемент или задача календаря.</span><span class="sxs-lookup"><span data-stu-id="dc401-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="dc401-123">даилирекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="dc401-124">Описывает частоту повторения элемента календаря или задачи в днях.</span><span class="sxs-lookup"><span data-stu-id="dc401-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="dc401-125">ноендрекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="dc401-126">Описывает шаблон повторения, для которого не определена конечная дата.</span><span class="sxs-lookup"><span data-stu-id="dc401-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="dc401-127">Использование этого элемента исключает использование элементов [енддатерекурренце](enddaterecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dc401-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="dc401-128">енддатерекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="dc401-129">Описывает дату начала и дату окончания расписания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="dc401-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="dc401-130">Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [нумбередрекурренце](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dc401-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="dc401-131">нумбередрекурренце</span><span class="sxs-lookup"><span data-stu-id="dc401-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="dc401-132">Описывает дату начала и число повторений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="dc401-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="dc401-133">Использование этого элемента исключает использование элементов [ноендрекурренце](noendrecurrence.md) и [енддатерекурренце](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="dc401-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="dc401-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dc401-134">Parent elements</span></span>

|<span data-ttu-id="dc401-135">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dc401-135">**Element**</span></span>|<span data-ttu-id="dc401-136">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dc401-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dc401-137">календаритем</span><span class="sxs-lookup"><span data-stu-id="dc401-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="dc401-138">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="dc401-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="dc401-139">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="dc401-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="dc401-140">Представляет приглашение на собрание в хранилище Exchange</span><span class="sxs-lookup"><span data-stu-id="dc401-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dc401-141">Примечания</span><span class="sxs-lookup"><span data-stu-id="dc401-141">Remarks</span></span>

<span data-ttu-id="dc401-142">Этот элемент является допустимым, если [календаритемтипе](calendaritemtype.md) имеет значение рекуррингмастер.</span><span class="sxs-lookup"><span data-stu-id="dc401-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="dc401-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dc401-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dc401-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="dc401-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dc401-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="dc401-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dc401-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="dc401-146">Schema name</span></span>  <br/> |<span data-ttu-id="dc401-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="dc401-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="dc401-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="dc401-148">Validation file</span></span>  <br/> |<span data-ttu-id="dc401-149">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="dc401-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dc401-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="dc401-150">Can be empty</span></span>  <br/> |<span data-ttu-id="dc401-151">False</span><span class="sxs-lookup"><span data-stu-id="dc401-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc401-152">См. также</span><span class="sxs-lookup"><span data-stu-id="dc401-152">See also</span></span>

- [<span data-ttu-id="dc401-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="dc401-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

