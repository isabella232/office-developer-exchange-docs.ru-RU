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
ms.openlocfilehash: 2acbd3afb50a92d4e4f3d7b552eecb36fe59be8b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461578"
---
# <a name="recurringdatetransition"></a><span data-ttu-id="81f8c-103">рекуррингдатетранситион</span><span class="sxs-lookup"><span data-stu-id="81f8c-103">RecurringDateTransition</span></span>

<span data-ttu-id="81f8c-104">Элемент **рекуррингдатетранситион** представляет переход часового пояса, который выполняется в определенный день каждого года.</span><span class="sxs-lookup"><span data-stu-id="81f8c-104">The **RecurringDateTransition** element represents a time zone transition that occurs on a specific date each year.</span></span> 
  
```xml
<RecurringDateTransition>
   <To/>
   <TimeOffset/>
   <Month/>
   <Day/>
</RecurringDateTransition>
```

 <span data-ttu-id="81f8c-105">**рекуррингдатетранситионтипе**</span><span class="sxs-lookup"><span data-stu-id="81f8c-105">**RecurringDateTransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81f8c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81f8c-106">Attributes and elements</span></span>

<span data-ttu-id="81f8c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="81f8c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81f8c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81f8c-108">Attributes</span></span>

<span data-ttu-id="81f8c-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="81f8c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81f8c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81f8c-110">Child elements</span></span>

|<span data-ttu-id="81f8c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81f8c-111">**Element**</span></span>|<span data-ttu-id="81f8c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81f8c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81f8c-113">To</span><span class="sxs-lookup"><span data-stu-id="81f8c-113">To</span></span>](to.md) <br/> |<span data-ttu-id="81f8c-114">Указывает [период](period.md) или [транситионсграуп](transitionsgroup.md) , который является целевым объектом перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="81f8c-115">тимеоффсет</span><span class="sxs-lookup"><span data-stu-id="81f8c-115">TimeOffset</span></span>](timeoffset.md) <br/> |<span data-ttu-id="81f8c-116">Представляет смещение длительности от времени в формате UTC для смены часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-116">Represents the duration offset from Coordinated Universal Time (UTC) for the time zone transition.</span></span>  <br/> |
|[<span data-ttu-id="81f8c-117">Month (переход часового пояса)</span><span class="sxs-lookup"><span data-stu-id="81f8c-117">Month (Time Zone Transition)</span></span>](month-time-zone-transition.md) <br/> |<span data-ttu-id="81f8c-118">Представляет месяц, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-118">Represents the month in which the time zone transition occurs.</span></span>  <br/> |
|[<span data-ttu-id="81f8c-119">Day</span><span class="sxs-lookup"><span data-stu-id="81f8c-119">Day</span></span>](day.md) <br/> |<span data-ttu-id="81f8c-120">Представляет день месяца, в который происходит переход часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-120">Represents the day of the month on which the time zone transition occurs.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81f8c-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81f8c-121">Parent elements</span></span>

|<span data-ttu-id="81f8c-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81f8c-122">**Element**</span></span>|<span data-ttu-id="81f8c-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81f8c-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81f8c-124">Выполняет</span><span class="sxs-lookup"><span data-stu-id="81f8c-124">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="81f8c-125">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-125">Represents a collection of time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="81f8c-126">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="81f8c-126">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="81f8c-127">Представляет коллекцию переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81f8c-127">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81f8c-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="81f8c-128">Remarks</span></span>

<span data-ttu-id="81f8c-129">Примером перехода по часовому поясу, который может быть представлен элементом [рекуррингдатетранситион](recurringdatetransition.md) , является переход, который выполняется 15 марта каждый год.</span><span class="sxs-lookup"><span data-stu-id="81f8c-129">An example of a time zone transition that could be represented by the [RecurringDateTransition](recurringdatetransition.md) element is a transition that occurs on March 15 each year.</span></span> 
  
<span data-ttu-id="81f8c-130">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="81f8c-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81f8c-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81f8c-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81f8c-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81f8c-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81f8c-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81f8c-133">Schema Name</span></span>  <br/> |<span data-ttu-id="81f8c-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="81f8c-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="81f8c-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81f8c-135">Validation File</span></span>  <br/> |<span data-ttu-id="81f8c-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="81f8c-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81f8c-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81f8c-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="81f8c-138">False</span><span class="sxs-lookup"><span data-stu-id="81f8c-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81f8c-139">См. также</span><span class="sxs-lookup"><span data-stu-id="81f8c-139">See also</span></span>



- [<span data-ttu-id="81f8c-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="81f8c-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

