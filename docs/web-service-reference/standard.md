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
ms.openlocfilehash: c121e959f243d982cfe50ed6b4ef39a82dae2cc8
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353436"
---
# <a name="standard"></a><span data-ttu-id="bc49a-103">Standard</span><span class="sxs-lookup"><span data-stu-id="bc49a-103">Standard</span></span>

<span data-ttu-id="bc49a-104">**Стандартный** элемент представляет дату и время изменения времени с летнего времени на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="bc49a-104">The **Standard** element represents the date and time when the time changes from daylight saving time to standard time.</span></span> 
  
```xml
<Standard TimeZoneName="">
   <Offset/>
   <RelativeYearlyRecurrence/>
   <Time/>
</Standard>
```

```xml
<Standard TimeZoneName="">
   <Offset/>
   <AbsoluteDate/>
   <Time/>
</Standard>
```

<span data-ttu-id="bc49a-105">**TimeChangeType**</span><span class="sxs-lookup"><span data-stu-id="bc49a-105">**TimeChangeType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bc49a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc49a-106">Attributes and elements</span></span>

<span data-ttu-id="bc49a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="bc49a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc49a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc49a-108">Attributes</span></span>

|<span data-ttu-id="bc49a-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="bc49a-109">**Attribute**</span></span>|<span data-ttu-id="bc49a-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc49a-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bc49a-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="bc49a-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="bc49a-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc49a-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bc49a-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc49a-113">Child elements</span></span>

|<span data-ttu-id="bc49a-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc49a-114">**Element**</span></span>|<span data-ttu-id="bc49a-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc49a-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc49a-116">Смещение</span><span class="sxs-lookup"><span data-stu-id="bc49a-116">Offset</span></span>](offset.md) <br/> |<span data-ttu-id="bc49a-117">Описание смещения от [BaseOffset](baseoffset.md).</span><span class="sxs-lookup"><span data-stu-id="bc49a-117">Describes the offset from the [BaseOffset](baseoffset.md).</span></span> <span data-ttu-id="bc49a-118">Вместе с **BaseOffset** элемент элемент **смещение** определяет, является ли время стандартное время или летнее время.</span><span class="sxs-lookup"><span data-stu-id="bc49a-118">Together with the **BaseOffset** element, the **Offset** element identifies whether the time is standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="bc49a-119">RelativeYearlyRecurrence</span><span class="sxs-lookup"><span data-stu-id="bc49a-119">RelativeYearlyRecurrence</span></span>](relativeyearlyrecurrence.md) <br/> |<span data-ttu-id="bc49a-120">Описывает относительное ежегодно повторяющейся для даты перехода часового пояса.</span><span class="sxs-lookup"><span data-stu-id="bc49a-120">Describes a relative yearly recurrence pattern for a time zone transition date.</span></span>  <br/> |
|[<span data-ttu-id="bc49a-121">AbsoluteDate</span><span class="sxs-lookup"><span data-stu-id="bc49a-121">AbsoluteDate</span></span>](absolutedate.md) <br/> |<span data-ttu-id="bc49a-122">Представляет дату, когда время изменяется с стандартное или летнее время.</span><span class="sxs-lookup"><span data-stu-id="bc49a-122">Represents the date when the time changes from standard time or daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="bc49a-123">Time (TimeChangeType)</span><span class="sxs-lookup"><span data-stu-id="bc49a-123">Time (TimeChangeType)</span></span>](time-timechangetype.md) <br/> |<span data-ttu-id="bc49a-124">Описание момента изменения времени между зимнего и летнего времени.</span><span class="sxs-lookup"><span data-stu-id="bc49a-124">Describes the time when the time changes between standard time and daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc49a-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc49a-125">Parent elements</span></span>

|<span data-ttu-id="bc49a-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc49a-126">**Element**</span></span>|<span data-ttu-id="bc49a-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc49a-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc49a-128">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="bc49a-128">MeetingTimeZone</span></span>](meetingtimezone.md) <br/> |<span data-ttu-id="bc49a-129">Представляет часовой пояс расположение, где размещен собрания.</span><span class="sxs-lookup"><span data-stu-id="bc49a-129">Represents the time zone of the location where the meeting is hosted.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc49a-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="bc49a-130">Remarks</span></span>

<span data-ttu-id="bc49a-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере, работающем под управлением Microsoft Exchange Server 2007, с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="bc49a-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc49a-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc49a-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc49a-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc49a-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="bc49a-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc49a-134">Schema Name</span></span>  <br/> |<span data-ttu-id="bc49a-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="bc49a-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="bc49a-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc49a-136">Validation File</span></span>  <br/> |<span data-ttu-id="bc49a-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="bc49a-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="bc49a-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc49a-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc49a-139">False</span><span class="sxs-lookup"><span data-stu-id="bc49a-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc49a-140">См. также</span><span class="sxs-lookup"><span data-stu-id="bc49a-140">See also</span></span>

- [<span data-ttu-id="bc49a-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bc49a-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

