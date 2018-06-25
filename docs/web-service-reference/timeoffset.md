---
title: TimeOffset
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeOffset
api_type:
- schema
ms.assetid: b70bf498-cc3a-4fa6-8236-514acb973b33
description: Элемент TimeOffset представляет смещение времени в формате UTC для перехода часового пояса.
ms.openlocfilehash: 46b1b2c8eec9bae871b4dafe43036e9d725075ae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840165"
---
# <a name="timeoffset"></a><span data-ttu-id="565db-103">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="565db-103">TimeOffset</span></span>

<span data-ttu-id="565db-104">Элемент **TimeOffset** представляет смещение времени в формате UTC для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="565db-104">The **TimeOffset** element represents the time offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span> 
  
```XML
<TimeOffset/>
```

 <span data-ttu-id="565db-105">**duration**</span><span class="sxs-lookup"><span data-stu-id="565db-105">**duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="565db-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="565db-106">Attributes and elements</span></span>

<span data-ttu-id="565db-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="565db-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="565db-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="565db-108">Attributes</span></span>

<span data-ttu-id="565db-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="565db-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="565db-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="565db-110">Child elements</span></span>

<span data-ttu-id="565db-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="565db-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="565db-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="565db-112">Parent elements</span></span>

|<span data-ttu-id="565db-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="565db-113">**Element**</span></span>|<span data-ttu-id="565db-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="565db-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="565db-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="565db-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="565db-116">Представляет переход часового пояса, что происходит в конкретный день каждый год.</span><span class="sxs-lookup"><span data-stu-id="565db-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
|[<span data-ttu-id="565db-117">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="565db-117">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="565db-118">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="565db-118">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="565db-119">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="565db-119">Text value</span></span>

<span data-ttu-id="565db-120">Текстовое значение элемента **TimeOffset** является длительность, указывающее смещение времени в формате UTC для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="565db-120">The text value of the **TimeOffset** element is a duration that specifies the time offset from UTC for the time zone transition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="565db-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="565db-121">Remarks</span></span>

<span data-ttu-id="565db-122">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="565db-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="565db-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="565db-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="565db-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="565db-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="565db-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="565db-125">Schema Name</span></span>  <br/> |<span data-ttu-id="565db-126">Схема Types</span><span class="sxs-lookup"><span data-stu-id="565db-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="565db-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="565db-127">Validation File</span></span>  <br/> |<span data-ttu-id="565db-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="565db-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="565db-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="565db-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="565db-130">False</span><span class="sxs-lookup"><span data-stu-id="565db-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="565db-131">См. также</span><span class="sxs-lookup"><span data-stu-id="565db-131">See also</span></span>



- [<span data-ttu-id="565db-132">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="565db-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

