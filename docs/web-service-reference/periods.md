---
title: Periods
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
description: Элемент Periods представляет массив периодов, которые определяют смещение времени на разных стадиях часового пояса.
ms.openlocfilehash: f2f9cf7c724b453d2b1975fcf72c55bc02caa54b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834729"
---
# <a name="periods"></a><span data-ttu-id="81c18-103">Periods</span><span class="sxs-lookup"><span data-stu-id="81c18-103">Periods</span></span>

<span data-ttu-id="81c18-104">Элемент **Periods** представляет массив периодов, которые определяют смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81c18-104">The **Periods** element represents an array of periods that define the time offset at different stages of the time zone.</span></span> 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 <span data-ttu-id="81c18-105">**нонемптяррайофпериодстипе**</span><span class="sxs-lookup"><span data-stu-id="81c18-105">**NonEmptyArrayOfPeriodsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81c18-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81c18-106">Attributes and elements</span></span>

<span data-ttu-id="81c18-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="81c18-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81c18-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81c18-108">Attributes</span></span>

<span data-ttu-id="81c18-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="81c18-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81c18-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81c18-110">Child elements</span></span>

|<span data-ttu-id="81c18-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c18-111">**Element**</span></span>|<span data-ttu-id="81c18-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c18-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c18-113">Period</span><span class="sxs-lookup"><span data-stu-id="81c18-113">Period</span></span>](period.md) <br/> |<span data-ttu-id="81c18-114">Определяет имя, смещение времени и уникальный идентификатор для определенного этапа часового пояса.</span><span class="sxs-lookup"><span data-stu-id="81c18-114">Defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="81c18-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81c18-115">Parent elements</span></span>

|<span data-ttu-id="81c18-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c18-116">**Element**</span></span>|<span data-ttu-id="81c18-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c18-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c18-118">StartTimeZone</span><span class="sxs-lookup"><span data-stu-id="81c18-118">StartTimeZone</span></span>](starttimezone.md) <br/> |<span data-ttu-id="81c18-119">Определяет часовой пояс времени начала [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="81c18-119">Defines the time zone for the start time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="81c18-120">EndTimeZone</span><span class="sxs-lookup"><span data-stu-id="81c18-120">EndTimeZone</span></span>](endtimezone.md) <br/> |<span data-ttu-id="81c18-121">Определяет часовой пояс для времени окончания [календаритем](calendaritem.md) или [свойство meetingrequest](meetingrequest.md).</span><span class="sxs-lookup"><span data-stu-id="81c18-121">Defines the time zone for the end time of a [CalendarItem](calendaritem.md) or [MeetingRequest](meetingrequest.md).</span></span>  <br/> |
|[<span data-ttu-id="81c18-122">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="81c18-122">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="81c18-123">Определяет часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="81c18-123">Defines a time zone.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="81c18-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="81c18-124">Remarks</span></span>

<span data-ttu-id="81c18-125">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="81c18-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81c18-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81c18-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81c18-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81c18-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81c18-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81c18-128">Schema Name</span></span>  <br/> |<span data-ttu-id="81c18-129">Схема Types</span><span class="sxs-lookup"><span data-stu-id="81c18-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="81c18-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81c18-130">Validation File</span></span>  <br/> |<span data-ttu-id="81c18-131">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="81c18-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81c18-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81c18-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="81c18-133">False</span><span class="sxs-lookup"><span data-stu-id="81c18-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81c18-134">См. также</span><span class="sxs-lookup"><span data-stu-id="81c18-134">See also</span></span>



- [<span data-ttu-id="81c18-135">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="81c18-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

