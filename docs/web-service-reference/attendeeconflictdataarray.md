---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: Элемент AttendeeConflictDataArray содержит массив данных конфликта запрашиваемого участников, определенный в операция GetUserAvailability.
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761517"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="de31a-103">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="de31a-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="de31a-104">Элемент **AttendeeConflictDataArray** содержит массив данных конфликта запрашиваемого участников, определенный в [операция GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="de31a-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="de31a-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de31a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="de31a-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="de31a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="de31a-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="de31a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="de31a-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="de31a-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="de31a-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="de31a-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="de31a-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="de31a-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="de31a-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="de31a-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="de31a-112">**ArrayOfAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="de31a-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="de31a-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="de31a-113">Attributes and elements</span></span>

<span data-ttu-id="de31a-114">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="de31a-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de31a-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="de31a-115">Attributes</span></span>

<span data-ttu-id="de31a-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="de31a-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="de31a-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="de31a-117">Child elements</span></span>

|<span data-ttu-id="de31a-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="de31a-118">**Element**</span></span>|<span data-ttu-id="de31a-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="de31a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de31a-120">UnknownAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="de31a-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="de31a-121">Представляет неразрешимые участника или участника, который не является пользователем, список рассылки или контактов.</span><span class="sxs-lookup"><span data-stu-id="de31a-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="de31a-122">IndividualAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="de31a-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="de31a-123">Содержит пользователя или контакта состояния занятости для временной интервал, что происходит в то же время согласно предложениям время, обнаруженных в элементе [предложение](suggestion.md) собрания.</span><span class="sxs-lookup"><span data-stu-id="de31a-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="de31a-124">TooBigGroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="de31a-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="de31a-125">Представляет участника, которая разрешается в качестве список рассылки, который был слишком велик для разверните узел.</span><span class="sxs-lookup"><span data-stu-id="de31a-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="de31a-126">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="de31a-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="de31a-127">Содержит конфликта статистические сведения об число доступных пользователей, число пользователей, имеющих конфликтов и количество пользователей, у которых нет сведений о доступности в списке рассылки для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="de31a-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de31a-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="de31a-128">Parent elements</span></span>

|<span data-ttu-id="de31a-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="de31a-129">**Element**</span></span>|<span data-ttu-id="de31a-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="de31a-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de31a-131">Предложения</span><span class="sxs-lookup"><span data-stu-id="de31a-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="de31a-132">Представляет один предложения о времени на собрания.</span><span class="sxs-lookup"><span data-stu-id="de31a-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="de31a-133">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="de31a-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="de31a-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="de31a-134">Remarks</span></span>

<span data-ttu-id="de31a-135">Положение каждого элемента в **AttendeeConflictDataArray** соответствует положение запрошенного участников в элементе [MailboxDataArray](mailboxdataarray.md) .</span><span class="sxs-lookup"><span data-stu-id="de31a-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="de31a-136">Каждого запроса участника должен соответствовать одному из **AttendeeConflictDataArray** дочерние элементы.</span><span class="sxs-lookup"><span data-stu-id="de31a-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="de31a-137">Эти элементы представляют отдельного конфликта с временем предложенного собрания, обнаруженных в элементе [предложения](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="de31a-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="de31a-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="de31a-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="de31a-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="de31a-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de31a-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="de31a-140">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="de31a-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="de31a-141">Schema Name</span></span>  <br/> |<span data-ttu-id="de31a-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="de31a-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="de31a-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="de31a-143">Validation File</span></span>  <br/> |<span data-ttu-id="de31a-144">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="de31a-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="de31a-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="de31a-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="de31a-146">False</span><span class="sxs-lookup"><span data-stu-id="de31a-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de31a-147">См. также</span><span class="sxs-lookup"><span data-stu-id="de31a-147">See also</span></span>

- [<span data-ttu-id="de31a-148">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="de31a-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="de31a-149">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="de31a-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="de31a-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="de31a-150">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

