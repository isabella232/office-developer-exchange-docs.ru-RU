---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: Элемент AbsoluteYearlyRecurrence представляет ежегодного шаблона повторения.
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762468"
---
# <a name="absoluteyearlyrecurrence"></a><span data-ttu-id="4b4b3-103">AbsoluteYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="4b4b3-103">AbsoluteYearlyRecurrence</span></span>

<span data-ttu-id="4b4b3-104">Элемент **AbsoluteYearlyRecurrence** представляет ежегодного шаблона повторения.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-104">The **AbsoluteYearlyRecurrence** element represents a yearly recurrence pattern.</span></span> 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 <span data-ttu-id="4b4b3-105">**AbsoluteYearlyRecurrencePatternType**</span><span class="sxs-lookup"><span data-stu-id="4b4b3-105">**AbsoluteYearlyRecurrencePatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b4b3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4b4b3-106">Attributes and elements</span></span>

<span data-ttu-id="4b4b3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b4b3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4b4b3-108">Attributes</span></span>

<span data-ttu-id="4b4b3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b4b3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4b4b3-110">Child elements</span></span>

|<span data-ttu-id="4b4b3-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b4b3-111">**Element**</span></span>|<span data-ttu-id="4b4b3-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b4b3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b4b3-113">День месяца</span><span class="sxs-lookup"><span data-stu-id="4b4b3-113">DayOfMonth</span></span>](dayofmonth.md) <br/> |<span data-ttu-id="4b4b3-114">Описывает день месяца, на котором происходит повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-114">Describes the day in a month on which a recurring item occurs.</span></span> <span data-ttu-id="4b4b3-115">Диапазон значений для этого свойства — от 1 до 31.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-115">The range of values for this property is 1 to 31.</span></span> <span data-ttu-id="4b4b3-116">Если за определенный месяц это значение больше, чем число дней в месяце, последний день месяца используется значение для этого свойства.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-116">If for a particular month this value is larger than the number of days in the month, the last day of the month is assumed for this property.</span></span>  <br/> |
|[<span data-ttu-id="4b4b3-117">Месяц (повторение элемента)</span><span class="sxs-lookup"><span data-stu-id="4b4b3-117">Month (Item Recurrence)</span></span>](month-item-recurrence.md) <br/> |<span data-ttu-id="4b4b3-118">Описывает месяц, в котором ежегодно повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-118">Describes the month in which a yearly recurring item occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4b4b3-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4b4b3-119">Parent elements</span></span>

|<span data-ttu-id="4b4b3-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4b4b3-120">**Element**</span></span>|<span data-ttu-id="4b4b3-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4b4b3-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4b4b3-122">Повторение (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4b4b3-122">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="4b4b3-123">Содержит данные о повторении для повторяющихся задач.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-123">Contains recurrence information for recurring tasks.</span></span>  <br/> |
|[<span data-ttu-id="4b4b3-124">Повторение (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="4b4b3-124">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="4b4b3-125">Содержит шаблон повторения для элементов календаря и приглашения на собрания.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-125">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4b4b3-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="4b4b3-126">Remarks</span></span>

<span data-ttu-id="4b4b3-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4b4b3-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b4b3-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4b4b3-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b4b3-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4b4b3-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b4b3-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4b4b3-130">Schema Name</span></span>  <br/> |<span data-ttu-id="4b4b3-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4b4b3-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b4b3-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4b4b3-132">Validation File</span></span>  <br/> |<span data-ttu-id="4b4b3-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b4b3-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b4b3-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4b4b3-134">Can Be Empty</span></span>  <br/> |<span data-ttu-id="4b4b3-135">False</span><span class="sxs-lookup"><span data-stu-id="4b4b3-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b4b3-136">См. также</span><span class="sxs-lookup"><span data-stu-id="4b4b3-136">See also</span></span>

- [<span data-ttu-id="4b4b3-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4b4b3-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

