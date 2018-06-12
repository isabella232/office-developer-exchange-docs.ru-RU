---
title: RelativeMonthlyRecurrence
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
description: Элемент RelativeMonthlyRecurrence описывает относительное ежемесячный шаблона повторения.
ms.openlocfilehash: 9b695052c38e2693946837bf99f03baea093df08
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835053"
---
# <a name="relativemonthlyrecurrence"></a><span data-ttu-id="85040-103">RelativeMonthlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="85040-103">RelativeMonthlyRecurrence</span></span>

<span data-ttu-id="85040-104">Элемент **RelativeMonthlyRecurrence** описывает относительное ежемесячный шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="85040-104">The **RelativeMonthlyRecurrence** element describes a relative monthly recurrence pattern.</span></span> 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 <span data-ttu-id="85040-105">**RelativeMonthlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="85040-105">**RelativeMonthlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85040-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="85040-106">Attributes and elements</span></span>

<span data-ttu-id="85040-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="85040-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85040-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="85040-108">Attributes</span></span>

<span data-ttu-id="85040-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="85040-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85040-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="85040-110">Child elements</span></span>

|<span data-ttu-id="85040-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85040-111">**Element**</span></span>|<span data-ttu-id="85040-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85040-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85040-113">Интервал</span><span class="sxs-lookup"><span data-stu-id="85040-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="85040-114">Задает интервал между двумя последовательными ежемесячно повторяющихся шаблон элементов.</span><span class="sxs-lookup"><span data-stu-id="85040-114">Defines the interval between two consecutive monthly recurring pattern items.</span></span> <span data-ttu-id="85040-115">Диапазон значений — от 1 до 99.</span><span class="sxs-lookup"><span data-stu-id="85040-115">The range for this value is 1 to 99.</span></span>  <br/> |
|[<span data-ttu-id="85040-116">DaysOfWeek (DayOfWeekType)</span><span class="sxs-lookup"><span data-stu-id="85040-116">DaysOfWeek (DayOfWeekType)</span></span>](daysofweek-dayofweektype.md) <br/> |<span data-ttu-id="85040-117">Описывается, какие дни недели находятся в относительный ежемесячный шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="85040-117">Describes which days of the week are in the relative monthly recurrence pattern.</span></span>  <br/> |
|[<span data-ttu-id="85040-118">DayOfWeekIndex</span><span class="sxs-lookup"><span data-stu-id="85040-118">DayOfWeekIndex</span></span>](dayofweekindex.md) <br/> |<span data-ttu-id="85040-119">Описывается, какие недели используется в относительный ежемесячный шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="85040-119">Describes which week is used in a relative monthly recurrence pattern.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85040-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="85040-120">Parent elements</span></span>

|<span data-ttu-id="85040-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85040-121">**Element**</span></span>|<span data-ttu-id="85040-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85040-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85040-123">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="85040-123">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="85040-124">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="85040-124">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="85040-125">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="85040-125">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="85040-126">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="85040-126">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="85040-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="85040-127">Remarks</span></span>

<span data-ttu-id="85040-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="85040-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85040-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="85040-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85040-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="85040-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85040-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="85040-131">Schema Name</span></span>  <br/> |<span data-ttu-id="85040-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="85040-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="85040-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="85040-133">Validation File</span></span>  <br/> |<span data-ttu-id="85040-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="85040-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85040-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="85040-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="85040-136">False</span><span class="sxs-lookup"><span data-stu-id="85040-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85040-137">См. также</span><span class="sxs-lookup"><span data-stu-id="85040-137">See also</span></span>



- [<span data-ttu-id="85040-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="85040-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

