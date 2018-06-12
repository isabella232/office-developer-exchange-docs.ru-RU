---
title: BusyType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BusyType
api_type:
- schema
ms.assetid: 26d4fae0-8c78-4705-b5e8-d6033712c41e
description: Элемент BusyType представляет состояние сведений о доступности для события календаря.
ms.openlocfilehash: 6484bc70c6a05084e5d2bc1738b575fbebe4c132
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761635"
---
# <a name="busytype"></a><span data-ttu-id="1a57f-103">BusyType</span><span class="sxs-lookup"><span data-stu-id="1a57f-103">BusyType</span></span>

<span data-ttu-id="1a57f-104">Элемент **BusyType** представляет состояние сведений о доступности для события календаря.</span><span class="sxs-lookup"><span data-stu-id="1a57f-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="1a57f-105">**BusyType**</span><span class="sxs-lookup"><span data-stu-id="1a57f-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a57f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a57f-106">Attributes and elements</span></span>

<span data-ttu-id="1a57f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1a57f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a57f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a57f-108">Attributes</span></span>

<span data-ttu-id="1a57f-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a57f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1a57f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a57f-110">Child elements</span></span>

<span data-ttu-id="1a57f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="1a57f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1a57f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a57f-112">Parent elements</span></span>

|<span data-ttu-id="1a57f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1a57f-113">**Element**</span></span>|<span data-ttu-id="1a57f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a57f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1a57f-115">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="1a57f-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="1a57f-116">Содержит пользователя или контакта состояния занятости для временной интервал, что происходит в то же время, как время предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="1a57f-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="1a57f-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1a57f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="1a57f-118">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="1a57f-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="1a57f-119">Представляет вхождение элемента уникальный календаря.</span><span class="sxs-lookup"><span data-stu-id="1a57f-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="1a57f-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="1a57f-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1a57f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1a57f-121">Text value</span></span>

<span data-ttu-id="1a57f-122">Для этого элемента требуется указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="1a57f-122">A text value is required for this element.</span></span> <span data-ttu-id="1a57f-123">Значение типа string.</span><span class="sxs-lookup"><span data-stu-id="1a57f-123">The value is a string type.</span></span> <span data-ttu-id="1a57f-124">Ниже приведены возможные значения для элемента [BusyType](busytype.md) :</span><span class="sxs-lookup"><span data-stu-id="1a57f-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="1a57f-125">Свободна</span><span class="sxs-lookup"><span data-stu-id="1a57f-125">Free</span></span>
    
- <span data-ttu-id="1a57f-126">Под вопросом</span><span class="sxs-lookup"><span data-stu-id="1a57f-126">Tentative</span></span>
    
- <span data-ttu-id="1a57f-127">Занята</span><span class="sxs-lookup"><span data-stu-id="1a57f-127">Busy</span></span>
    
- <span data-ttu-id="1a57f-128">ОБ ОТСУТСТВИИ НА РАБОТЕ</span><span class="sxs-lookup"><span data-stu-id="1a57f-128">OOF</span></span>
    
- <span data-ttu-id="1a57f-129">NoData</span><span class="sxs-lookup"><span data-stu-id="1a57f-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="1a57f-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="1a57f-130">Remarks</span></span>

<span data-ttu-id="1a57f-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1a57f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a57f-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a57f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a57f-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a57f-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a57f-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a57f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="1a57f-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1a57f-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a57f-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a57f-136">Validation File</span></span>  <br/> |<span data-ttu-id="1a57f-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a57f-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a57f-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a57f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="1a57f-139">False</span><span class="sxs-lookup"><span data-stu-id="1a57f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1a57f-140">См. также</span><span class="sxs-lookup"><span data-stu-id="1a57f-140">See also</span></span>



[<span data-ttu-id="1a57f-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="1a57f-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="1a57f-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="1a57f-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="1a57f-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="1a57f-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

