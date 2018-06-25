---
title: RecurringDayTransition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDayTransition
api_type:
- schema
ms.assetid: 1ae28d14-c2b8-4084-9e76-e2e347a884ce
description: Элемент RecurringDayTransition представляет переход часового пояса, что происходит в тот же день каждый год.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835012"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="f1617-103">RecurringDayTransition</span><span class="sxs-lookup"><span data-stu-id="f1617-103">RecurringDayTransition</span></span>

<span data-ttu-id="f1617-104">Элемент **RecurringDayTransition** представляет переход часового пояса, что происходит в тот же день каждый год.</span><span class="sxs-lookup"><span data-stu-id="f1617-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="f1617-105">**RecurringDayTransitionType**</span><span class="sxs-lookup"><span data-stu-id="f1617-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f1617-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f1617-106">Attributes and elements</span></span>

<span data-ttu-id="f1617-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f1617-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f1617-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f1617-108">Attributes</span></span>

<span data-ttu-id="f1617-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="f1617-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f1617-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f1617-110">Child elements</span></span>

|<span data-ttu-id="f1617-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1617-111">**Element**</span></span>|<span data-ttu-id="f1617-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1617-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1617-113">Задача</span><span class="sxs-lookup"><span data-stu-id="f1617-113">To</span></span>](to.md) <br/> |<span data-ttu-id="f1617-114">Задает [период](period.md) или [TransitionsGroup](transitionsgroup.md) , который является целевым для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="f1617-115">TimeOffset</span><span class="sxs-lookup"><span data-stu-id="f1617-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="f1617-116">Представляет смещение продолжительность в формате UTC для перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="f1617-117">Месяц (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="f1617-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="f1617-118">Представляет месяц, в котором осуществляется часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="f1617-119">DayOfWeek (часовой пояс)</span><span class="sxs-lookup"><span data-stu-id="f1617-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="f1617-120">Представляет день недели, на котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="f1617-121">Вхождение (часовой пояс переходов)</span><span class="sxs-lookup"><span data-stu-id="f1617-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="f1617-122">Представляет экземпляр день недели, месяца, которая происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f1617-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f1617-123">Parent elements</span></span>

|<span data-ttu-id="f1617-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f1617-124">**Element**</span></span>|<span data-ttu-id="f1617-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f1617-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f1617-126">Переходы между</span><span class="sxs-lookup"><span data-stu-id="f1617-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="f1617-127">Представляет коллекцию переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="f1617-128">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="f1617-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="f1617-129">Представляет коллекцию переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="f1617-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f1617-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="f1617-130">Remarks</span></span>

<span data-ttu-id="f1617-131">Пример перехода часовой пояс, который может быть представлен элемент [RecurringDayTransition](recurringdaytransition.md) является переход, возникает во второй вторник февраля каждый год.</span><span class="sxs-lookup"><span data-stu-id="f1617-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="f1617-132">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f1617-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f1617-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f1617-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f1617-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f1617-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f1617-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f1617-135">Schema Name</span></span>  <br/> |<span data-ttu-id="f1617-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f1617-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="f1617-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f1617-137">Validation File</span></span>  <br/> |<span data-ttu-id="f1617-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f1617-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f1617-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f1617-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="f1617-140">False</span><span class="sxs-lookup"><span data-stu-id="f1617-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f1617-141">См. также</span><span class="sxs-lookup"><span data-stu-id="f1617-141">See also</span></span>



- [<span data-ttu-id="f1617-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="f1617-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

