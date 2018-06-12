---
title: MeetingTimeZone
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTimeZone
api_type:
- schema
ms.assetid: 413b47d9-8126-462c-9a4f-4e771a5e8889
description: Элемент MeetingTimeZone представляет часовой пояс расположение, где размещен собрания.
ms.openlocfilehash: ce014ac6d8841e451927a94049cb4e8860886fdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834440"
---
# <a name="meetingtimezone"></a><span data-ttu-id="fdae1-103">MeetingTimeZone</span><span class="sxs-lookup"><span data-stu-id="fdae1-103">MeetingTimeZone</span></span>

<span data-ttu-id="fdae1-104">Элемент **MeetingTimeZone** представляет часовой пояс расположение, где размещен собрания.</span><span class="sxs-lookup"><span data-stu-id="fdae1-104">The **MeetingTimeZone** element represents the time zone of the location where the meeting is hosted.</span></span> 
  
```xml
<MeetingTimeZone>
   <BaseOffset/>
   <Standard/>
   <Daylight/>
</MeetingTimeZone>
```

 <span data-ttu-id="fdae1-105">**TimeZoneType**</span><span class="sxs-lookup"><span data-stu-id="fdae1-105">**TimeZoneType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fdae1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fdae1-106">Attributes and elements</span></span>

<span data-ttu-id="fdae1-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fdae1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fdae1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fdae1-108">Attributes</span></span>

|<span data-ttu-id="fdae1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="fdae1-109">**Attribute**</span></span>|<span data-ttu-id="fdae1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fdae1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fdae1-111">**TimeZoneName**</span><span class="sxs-lookup"><span data-stu-id="fdae1-111">**TimeZoneName**</span></span> <br/> |<span data-ttu-id="fdae1-112">Описывает имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="fdae1-112">Describes the name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fdae1-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fdae1-113">Child elements</span></span>

|<span data-ttu-id="fdae1-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fdae1-114">**Element**</span></span>|<span data-ttu-id="fdae1-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fdae1-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdae1-116">BaseOffset</span><span class="sxs-lookup"><span data-stu-id="fdae1-116">BaseOffset</span></span>](baseoffset.md) <br/> |<span data-ttu-id="fdae1-117">Представляет ежечасно смещение от времени UTC для текущего часового пояса.</span><span class="sxs-lookup"><span data-stu-id="fdae1-117">Represents the hourly offset from UTC for the current time zone.</span></span>  <br/> |
|[<span data-ttu-id="fdae1-118">Стандартный</span><span class="sxs-lookup"><span data-stu-id="fdae1-118">Standard</span></span>](standard.md) <br/> |<span data-ttu-id="fdae1-119">Представляет дату и время изменения времени с летнего времени на стандартное время.</span><span class="sxs-lookup"><span data-stu-id="fdae1-119">Represents the date and time when the time changes from daylight saving time to standard time.</span></span>  <br/> |
|[<span data-ttu-id="fdae1-120">Переход на летнее</span><span class="sxs-lookup"><span data-stu-id="fdae1-120">Daylight</span></span>](daylight.md) <br/> |<span data-ttu-id="fdae1-121">Представляет дату и время изменения времени с зимнего на летнее время.</span><span class="sxs-lookup"><span data-stu-id="fdae1-121">Represents the date and time when the time changes from standard time to daylight saving time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fdae1-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fdae1-122">Parent elements</span></span>

|<span data-ttu-id="fdae1-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fdae1-123">**Element**</span></span>|<span data-ttu-id="fdae1-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fdae1-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fdae1-125">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="fdae1-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="fdae1-126">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdae1-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="fdae1-127">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="fdae1-127">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="fdae1-128">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="fdae1-128">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fdae1-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="fdae1-129">Remarks</span></span>

<span data-ttu-id="fdae1-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fdae1-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fdae1-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fdae1-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fdae1-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fdae1-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fdae1-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fdae1-133">Schema Name</span></span>  <br/> |<span data-ttu-id="fdae1-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fdae1-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="fdae1-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fdae1-135">Validation File</span></span>  <br/> |<span data-ttu-id="fdae1-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fdae1-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fdae1-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fdae1-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="fdae1-138">False</span><span class="sxs-lookup"><span data-stu-id="fdae1-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fdae1-139">См. также</span><span class="sxs-lookup"><span data-stu-id="fdae1-139">See also</span></span>



- [<span data-ttu-id="fdae1-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="fdae1-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

