---
title: Время окончания
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: Элемент EndTime представляет конец промежуток времени.
ms.openlocfilehash: 7d3d186618a7bcc05ad82532e13e03d2e67a0e40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762370"
---
# <a name="endtime"></a><span data-ttu-id="21f5a-103">Время окончания</span><span class="sxs-lookup"><span data-stu-id="21f5a-103">EndTime</span></span>

<span data-ttu-id="21f5a-104">Элемент **EndTime** представляет конец промежуток времени.</span><span class="sxs-lookup"><span data-stu-id="21f5a-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="21f5a-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="21f5a-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21f5a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="21f5a-106">Attributes and elements</span></span>

<span data-ttu-id="21f5a-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="21f5a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21f5a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="21f5a-108">Attributes</span></span>

<span data-ttu-id="21f5a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="21f5a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="21f5a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="21f5a-110">Child elements</span></span>

<span data-ttu-id="21f5a-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="21f5a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="21f5a-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="21f5a-112">Parent elements</span></span>

|<span data-ttu-id="21f5a-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="21f5a-113">**Element**</span></span>|<span data-ttu-id="21f5a-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="21f5a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21f5a-115">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="21f5a-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="21f5a-116">Определяет период времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="21f5a-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="21f5a-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="21f5a-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="21f5a-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="21f5a-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="21f5a-119">Определяет период времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="21f5a-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="21f5a-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="21f5a-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="21f5a-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="21f5a-121"></span></span>  <br/> |
|[<span data-ttu-id="21f5a-122">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="21f5a-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="21f5a-123">Указывает, во время выполнения, для которого включен состояние об отсутствии на работе Office (OOF), если элемент [OofState](oofstate.md) задано значение **расписанию**.</span><span class="sxs-lookup"><span data-stu-id="21f5a-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="21f5a-124">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="21f5a-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="21f5a-125">Вхождение</span><span class="sxs-lookup"><span data-stu-id="21f5a-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="21f5a-126">Представляет измененной вхождения повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="21f5a-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="21f5a-127">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="21f5a-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="21f5a-128">Представляет вхождение элемента уникальный календаря.</span><span class="sxs-lookup"><span data-stu-id="21f5a-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="21f5a-129">Используется для обеспечения доступности запросы.</span><span class="sxs-lookup"><span data-stu-id="21f5a-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="21f5a-130">Элемент **EndTime** является обязательным в элементе **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="21f5a-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="21f5a-131">Элемент **EndTime** в элементе **CalendarEvent** является уникальным для типа **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="21f5a-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="21f5a-132">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="21f5a-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21f5a-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="21f5a-133">Text value</span></span>

<span data-ttu-id="21f5a-134">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="21f5a-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21f5a-135">Замечания</span><span class="sxs-lookup"><span data-stu-id="21f5a-135">Remarks</span></span>

<span data-ttu-id="21f5a-136">Элемент [StartTime](starttime.md) представляет начало периода времени.</span><span class="sxs-lookup"><span data-stu-id="21f5a-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="21f5a-137">Время окончания представляет времени клиента.</span><span class="sxs-lookup"><span data-stu-id="21f5a-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="21f5a-138">Схема включает в себя многие элементы [EndTime](endtime.md) .</span><span class="sxs-lookup"><span data-stu-id="21f5a-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="21f5a-139">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="21f5a-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="21f5a-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="21f5a-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21f5a-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="21f5a-141">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="21f5a-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="21f5a-142">Schema Name</span></span>  <br/> |<span data-ttu-id="21f5a-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="21f5a-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="21f5a-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="21f5a-144">Validation File</span></span>  <br/> |<span data-ttu-id="21f5a-145">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="21f5a-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="21f5a-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="21f5a-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="21f5a-147">False</span><span class="sxs-lookup"><span data-stu-id="21f5a-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21f5a-148">См. также</span><span class="sxs-lookup"><span data-stu-id="21f5a-148">See also</span></span>

- [<span data-ttu-id="21f5a-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="21f5a-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="21f5a-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="21f5a-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

