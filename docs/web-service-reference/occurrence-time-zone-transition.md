---
title: Вхождение (часовой пояс переходов)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: 5c1142b1-c51f-42e1-bbb2-57e00cad0fdb
description: Элемент вхождение представляет вхождения день недели, месяца, которая происходит переход часового пояса.
ms.openlocfilehash: bc5160480cc6881bb9d724aa61323f5717d1f2fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834636"
---
# <a name="occurrence-time-zone-transition"></a><span data-ttu-id="25738-103">Вхождение (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="25738-103">Occurrence (Time Zone Transition)</span></span>

<span data-ttu-id="25738-104">Элемент **вхождение** представляет вхождения день недели, месяца, которая происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25738-104">The **Occurrence** element represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> 
  
```xml
<Occurrence/>
```

<span data-ttu-id="25738-105">**int**</span><span class="sxs-lookup"><span data-stu-id="25738-105">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="25738-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="25738-106">Attributes and elements</span></span>

<span data-ttu-id="25738-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="25738-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25738-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="25738-108">Attributes</span></span>

<span data-ttu-id="25738-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="25738-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25738-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="25738-110">Child elements</span></span>

<span data-ttu-id="25738-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="25738-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25738-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="25738-112">Parent elements</span></span>

|<span data-ttu-id="25738-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="25738-113">**Element**</span></span>|<span data-ttu-id="25738-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25738-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="25738-115">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="25738-115">RecurringDayTransition</span></span>](recurringdaytransition.md) <br/> |<span data-ttu-id="25738-116">Представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="25738-116">Represents a time zone transition that occurs on the same day each year.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="25738-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="25738-117">Text value</span></span>

<span data-ttu-id="25738-118">Текстовое значение представляет собой целое число, представляющее вхождения день недели, месяца, которая происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="25738-118">The text value is an integer that represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span> <span data-ttu-id="25738-119">В следующей таблице приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="25738-119">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="25738-120">**Значение**</span><span class="sxs-lookup"><span data-stu-id="25738-120">**Value**</span></span>|<span data-ttu-id="25738-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="25738-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25738-122">1</span><span class="sxs-lookup"><span data-stu-id="25738-122">1</span></span>  <br/> |<span data-ttu-id="25738-123">Первого появления указан определенный день недели от начала месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-123">The first occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-124">2</span><span class="sxs-lookup"><span data-stu-id="25738-124">2</span></span>  <br/> |<span data-ttu-id="25738-125">Второе вхождение указан определенный день недели от начала месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-125">The second occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-126">3</span><span class="sxs-lookup"><span data-stu-id="25738-126">3</span></span>  <br/> |<span data-ttu-id="25738-127">Третий вхождения указан определенный день недели от начала месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-127">The third occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-128">4</span><span class="sxs-lookup"><span data-stu-id="25738-128">4</span></span>  <br/> |<span data-ttu-id="25738-129">Четвертая вхождения указан определенный день недели от начала месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-129">The fourth occurrence of the specified day of the week from the beginning of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-130">-1</span><span class="sxs-lookup"><span data-stu-id="25738-130">-1</span></span>  <br/> |<span data-ttu-id="25738-131">Первого появления указан определенный день недели в конце месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-131">The first occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-132">-2</span><span class="sxs-lookup"><span data-stu-id="25738-132">-2</span></span>  <br/> |<span data-ttu-id="25738-133">Второе вхождение указан определенный день недели в конце месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-133">The second occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-134">от -3</span><span class="sxs-lookup"><span data-stu-id="25738-134">-3</span></span>  <br/> |<span data-ttu-id="25738-135">Третий вхождения указан определенный день недели в конце месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-135">The third occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
|<span data-ttu-id="25738-136">-4</span><span class="sxs-lookup"><span data-stu-id="25738-136">-4</span></span>  <br/> |<span data-ttu-id="25738-137">Четвертая вхождения указан определенный день недели в конце месяца.</span><span class="sxs-lookup"><span data-stu-id="25738-137">The fourth occurrence of the specified day of the week from the end of the month.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="25738-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="25738-138">Remarks</span></span>

<span data-ttu-id="25738-139">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="25738-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25738-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="25738-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25738-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="25738-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25738-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="25738-142">Schema Name</span></span>  <br/> |<span data-ttu-id="25738-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="25738-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="25738-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="25738-144">Validation File</span></span>  <br/> |<span data-ttu-id="25738-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="25738-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25738-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="25738-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="25738-147">False</span><span class="sxs-lookup"><span data-stu-id="25738-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="25738-148">См. также</span><span class="sxs-lookup"><span data-stu-id="25738-148">See also</span></span>

- [<span data-ttu-id="25738-149">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="25738-149">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

