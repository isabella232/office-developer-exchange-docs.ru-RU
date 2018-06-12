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
description: Элемент повторения содержит шаблон повторения для элементов календаря и приглашения на собрания.
ms.openlocfilehash: f26ccf5912848a6d7fbbfa7d0a19d41635c896e0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835004"
---
# <a name="recurrence-recurrencetype"></a><span data-ttu-id="8daa1-103">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="8daa1-103">Recurrence (RecurrenceType)</span></span>

<span data-ttu-id="8daa1-104">Элемент **повторения** содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="8daa1-104">The **Recurrence** element contains the recurrence pattern for calendar items and meeting requests.</span></span> 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 <span data-ttu-id="8daa1-105">**RecurrenceType**</span><span class="sxs-lookup"><span data-stu-id="8daa1-105">**RecurrenceType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8daa1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8daa1-106">Attributes and elements</span></span>

<span data-ttu-id="8daa1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8daa1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8daa1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8daa1-108">Attributes</span></span>

<span data-ttu-id="8daa1-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="8daa1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8daa1-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8daa1-110">Child elements</span></span>

|<span data-ttu-id="8daa1-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8daa1-111">**Element**</span></span>|<span data-ttu-id="8daa1-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8daa1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8daa1-113">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-113">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="8daa1-114">Описывает относительное ежегодно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="8daa1-114">Describes a relative yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-115">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-115">AbsoluteYearlyRecurrence</span></span>](absoluteyearlyrecurrence.md) <br/> |<span data-ttu-id="8daa1-116">Представляет шаблон повторения ежегодно.</span><span class="sxs-lookup"><span data-stu-id="8daa1-116">Represents a yearly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-117">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-117">RelativeMonthlyRecurrence</span></span>](relativemonthlyrecurrence.md) <br/> |<span data-ttu-id="8daa1-118">Описывает относительное ежемесячный шаблона повторения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="8daa1-118">Describes a relative monthly recurrence pattern for a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-119">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-119">AbsoluteMonthlyRecurrence</span></span>](absolutemonthlyrecurrence.md) <br/> |<span data-ttu-id="8daa1-120">Представляет шаблон повторения ежемесячно.</span><span class="sxs-lookup"><span data-stu-id="8daa1-120">Represents a monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-121">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-121">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="8daa1-122">Описание частоты недели и дней, элемента календаря или задача повторяется.</span><span class="sxs-lookup"><span data-stu-id="8daa1-122">Describes the frequency, in weeks, and the days that a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-123">DailyRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-123">DailyRecurrence</span></span>](dailyrecurrence.md) <br/> |<span data-ttu-id="8daa1-124">Описывает период в днях, в котором повторяется элемента календаря или задач.</span><span class="sxs-lookup"><span data-stu-id="8daa1-124">Describes the frequency, in days, in which a calendar item or task recurs.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-125">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-125">NoEndRecurrence</span></span>](noendrecurrence.md) <br/> |<span data-ttu-id="8daa1-126">Описание шаблона повторения, который не имеет определенный срок.</span><span class="sxs-lookup"><span data-stu-id="8daa1-126">Describes a recurrence pattern that does not have a defined end date.</span></span>  <br/> <span data-ttu-id="8daa1-127">Использование этого элемента исключает использование элементов [EndDateRecurrence](enddaterecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="8daa1-127">The use of this element excludes the use of the [EndDateRecurrence](enddaterecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-128">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-128">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="8daa1-129">Описание, Дата начала и Дата окончания повторения элемента.</span><span class="sxs-lookup"><span data-stu-id="8daa1-129">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> <span data-ttu-id="8daa1-130">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [NumberedRecurrence](numberedrecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="8daa1-130">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [NumberedRecurrence](numberedrecurrence.md) elements.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-131">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="8daa1-131">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="8daa1-132">Описание, Дата начала и число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="8daa1-132">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> <span data-ttu-id="8daa1-133">Использование этого элемента исключает использование элементов [NoEndRecurrence](noendrecurrence.md) и [EndDateRecurrence](enddaterecurrence.md) .</span><span class="sxs-lookup"><span data-stu-id="8daa1-133">The use of this element excludes the use of the [NoEndRecurrence](noendrecurrence.md) and [EndDateRecurrence](enddaterecurrence.md) elements.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8daa1-134">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8daa1-134">Parent elements</span></span>

|<span data-ttu-id="8daa1-135">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8daa1-135">**Element**</span></span>|<span data-ttu-id="8daa1-136">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8daa1-136">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8daa1-137">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="8daa1-137">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="8daa1-138">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="8daa1-138">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8daa1-139">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="8daa1-139">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="8daa1-140">Представляет приглашения на собрание в хранилище Exchange</span><span class="sxs-lookup"><span data-stu-id="8daa1-140">Represents a meeting request in the Exchange store</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8daa1-141">Замечания</span><span class="sxs-lookup"><span data-stu-id="8daa1-141">Remarks</span></span>

<span data-ttu-id="8daa1-142">Этот элемент является допустимым, если [CalendarItemType](calendaritemtype.md) имеет значение RecurringMaster.</span><span class="sxs-lookup"><span data-stu-id="8daa1-142">This element is valid if [CalendarItemType](calendaritemtype.md) has the RecurringMaster value.</span></span> 
  
<span data-ttu-id="8daa1-143">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8daa1-143">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8daa1-144">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8daa1-144">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8daa1-145">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8daa1-145">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8daa1-146">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8daa1-146">Schema name</span></span>  <br/> |<span data-ttu-id="8daa1-147">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8daa1-147">Types schema</span></span>  <br/> |
|<span data-ttu-id="8daa1-148">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8daa1-148">Validation file</span></span>  <br/> |<span data-ttu-id="8daa1-149">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8daa1-149">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8daa1-150">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8daa1-150">Can be empty</span></span>  <br/> |<span data-ttu-id="8daa1-151">False</span><span class="sxs-lookup"><span data-stu-id="8daa1-151">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8daa1-152">См. также</span><span class="sxs-lookup"><span data-stu-id="8daa1-152">See also</span></span>



- [<span data-ttu-id="8daa1-153">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8daa1-153">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

