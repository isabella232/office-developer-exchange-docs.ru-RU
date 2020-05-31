---
title: рекуррингдатетранситион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurringDateTransition
api_type:
- schema
ms.assetid: 52fe1e05-3c50-40a1-8752-5c3c64c9f1ed
description: Элемент Рекуррингдатетранситион представляет переход часового пояса, который выполняется в определенный день каждого года.
ms.openlocfilehash: 7cd8f3452a744e0c9a98fd3698dffb9ed8721a6c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835014"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="671c0-103">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="671c0-103">RecurringDateTransition</span></span>

<span data-ttu-id="671c0-104">Элемент **рекуррингдатетранситион** представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="671c0-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="671c0-105">**рекуррингдатетранситионтипе**</span><span class="sxs-lookup"><span data-stu-id="671c0-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="671c0-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="671c0-106">Attributes and elements</span></span>

<span data-ttu-id="671c0-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="671c0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="671c0-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="671c0-108">Attributes</span></span>

<span data-ttu-id="671c0-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="671c0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="671c0-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="671c0-110">Child elements</span></span>

|<span data-ttu-id="671c0-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="671c0-111">**Element**</span></span>|<span data-ttu-id="671c0-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="671c0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="671c0-113">To</span><span class="sxs-lookup"><span data-stu-id="671c0-113">To</span></span>](to.md) <br/> |<span data-ttu-id="671c0-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="671c0-115">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="671c0-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="671c0-116">Представляет смещение длительности от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="671c0-117">Month (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="671c0-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="671c0-118">Представляет месяц, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="671c0-119">Day</span><span class="sxs-lookup"><span data-stu-id="671c0-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="671c0-120">Представляет день месяца, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="671c0-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="671c0-121">Parent elements</span></span>

|<span data-ttu-id="671c0-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="671c0-122">**Element**</span></span>|<span data-ttu-id="671c0-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="671c0-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="671c0-124">Выполняет</span><span class="sxs-lookup"><span data-stu-id="671c0-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="671c0-125">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="671c0-126">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="671c0-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="671c0-127">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="671c0-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="671c0-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="671c0-128">Remarks</span></span>

<span data-ttu-id="671c0-129">Примером перехода по часовому поясу, который может быть представлен элементом [рекуррингдатетранситион](recurringdatetransition.md) , является переход, который выполняется 15 марта каждый год.</span><span class="sxs-lookup"><span data-stu-id="671c0-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="671c0-130">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="671c0-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="671c0-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="671c0-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="671c0-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="671c0-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="671c0-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="671c0-133">Schema Name</span></span>  <br/> |<span data-ttu-id="671c0-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="671c0-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="671c0-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="671c0-135">Validation File</span></span>  <br/> |<span data-ttu-id="671c0-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="671c0-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="671c0-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="671c0-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="671c0-138">False</span><span class="sxs-lookup"><span data-stu-id="671c0-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="671c0-139">См. также</span><span class="sxs-lookup"><span data-stu-id="671c0-139">See also</span></span>



- [<span data-ttu-id="671c0-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="671c0-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

