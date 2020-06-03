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
ms.openlocfilehash: 1b4aee8e1ce2548cd6b0047623b0bcda47ad316b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530974"
---
# <a name="firstdayofweek"></a><span data-ttu-id="ad9cc-103">FirstDayOfWeek</span><span class="sxs-lookup"><span data-stu-id="ad9cc-103">FirstDayOfWeek</span></span>

<span data-ttu-id="ad9cc-104">Элемент **FirstDayOfWeek** указывает первый день недели.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-104">The **FirstDayOfWeek** element specifies the first day of the week.</span></span> 
  
```XML
<FirstDayOfWeek> Sunday | Monday | Tuesday | Wednesday | Thursday | Friday | Saturday</FirstDayOfWeek>
```

 <span data-ttu-id="ad9cc-105">**дайофвиктипе**</span><span class="sxs-lookup"><span data-stu-id="ad9cc-105">**DayOfWeekType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad9cc-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad9cc-106">Attributes and elements</span></span>

<span data-ttu-id="ad9cc-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad9cc-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad9cc-108">Attributes</span></span>

<span data-ttu-id="ad9cc-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad9cc-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad9cc-110">Child elements</span></span>

<span data-ttu-id="ad9cc-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad9cc-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad9cc-112">Parent elements</span></span>

|<span data-ttu-id="ad9cc-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad9cc-113">**Element**</span></span>|<span data-ttu-id="ad9cc-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad9cc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad9cc-115">виклирекурренце</span><span class="sxs-lookup"><span data-stu-id="ad9cc-115">WeeklyRecurrence</span></span>](weeklyrecurrence.md) <br/> |<span data-ttu-id="ad9cc-116">Описывает еженедельный шаблон повторения.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-116">Describes a weekly recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad9cc-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ad9cc-117">Text value</span></span>

<span data-ttu-id="ad9cc-118">Текстовое значение элемента **FirstDayOfWeek** указывает, какой день недели используется как первый день недели.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-118">The text value of the **FirstDayOfWeek** element indicates which day of the week is used as the first day of the week.</span></span> <span data-ttu-id="ad9cc-119">Ниже приведены возможные текстовые значения.</span><span class="sxs-lookup"><span data-stu-id="ad9cc-119">The following are the possible text values:</span></span> 
  
- <span data-ttu-id="ad9cc-120">Воскресеньям</span><span class="sxs-lookup"><span data-stu-id="ad9cc-120">Sunday</span></span>
    
- <span data-ttu-id="ad9cc-121">Понедельник</span><span class="sxs-lookup"><span data-stu-id="ad9cc-121">Monday</span></span>
    
- <span data-ttu-id="ad9cc-122">Вторник</span><span class="sxs-lookup"><span data-stu-id="ad9cc-122">Tuesday</span></span>
    
- <span data-ttu-id="ad9cc-123">Среда</span><span class="sxs-lookup"><span data-stu-id="ad9cc-123">Wednesday</span></span>
    
- <span data-ttu-id="ad9cc-124">Четверг</span><span class="sxs-lookup"><span data-stu-id="ad9cc-124">Thursday</span></span>
    
- <span data-ttu-id="ad9cc-125">Пятница</span><span class="sxs-lookup"><span data-stu-id="ad9cc-125">Friday</span></span>
    
- <span data-ttu-id="ad9cc-126">Суббота</span><span class="sxs-lookup"><span data-stu-id="ad9cc-126">Saturday</span></span>
    
## <a name="remarks"></a><span data-ttu-id="ad9cc-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="ad9cc-127">Remarks</span></span>

<span data-ttu-id="ad9cc-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ad9cc-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad9cc-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad9cc-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad9cc-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad9cc-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad9cc-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad9cc-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ad9cc-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad9cc-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad9cc-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad9cc-133">Validation File</span></span>  <br/> |<span data-ttu-id="ad9cc-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ad9cc-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad9cc-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad9cc-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad9cc-136">False</span><span class="sxs-lookup"><span data-stu-id="ad9cc-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad9cc-137">См. также</span><span class="sxs-lookup"><span data-stu-id="ad9cc-137">See also</span></span>



- [<span data-ttu-id="ad9cc-138">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ad9cc-138">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

