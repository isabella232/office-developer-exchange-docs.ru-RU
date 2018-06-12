---
title: Периоды
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: Элемент периоды представляет массив периодов, которые определяют смещение времени на различных этапах часового пояса.
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834729"
---
# <a name="periods"></a><span data-ttu-id="c7c00-103">Периоды</span><span class="sxs-lookup"><span data-stu-id="c7c00-103">Periods</span></span>

<span data-ttu-id="c7c00-104">Элемент **периоды** представляет массив периодов, которые определяют смещение времени на различных этапах часового пояса.</span><span class="sxs-lookup"><span data-stu-id="c7c00-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="c7c00-105">**NonEmptyArrayOfPeriodsType**</span><span class="sxs-lookup"><span data-stu-id="c7c00-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c7c00-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c7c00-106">Attributes and elements</span></span>

<span data-ttu-id="c7c00-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c7c00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c7c00-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c7c00-108">Attributes</span></span>

<span data-ttu-id="c7c00-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="c7c00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c7c00-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c7c00-110">Child elements</span></span>

|<span data-ttu-id="c7c00-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7c00-111">**Element**</span></span>|<span data-ttu-id="c7c00-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7c00-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c00-113">Период</span><span class="sxs-lookup"><span data-stu-id="c7c00-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="c7c00-114">Определяет имя, смещение времени и уникальный идентификатор для конкретного этапа часового пояса.</span><span class="sxs-lookup"><span data-stu-id="c7c00-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c7c00-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c7c00-115">Parent elements</span></span>

|<span data-ttu-id="c7c00-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c7c00-116">**Element**</span></span>|<span data-ttu-id="c7c00-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c7c00-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c7c00-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7c00-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="c7c00-119">Определяет часовой пояс для времени начала [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c7c00-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="c7c00-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="c7c00-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="c7c00-121">Определяет часовой пояс для время окончания [элемента календаря, имеющего](calendaritem.md) или [MeetingRequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="c7c00-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="c7c00-122">Определение часового пояса</span><span class="sxs-lookup"><span data-stu-id="c7c00-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="c7c00-123">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="c7c00-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c7c00-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="c7c00-124">Remarks</span></span>

<span data-ttu-id="c7c00-125">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c7c00-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c7c00-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c7c00-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c7c00-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c7c00-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c7c00-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c7c00-128">Schema Name</span></span>  <br/> |<span data-ttu-id="c7c00-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c7c00-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="c7c00-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c7c00-130">Validation File</span></span>  <br/> |<span data-ttu-id="c7c00-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c7c00-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c7c00-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c7c00-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="c7c00-133">False</span><span class="sxs-lookup"><span data-stu-id="c7c00-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c7c00-134">См. также</span><span class="sxs-lookup"><span data-stu-id="c7c00-134">See also</span></span>



- [<span data-ttu-id="c7c00-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c7c00-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

