---
title: FirstDayOfWeek
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FirstDayOfWeek
api_type:
- schema
ms.assetid: d6cf1bd3-a19b-4d5f-9e25-8e337a4939e0
description: Элемент FirstDayOfWeek указывает первый день недели.
ms.openlocfilehash: 99858d17213d077ce7c51ad1c746588f2f3939a7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762602"
---
# <a name="firstdayofweek"></a><span data-ttu-id="6cd43-103">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="6cd43-103">FirstDayOfWeek</span></span>

<span data-ttu-id="6cd43-104">Элемент **FirstDayOfWeek** указывает первый день недели.</span><span class="sxs-lookup"><span data-stu-id="6cd43-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="6cd43-105">**DayOfWeekType**</span><span class="sxs-lookup"><span data-stu-id="6cd43-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cd43-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6cd43-106">Attributes and elements</span></span>

<span data-ttu-id="6cd43-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6cd43-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cd43-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6cd43-108">Attributes</span></span>

<span data-ttu-id="6cd43-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cd43-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6cd43-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6cd43-110">Child elements</span></span>

<span data-ttu-id="6cd43-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="6cd43-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6cd43-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6cd43-112">Parent elements</span></span>

|<span data-ttu-id="6cd43-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6cd43-113">**Element**</span></span>|<span data-ttu-id="6cd43-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6cd43-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cd43-115">WeeklyRecurrence</span><span class="sxs-lookup"><span data-stu-id="6cd43-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="6cd43-116">Описание еженедельно повторяющейся.</span><span class="sxs-lookup"><span data-stu-id="6cd43-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6cd43-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="6cd43-117">Text value</span></span>

<span data-ttu-id="6cd43-118">Текстовое значение элемента **FirstDayOfWeek** указывает, какой день недели используется в качестве первого дня недели.</span><span class="sxs-lookup"><span data-stu-id="6cd43-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="6cd43-119">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="6cd43-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="6cd43-120">Воскресенье</span><span class="sxs-lookup"><span data-stu-id="6cd43-120">Sunday</span></span>
    
- <span data-ttu-id="6cd43-121">Понедельник</span><span class="sxs-lookup"><span data-stu-id="6cd43-121">Monday</span></span>
    
- <span data-ttu-id="6cd43-122">Вторник</span><span class="sxs-lookup"><span data-stu-id="6cd43-122">Tuesday</span></span>
    
- <span data-ttu-id="6cd43-123">Среда</span><span class="sxs-lookup"><span data-stu-id="6cd43-123">Wednesday</span></span>
    
- <span data-ttu-id="6cd43-124">Четверг</span><span class="sxs-lookup"><span data-stu-id="6cd43-124">Thursday</span></span>
    
- <span data-ttu-id="6cd43-125">Пятница</span><span class="sxs-lookup"><span data-stu-id="6cd43-125">Friday</span></span>
    
- <span data-ttu-id="6cd43-126">Суббота</span><span class="sxs-lookup"><span data-stu-id="6cd43-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="6cd43-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="6cd43-127">Remarks</span></span>

<span data-ttu-id="6cd43-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="6cd43-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cd43-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6cd43-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cd43-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6cd43-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6cd43-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6cd43-131">Schema Name</span></span>  <br/> |<span data-ttu-id="6cd43-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="6cd43-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="6cd43-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6cd43-133">Validation File</span></span>  <br/> |<span data-ttu-id="6cd43-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6cd43-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6cd43-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6cd43-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cd43-136">False</span><span class="sxs-lookup"><span data-stu-id="6cd43-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cd43-137">См. также</span><span class="sxs-lookup"><span data-stu-id="6cd43-137">See also</span></span>



- [<span data-ttu-id="6cd43-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6cd43-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

