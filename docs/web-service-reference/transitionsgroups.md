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
ms.openlocfilehash: 35244e122ee31045359afd0833459bbb94fd0aa1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467412"
---
# <a name="transitionsgroups"></a><span data-ttu-id="e6496-103">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="e6496-103">TransitionsGroups</span></span>

<span data-ttu-id="e6496-104">Элемент **транситионсграупс** представляет массив групп смены часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="e6496-104">The **TransitionsGroups** element represents an array of time zone transition groups.</span></span> 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 <span data-ttu-id="e6496-105">**аррайофтранситионсграупстипе**</span><span class="sxs-lookup"><span data-stu-id="e6496-105">**ArrayOfTransitionsGroupsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6496-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e6496-106">Attributes and elements</span></span>

<span data-ttu-id="e6496-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e6496-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6496-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e6496-108">Attributes</span></span>

<span data-ttu-id="e6496-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e6496-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6496-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e6496-110">Child elements</span></span>

|<span data-ttu-id="e6496-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e6496-111">**Element**</span></span>|<span data-ttu-id="e6496-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e6496-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6496-113">транситионсграуп</span><span class="sxs-lookup"><span data-stu-id="e6496-113">TransitionsGroup</span></span>](transitionsgroup.md) <br/> |<span data-ttu-id="e6496-114">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e6496-114">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e6496-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e6496-115">Parent elements</span></span>

|<span data-ttu-id="e6496-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e6496-116">**Element**</span></span>|<span data-ttu-id="e6496-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e6496-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6496-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="e6496-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="e6496-119">Определяет часовой пояс времени начала [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e6496-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="e6496-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="e6496-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="e6496-121">Определяет часовой пояс для времени окончания [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="e6496-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="e6496-122">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="e6496-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="e6496-123">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="e6496-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e6496-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="e6496-124">Remarks</span></span>

<span data-ttu-id="e6496-125">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e6496-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6496-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e6496-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6496-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e6496-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e6496-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e6496-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e6496-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e6496-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="e6496-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e6496-130">Validation File</span></span>  <br/> |<span data-ttu-id="e6496-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e6496-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e6496-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e6496-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6496-133">False</span><span class="sxs-lookup"><span data-stu-id="e6496-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6496-134">См. также</span><span class="sxs-lookup"><span data-stu-id="e6496-134">See also</span></span>



- [<span data-ttu-id="e6496-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e6496-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

