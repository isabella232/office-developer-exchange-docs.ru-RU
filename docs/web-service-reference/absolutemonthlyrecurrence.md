---
title: AbsoluteMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteMonthlyRecurrence
api_type:
- schema
ms.assetid: 178fa0ae-9dfc-417f-933c-d657d31c2161
description: Элемент AbsoluteMonthlyRecurrence представляет ежемесячный шаблона повторения.
ms.openlocfilehash: f4613fa71a9164c45b60a82f675959817cd4bdd5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762473"
---
# <a name="absolutemonthlyrecurrence"></a><span data-ttu-id="49438-103">AbsoluteMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="49438-103">AbsoluteMonthlyRecurrence</span></span>

<span data-ttu-id="49438-104">Элемент **AbsoluteMonthlyRecurrence** представляет ежемесячный шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="49438-104">The **AbsoluteMonthlyRecurrence** element represents a monthly recurrence pattern.</span></span> 
  
```xml
<AbsoluteMonthlyRecurrence>
   <Interval/>
   <DayOfMonth/>
</AbsoluteMonthlyRecurrence>
```

 <span data-ttu-id="49438-105">**AbsoluteMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="49438-105">**AbsoluteMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49438-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49438-106">Attributes and elements</span></span>

<span data-ttu-id="49438-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="49438-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49438-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49438-108">Attributes</span></span>

<span data-ttu-id="49438-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="49438-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49438-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49438-110">Child elements</span></span>

|<span data-ttu-id="49438-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49438-111">**Element**</span></span>|<span data-ttu-id="49438-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49438-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49438-113">День месяца</span><span class="sxs-lookup"><span data-stu-id="49438-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="49438-114">Описывает день месяца, которая происходит повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="49438-114">Describes the day in a month that a recurring item occurs.</span></span> <span data-ttu-id="49438-115">Диапазон значений для этого свойства — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="49438-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="49438-116">Если за определенный месяц это значение больше, чем число дней в месяце, последний день месяца используется значение для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="49438-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="49438-117">Интервал</span><span class="sxs-lookup"><span data-stu-id="49438-117">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="49438-118">Задает интервал между двумя последовательными повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="49438-118">Defines the interval between two consecutive recurring items.</span></span> <span data-ttu-id="49438-119">Например если элемент **интервал** имеет значение 5, повторяющегося элемента происходит каждые 5 месяцев.</span><span class="sxs-lookup"><span data-stu-id="49438-119">For example, if the **Interval** element has a value of 5, the recurring item occurs every 5 months.</span></span> <span data-ttu-id="49438-120">Диапазон допустимых значений — от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="49438-120">The range of valid values is from 1 to 99.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49438-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49438-121">Parent elements</span></span>

|<span data-ttu-id="49438-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49438-122">**Element**</span></span>|<span data-ttu-id="49438-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49438-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49438-124">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="49438-124">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="49438-125">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="49438-125">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="49438-126">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="49438-126">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="49438-127">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="49438-127">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="49438-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="49438-128">Remarks</span></span>

<span data-ttu-id="49438-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="49438-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49438-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="49438-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49438-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="49438-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="49438-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="49438-132">Schema Name</span></span>  <br/> |<span data-ttu-id="49438-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="49438-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="49438-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="49438-134">Validation File</span></span>  <br/> |<span data-ttu-id="49438-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="49438-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="49438-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="49438-136">Can Be Empty</span></span>  <br/> |<span data-ttu-id="49438-137">False</span><span class="sxs-lookup"><span data-stu-id="49438-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49438-138">См. также</span><span class="sxs-lookup"><span data-stu-id="49438-138">See also</span></span>

- [<span data-ttu-id="49438-139">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="49438-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

