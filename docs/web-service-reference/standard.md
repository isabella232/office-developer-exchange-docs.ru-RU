---
title: Standard
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Standard
api_type:
- schema
ms.assetid: d598f0a6-e296-423f-8ce5-3da57cfd8189
description: Стандартный элемент представляет дату и время изменения времени с летнего времени на стандартное время.
ms.openlocfilehash: 1c9be4cf35773583078bc8e16ddf44433d3ad98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835536"
---
# <a name="standard"></a><span data-ttu-id="ab021-103">Standard</span><span class="sxs-lookup"><span data-stu-id="ab021-103">Standard</span></span>

<span data-ttu-id="ab021-104">**Стандартный** элемент представляет дату и время изменения времени с летнего времени на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="ab021-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

 <span data-ttu-id="ab021-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="ab021-105">**TimeChangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ab021-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ab021-106">Attributes and elements</span></span>

<span data-ttu-id="ab021-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ab021-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ab021-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ab021-108">Attributes</span></span>

|<span data-ttu-id="ab021-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="ab021-109">**Attribute**</span></span>|<span data-ttu-id="ab021-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab021-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ab021-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="ab021-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="ab021-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="ab021-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ab021-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ab021-113">Child elements</span></span>

|<span data-ttu-id="ab021-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ab021-114">**Element**</span></span>|<span data-ttu-id="ab021-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab021-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab021-116">Смещение</span><span class="sxs-lookup"><span data-stu-id="ab021-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="ab021-117">Описание смещения от [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="ab021-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="ab021-118">Вместе с **BaseOffset** элемент элемент **смещение** определяет, является ли время стандартное время или летнее время.</span><span class="sxs-lookup"><span data-stu-id="ab021-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="ab021-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="ab021-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="ab021-120">Описывает относительное ежегодно повторяющейся для даты перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="ab021-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="ab021-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="ab021-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="ab021-122">Представляет дату, когда время изменяется с стандартное или летнее время.</span><span class="sxs-lookup"><span data-stu-id="ab021-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="ab021-123">Время (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="ab021-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="ab021-124">Описание момента изменения времени между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="ab021-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ab021-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ab021-125">Parent elements</span></span>

|<span data-ttu-id="ab021-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ab021-126">**Element**</span></span>|<span data-ttu-id="ab021-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ab021-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ab021-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="ab021-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="ab021-129">Представляет часовой пояс расположение, где размещен собрания.</span><span class="sxs-lookup"><span data-stu-id="ab021-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ab021-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="ab021-130">Remarks</span></span>

<span data-ttu-id="ab021-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ab021-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ab021-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ab021-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ab021-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ab021-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ab021-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ab021-134">Schema Name</span></span>  <br/> |<span data-ttu-id="ab021-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ab021-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="ab021-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ab021-136">Validation File</span></span>  <br/> |<span data-ttu-id="ab021-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ab021-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ab021-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ab021-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="ab021-139">False</span><span class="sxs-lookup"><span data-stu-id="ab021-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ab021-140">См. также</span><span class="sxs-lookup"><span data-stu-id="ab021-140">See also</span></span>



- [<span data-ttu-id="ab021-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ab021-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

