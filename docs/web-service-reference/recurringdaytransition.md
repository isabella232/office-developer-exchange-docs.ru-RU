---
title: рекуррингдайтранситион
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
description: Элемент Рекуррингдайтранситион представляет переход часового пояса, который выполняется в один день каждого года.
ms.openlocfilehash: 913345188547ce9903809fdc1cbbbe3e20ae7f36
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835012"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="bc51b-103">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="bc51b-103">RecurringDayTransition</span></span>

<span data-ttu-id="bc51b-104">Элемент **рекуррингдайтранситион** представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="bc51b-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="bc51b-105">**рекуррингдайтранситионтипе**</span><span class="sxs-lookup"><span data-stu-id="bc51b-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc51b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc51b-106">Attributes and elements</span></span>

<span data-ttu-id="bc51b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc51b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc51b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc51b-108">Attributes</span></span>

<span data-ttu-id="bc51b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="bc51b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc51b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc51b-110">Child elements</span></span>

|<span data-ttu-id="bc51b-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc51b-111">**Element**</span></span>|<span data-ttu-id="bc51b-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc51b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc51b-113">To</span><span class="sxs-lookup"><span data-stu-id="bc51b-113">To</span></span>](to.md) <br/> |<span data-ttu-id="bc51b-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="bc51b-115">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="bc51b-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="bc51b-116">Представляет смещение длительности от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="bc51b-117">Month (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="bc51b-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="bc51b-118">Представляет месяц, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="bc51b-119">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="bc51b-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="bc51b-120">Представляет день недели, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="bc51b-121">Вхождение (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="bc51b-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="bc51b-122">Представляет число дней недели в месяце, в котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc51b-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc51b-123">Parent elements</span></span>

|<span data-ttu-id="bc51b-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc51b-124">**Element**</span></span>|<span data-ttu-id="bc51b-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc51b-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc51b-126">Выполняет</span><span class="sxs-lookup"><span data-stu-id="bc51b-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="bc51b-127">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="bc51b-128">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="bc51b-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="bc51b-129">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc51b-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc51b-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc51b-130">Remarks</span></span>

<span data-ttu-id="bc51b-131">Примером перехода по часовым поясам, которые могут быть представлены элементом [рекуррингдайтранситион](recurringdaytransition.md) , является переход, который выполняется на второй вторник февраля каждого года.</span><span class="sxs-lookup"><span data-stu-id="bc51b-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="bc51b-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc51b-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc51b-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc51b-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc51b-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc51b-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc51b-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc51b-135">Schema Name</span></span>  <br/> |<span data-ttu-id="bc51b-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bc51b-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc51b-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc51b-137">Validation File</span></span>  <br/> |<span data-ttu-id="bc51b-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="bc51b-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc51b-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc51b-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc51b-140">False</span><span class="sxs-lookup"><span data-stu-id="bc51b-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc51b-141">См. также</span><span class="sxs-lookup"><span data-stu-id="bc51b-141">See also</span></span>



- [<span data-ttu-id="bc51b-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc51b-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

