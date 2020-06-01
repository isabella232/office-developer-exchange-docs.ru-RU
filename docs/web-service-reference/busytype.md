---
title: буситипе
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
description: Элемент Буситипе представляет состояние занятости, заданное для события календаря.
ms.openlocfilehash: 7c2d18c21156a8603d3caeeb796a56c5d8afcba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459085"
---
# <a name="busytype"></a><span data-ttu-id="cbb6f-103">буситипе</span><span class="sxs-lookup"><span data-stu-id="cbb6f-103">BusyType</span></span>

<span data-ttu-id="cbb6f-104">Элемент **буситипе** представляет состояние занятости, заданное для события календаря.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-104">The **BusyType** element represents the free/busy status set for a calendar event.</span></span> 
  
```xml
<BusyType>Free or Tentative or Busy or OOF or NoData</BusyType>
```

 <span data-ttu-id="cbb6f-105">**буситипе**</span><span class="sxs-lookup"><span data-stu-id="cbb6f-105">**BusyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbb6f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cbb6f-106">Attributes and elements</span></span>

<span data-ttu-id="cbb6f-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbb6f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cbb6f-108">Attributes</span></span>

<span data-ttu-id="cbb6f-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbb6f-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cbb6f-110">Child elements</span></span>

<span data-ttu-id="cbb6f-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbb6f-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cbb6f-112">Parent elements</span></span>

|<span data-ttu-id="cbb6f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cbb6f-113">**Element**</span></span>|<span data-ttu-id="cbb6f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cbb6f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbb6f-115">индивидуалаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="cbb6f-115">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="cbb6f-116">Содержит сведения о доступности пользователя или контакта для периода времени, выполняемого одновременно с предложенным временем собрания.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-116">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time.</span></span>  <br/> <span data-ttu-id="cbb6f-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="cbb6f-117">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/IndividualAttendeeConflictData` <br/> |
|[<span data-ttu-id="cbb6f-118">календаревент</span><span class="sxs-lookup"><span data-stu-id="cbb6f-118">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="cbb6f-119">Представляет уникальное вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-119">Represents a unique calendar item occurrence.</span></span>  <br/> <span data-ttu-id="cbb6f-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="cbb6f-120">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cbb6f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cbb6f-121">Text value</span></span>

<span data-ttu-id="cbb6f-122">Для этого элемента требуется указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-122">A text value is required for this element.</span></span> <span data-ttu-id="cbb6f-123">Значением является строковый тип.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-123">The value is a string type.</span></span> <span data-ttu-id="cbb6f-124">Ниже приведены возможные значения для элемента [буситипе](busytype.md) .</span><span class="sxs-lookup"><span data-stu-id="cbb6f-124">The following are the possible values for the [BusyType](busytype.md) element:</span></span> 
  
- <span data-ttu-id="cbb6f-125">Свободна</span><span class="sxs-lookup"><span data-stu-id="cbb6f-125">Free</span></span>
    
- <span data-ttu-id="cbb6f-126">Занят</span><span class="sxs-lookup"><span data-stu-id="cbb6f-126">Tentative</span></span>
    
- <span data-ttu-id="cbb6f-127">Занята</span><span class="sxs-lookup"><span data-stu-id="cbb6f-127">Busy</span></span>
    
- <span data-ttu-id="cbb6f-128">OOF</span><span class="sxs-lookup"><span data-stu-id="cbb6f-128">OOF</span></span>
    
- <span data-ttu-id="cbb6f-129">NoData</span><span class="sxs-lookup"><span data-stu-id="cbb6f-129">NoData</span></span>
    
## <a name="remarks"></a><span data-ttu-id="cbb6f-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="cbb6f-130">Remarks</span></span>

<span data-ttu-id="cbb6f-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cbb6f-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbb6f-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="cbb6f-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbb6f-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="cbb6f-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbb6f-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="cbb6f-134">Schema Name</span></span>  <br/> |<span data-ttu-id="cbb6f-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="cbb6f-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbb6f-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="cbb6f-136">Validation File</span></span>  <br/> |<span data-ttu-id="cbb6f-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="cbb6f-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbb6f-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="cbb6f-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="cbb6f-139">False</span><span class="sxs-lookup"><span data-stu-id="cbb6f-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbb6f-140">См. также</span><span class="sxs-lookup"><span data-stu-id="cbb6f-140">See also</span></span>



[<span data-ttu-id="cbb6f-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="cbb6f-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="cbb6f-142">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="cbb6f-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="cbb6f-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="cbb6f-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

