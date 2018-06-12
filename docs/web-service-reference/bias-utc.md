---
title: Смещение (UTC)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: Элемент Bias представляет общие смещение в формате UTC. Это значение представлено в минутах.
ms.openlocfilehash: 43613593565ca15be97bd2a98dbe5c512dbe5fc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761559"
---
# <a name="bias-utc"></a><span data-ttu-id="692f7-104">Смещение (UTC)</span><span class="sxs-lookup"><span data-stu-id="692f7-104">Bias (UTC)</span></span>

<span data-ttu-id="692f7-105">Элемент **Bias** представляет общие смещение в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="692f7-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="692f7-106">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="692f7-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="692f7-107">**int**</span><span class="sxs-lookup"><span data-stu-id="692f7-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="692f7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="692f7-108">Attributes and elements</span></span>

<span data-ttu-id="692f7-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="692f7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="692f7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="692f7-110">Attributes</span></span>

<span data-ttu-id="692f7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="692f7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="692f7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="692f7-112">Child elements</span></span>

<span data-ttu-id="692f7-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="692f7-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="692f7-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="692f7-114">Parent elements</span></span>

|<span data-ttu-id="692f7-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="692f7-115">**Element**</span></span>|<span data-ttu-id="692f7-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="692f7-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="692f7-117">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="692f7-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="692f7-118">Контейнер, определяющий сведения даты и времени запроса.</span><span class="sxs-lookup"><span data-stu-id="692f7-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="692f7-119">Этот элемент содержит сведения о переходе между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="692f7-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="692f7-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="692f7-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="692f7-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="692f7-121">Text value</span></span>

<span data-ttu-id="692f7-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="692f7-122">A text value is required.</span></span> <span data-ttu-id="692f7-123">Текстовое значение представляет собой целое число.</span><span class="sxs-lookup"><span data-stu-id="692f7-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="692f7-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="692f7-124">Remarks</span></span>

<span data-ttu-id="692f7-125">Второй элемент [Bias](bias.md) в схеме представляет смещение из смещения по Гринвичу (UTC).</span><span class="sxs-lookup"><span data-stu-id="692f7-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="692f7-126">Пример</span><span class="sxs-lookup"><span data-stu-id="692f7-126">Example</span></span>

<span data-ttu-id="692f7-127">Следующий пример показывает часть запроса XML, который определяет смещение-8 часов от времени UTC в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="692f7-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="692f7-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="692f7-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="692f7-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="692f7-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="692f7-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="692f7-130">Schema Name</span></span>  <br/> |<span data-ttu-id="692f7-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="692f7-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="692f7-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="692f7-132">Validation File</span></span>  <br/> |<span data-ttu-id="692f7-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="692f7-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="692f7-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="692f7-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="692f7-135">False</span><span class="sxs-lookup"><span data-stu-id="692f7-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="692f7-136">См. также</span><span class="sxs-lookup"><span data-stu-id="692f7-136">See also</span></span>

- [<span data-ttu-id="692f7-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="692f7-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="692f7-138">Уровень защиты</span><span class="sxs-lookup"><span data-stu-id="692f7-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="692f7-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="692f7-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

