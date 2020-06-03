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
ms.openlocfilehash: 44c2a6ec4dbaaa52a2772cb5c35a84b14dd77f97
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468469"
---
# <a name="recurringdaytransition"></a><span data-ttu-id="4be6f-103">рекуррингдайтранситион</span><span class="sxs-lookup"><span data-stu-id="4be6f-103">RecurringDayTransition</span></span>

<span data-ttu-id="4be6f-104">Элемент **рекуррингдайтранситион** представляет переход часового пояса, который выполняется в один день каждого года.</span><span class="sxs-lookup"><span data-stu-id="4be6f-104">The **RecurringDayTransition** element represents a time zone transition that occurs on the same day each year.</span></span> 
  
```xml
<RecurringDayTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <DayOfWeek/>
   <Occurrence/>
</RecurringDayTransition>
```

 <span data-ttu-id="4be6f-105">**рекуррингдайтранситионтипе**</span><span class="sxs-lookup"><span data-stu-id="4be6f-105">**RecurringDayTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4be6f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4be6f-106">Attributes and elements</span></span>

<span data-ttu-id="4be6f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4be6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4be6f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4be6f-108">Attributes</span></span>

<span data-ttu-id="4be6f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4be6f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4be6f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4be6f-110">Child elements</span></span>

|<span data-ttu-id="4be6f-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4be6f-111">**Element**</span></span>|<span data-ttu-id="4be6f-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4be6f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4be6f-113">To</span><span class="sxs-lookup"><span data-stu-id="4be6f-113">To</span></span>](to.md) <br/> |<span data-ttu-id="4be6f-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="4be6f-115">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="4be6f-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="4be6f-116">Представляет смещение длительности от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="4be6f-117">Month (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="4be6f-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="4be6f-118">Представляет месяц, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="4be6f-119">DayOfWeek (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="4be6f-119">DayOfWeek (TimeZone)</span></span>](dayofweek-timezone.md) <br/> |<span data-ttu-id="4be6f-120">Представляет день недели, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-120">Represents the day of the week on which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="4be6f-121">Вхождение (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="4be6f-121">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="4be6f-122">Представляет число дней недели в месяце, в котором происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-122">Represents the occurrence of the day of the week in the month that the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4be6f-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4be6f-123">Parent elements</span></span>

|<span data-ttu-id="4be6f-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4be6f-124">**Element**</span></span>|<span data-ttu-id="4be6f-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4be6f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4be6f-126">Выполняет</span><span class="sxs-lookup"><span data-stu-id="4be6f-126">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="4be6f-127">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-127">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="4be6f-128">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="4be6f-128">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="4be6f-129">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="4be6f-129">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4be6f-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="4be6f-130">Remarks</span></span>

<span data-ttu-id="4be6f-131">Примером перехода по часовым поясам, которые могут быть представлены элементом [рекуррингдайтранситион](recurringdaytransition.md) , является переход, который выполняется на второй вторник февраля каждого года.</span><span class="sxs-lookup"><span data-stu-id="4be6f-131">An example of a time zone transition that could be represented by the [RecurringDayTransition](recurringdaytransition.md) element is a transition that occurs on the second Tuesday of February each year.</span></span> 
  
<span data-ttu-id="4be6f-132">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4be6f-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4be6f-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4be6f-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4be6f-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4be6f-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4be6f-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4be6f-135">Schema Name</span></span>  <br/> |<span data-ttu-id="4be6f-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4be6f-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="4be6f-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4be6f-137">Validation File</span></span>  <br/> |<span data-ttu-id="4be6f-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4be6f-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4be6f-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4be6f-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="4be6f-140">False</span><span class="sxs-lookup"><span data-stu-id="4be6f-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4be6f-141">См. также</span><span class="sxs-lookup"><span data-stu-id="4be6f-141">See also</span></span>



- [<span data-ttu-id="4be6f-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4be6f-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

