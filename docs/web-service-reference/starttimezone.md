---
title: StartTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeZone
api_type:
- schema
ms.assetid: d38c4dc1-4ecb-42a1-8d57-a451b16a2de2
description: Элемент StartTimeZone определяет часовой пояс для времени начала элемента календаря, имеющего или MeetingRequest.
ms.openlocfilehash: 6d21869c4b3be048db27dcc9f128fff868aebcb5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835559"
---
# <a name="starttimezone"></a><span data-ttu-id="e708d-103">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="e708d-103">StartTimeZone</span></span>

<span data-ttu-id="e708d-104">Элемент **StartTimeZone** определяет часовой пояс для времени начала [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e708d-104">The **StartTimeZone** element defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>
  
```xml
<StartTimeZone Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</StartTimeZone>
```

<span data-ttu-id="e708d-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="e708d-105">**TimeZoneDefinitionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e708d-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e708d-106">Attributes and elements</span></span>

<span data-ttu-id="e708d-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e708d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e708d-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e708d-108">Attributes</span></span>

|<span data-ttu-id="e708d-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e708d-109">**Attribute**</span></span>|<span data-ttu-id="e708d-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e708d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e708d-111">Id</span><span class="sxs-lookup"><span data-stu-id="e708d-111">Id</span></span>  <br/> |<span data-ttu-id="e708d-112">Представляет уникальный идентификатор определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e708d-112">Represents the unique identifier of the time zone definition.</span></span>  <br/> |
|<span data-ttu-id="e708d-113">Имя</span><span class="sxs-lookup"><span data-stu-id="e708d-113">Name</span></span>  <br/> |<span data-ttu-id="e708d-114">Представляет описательное имя определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e708d-114">Represents the descriptive name of the time zone definition.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e708d-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e708d-115">Child elements</span></span>

|<span data-ttu-id="e708d-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e708d-116">**Element**</span></span>|<span data-ttu-id="e708d-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e708d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e708d-118">Периоды</span><span class="sxs-lookup"><span data-stu-id="e708d-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="e708d-119">Представляет массив элементов [периода времени](period.md) , которые определяют смещение времени на различных этапах часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e708d-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="e708d-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="e708d-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="e708d-121">Представляет массив [TransitionsGroup](transitionsgroup.md) элементов, которые задают переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e708d-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e708d-122">Переходы между</span><span class="sxs-lookup"><span data-stu-id="e708d-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e708d-123">Представляет массив переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e708d-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e708d-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e708d-124">Parent elements</span></span>

|<span data-ttu-id="e708d-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e708d-125">**Element**</span></span>|<span data-ttu-id="e708d-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e708d-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e708d-127">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="e708d-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="e708d-128">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="e708d-128">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="e708d-129">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="e708d-129">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="e708d-130">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="e708d-130">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e708d-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="e708d-131">Remarks</span></span>

<span data-ttu-id="e708d-132">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e708d-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e708d-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e708d-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e708d-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e708d-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e708d-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e708d-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e708d-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e708d-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e708d-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e708d-137">Validation File</span></span>  <br/> |<span data-ttu-id="e708d-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e708d-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e708d-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e708d-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e708d-140">False</span><span class="sxs-lookup"><span data-stu-id="e708d-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e708d-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e708d-141">See also</span></span>

- [<span data-ttu-id="e708d-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e708d-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

