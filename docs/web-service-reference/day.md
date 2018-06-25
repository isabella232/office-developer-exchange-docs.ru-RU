---
title: День
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Day
api_type:
- schema
ms.assetid: d3b2dc66-486a-41d1-bff3-606f0bf92715
description: Элемент Day представляет день месяца, на котором происходит переход часового пояса.
ms.openlocfilehash: 01d1bf7833a89c0bb9a2b1af95ec8dfc627336d9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761988"
---
# <a name="day"></a><span data-ttu-id="07cf3-103">День</span><span class="sxs-lookup"><span data-stu-id="07cf3-103">Day</span></span>

<span data-ttu-id="07cf3-104">Элемент **Day** представляет день месяца, на котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="07cf3-104">The **Day** element represents the day of the month on which the time zone transition occurs.</span></span> 
  
```xml
<Day/>
```

<span data-ttu-id="07cf3-105">**int**</span><span class="sxs-lookup"><span data-stu-id="07cf3-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="07cf3-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07cf3-106">Attributes and elements</span></span>

<span data-ttu-id="07cf3-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="07cf3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07cf3-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07cf3-108">Attributes</span></span>

<span data-ttu-id="07cf3-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="07cf3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07cf3-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07cf3-110">Child elements</span></span>

<span data-ttu-id="07cf3-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="07cf3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="07cf3-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07cf3-112">Parent elements</span></span>

|<span data-ttu-id="07cf3-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07cf3-113">**Element**</span></span>|<span data-ttu-id="07cf3-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07cf3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07cf3-115">RecurringDateTransition</span><span class="sxs-lookup"><span data-stu-id="07cf3-115">RecurringDateTransition</span></span>](recurringdatetransition.md) <br/> |<span data-ttu-id="07cf3-116">Представляет переход часового пояса, что происходит в конкретный день каждый год.</span><span class="sxs-lookup"><span data-stu-id="07cf3-116">Represents a time zone transition that occurs on a specific date each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="07cf3-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="07cf3-117">Text value</span></span>

<span data-ttu-id="07cf3-118">Текстовое значение элемента **день** — целое число, представляющее день месяца, на котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="07cf3-118">The text value of the **Day** element is an integer that represents the day of the month on which the time zone transition occurs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="07cf3-119">Замечания</span><span class="sxs-lookup"><span data-stu-id="07cf3-119">Remarks</span></span>

<span data-ttu-id="07cf3-120">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="07cf3-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="07cf3-121">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="07cf3-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="07cf3-122">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="07cf3-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="07cf3-123">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="07cf3-123">Schema Name</span></span>  <br/> |<span data-ttu-id="07cf3-124">Схема Types</span><span class="sxs-lookup"><span data-stu-id="07cf3-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="07cf3-125">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="07cf3-125">Validation File</span></span>  <br/> |<span data-ttu-id="07cf3-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="07cf3-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="07cf3-127">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="07cf3-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="07cf3-128">False</span><span class="sxs-lookup"><span data-stu-id="07cf3-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="07cf3-129">См. также</span><span class="sxs-lookup"><span data-stu-id="07cf3-129">See also</span></span>

- [<span data-ttu-id="07cf3-130">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="07cf3-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

