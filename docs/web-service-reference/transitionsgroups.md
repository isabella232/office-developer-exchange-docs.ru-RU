---
title: транситионсграупс
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
description: Элемент Транситионсграупс представляет массив групп смены часовых поясов.
ms.openlocfilehash: 546dd3c96187bf9f1ebf574b37b689e26e3af997
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840240"
---
# <a name="transitionsgroups"></a><span data-ttu-id="521ab-103">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="521ab-103">TransitionsGroups</span></span>

<span data-ttu-id="521ab-104">Элемент **транситионсграупс** представляет массив групп смены часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="521ab-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="521ab-105">**аррайофтранситионсграупстипе**</span><span class="sxs-lookup"><span data-stu-id="521ab-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="521ab-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="521ab-106">Attributes and elements</span></span>

<span data-ttu-id="521ab-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="521ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="521ab-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="521ab-108">Attributes</span></span>

<span data-ttu-id="521ab-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="521ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="521ab-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="521ab-110">Child elements</span></span>

|<span data-ttu-id="521ab-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="521ab-111">**Element**</span></span>|<span data-ttu-id="521ab-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="521ab-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="521ab-113">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="521ab-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="521ab-114">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="521ab-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="521ab-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="521ab-115">Parent elements</span></span>

|<span data-ttu-id="521ab-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="521ab-116">**Element**</span></span>|<span data-ttu-id="521ab-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="521ab-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="521ab-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="521ab-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="521ab-119">Определяет часовой пояс времени начала [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="521ab-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="521ab-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="521ab-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="521ab-121">Определяет часовой пояс для времени окончания [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="521ab-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="521ab-122">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="521ab-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="521ab-123">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="521ab-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="521ab-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="521ab-124">Remarks</span></span>

<span data-ttu-id="521ab-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="521ab-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="521ab-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="521ab-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="521ab-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="521ab-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="521ab-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="521ab-128">Schema Name</span></span>  <br/> |<span data-ttu-id="521ab-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="521ab-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="521ab-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="521ab-130">Validation File</span></span>  <br/> |<span data-ttu-id="521ab-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="521ab-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="521ab-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="521ab-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="521ab-133">False</span><span class="sxs-lookup"><span data-stu-id="521ab-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="521ab-134">См. также</span><span class="sxs-lookup"><span data-stu-id="521ab-134">See also</span></span>



- [<span data-ttu-id="521ab-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="521ab-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

