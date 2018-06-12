---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: Элемент TransitionsGroups представляет массив групп перехода часового пояса.
ms.openlocfilehash: 546dd3c96187bf9f1ebf574b37b689e26e3af997
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840240"
---
# <a name="transitionsgroups"></a><span data-ttu-id="69c90-103">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="69c90-103">TransitionsGroups</span></span>

<span data-ttu-id="69c90-104">Элемент **TransitionsGroups** представляет массив групп перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="69c90-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="69c90-105">**ArrayOfTransitionsGroupsType**</span><span class="sxs-lookup"><span data-stu-id="69c90-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="69c90-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69c90-106">Attributes and elements</span></span>

<span data-ttu-id="69c90-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="69c90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69c90-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69c90-108">Attributes</span></span>

<span data-ttu-id="69c90-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="69c90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69c90-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69c90-110">Child elements</span></span>

|<span data-ttu-id="69c90-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69c90-111">**Element**</span></span>|<span data-ttu-id="69c90-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69c90-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69c90-113">TransitionsGroup</span><span class="sxs-lookup"><span data-stu-id="69c90-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="69c90-114">Представляет массив переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="69c90-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="69c90-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69c90-115">Parent elements</span></span>

|<span data-ttu-id="69c90-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69c90-116">**Element**</span></span>|<span data-ttu-id="69c90-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69c90-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69c90-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="69c90-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="69c90-119">Определяет часовой пояс для времени начала [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="69c90-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="69c90-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="69c90-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="69c90-121">Определяет часовой пояс для время окончания [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="69c90-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="69c90-122">Определение часового пояса</span><span class="sxs-lookup"><span data-stu-id="69c90-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="69c90-123">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="69c90-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="69c90-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="69c90-124">Remarks</span></span>

<span data-ttu-id="69c90-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="69c90-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="69c90-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="69c90-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="69c90-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="69c90-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="69c90-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="69c90-128">Schema Name</span></span>  <br/> |<span data-ttu-id="69c90-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="69c90-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="69c90-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="69c90-130">Validation File</span></span>  <br/> |<span data-ttu-id="69c90-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="69c90-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="69c90-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="69c90-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="69c90-133">False</span><span class="sxs-lookup"><span data-stu-id="69c90-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="69c90-134">См. также</span><span class="sxs-lookup"><span data-stu-id="69c90-134">See also</span></span>



- [<span data-ttu-id="69c90-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="69c90-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

