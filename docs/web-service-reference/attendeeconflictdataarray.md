---
title: аттендиконфликтдатааррай
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
description: Элемент Аттендиконфликтдатааррай содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в операции GetUserAvailability.
ms.openlocfilehash: 770e8c00ca248ec3562180dc9d3626fd5b58f4d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455802"
---
# <a name="attendeeconflictdataarray"></a><span data-ttu-id="ded59-103">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="ded59-103">AttendeeConflictDataArray</span></span>

<span data-ttu-id="ded59-104">Элемент **аттендиконфликтдатааррай** содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="ded59-104">The **AttendeeConflictDataArray** element contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>
  
- [<span data-ttu-id="ded59-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ded59-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="ded59-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="ded59-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
- [<span data-ttu-id="ded59-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="ded59-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
- [<span data-ttu-id="ded59-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="ded59-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
- [<span data-ttu-id="ded59-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="ded59-109">SuggestionArray</span></span>](suggestionarray.md)
  
- [<span data-ttu-id="ded59-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="ded59-110">Suggestion</span></span>](suggestion.md)
  
- [<span data-ttu-id="ded59-111">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="ded59-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 <span data-ttu-id="ded59-112">**аррайофаттендиконфликтдата**</span><span class="sxs-lookup"><span data-stu-id="ded59-112">**ArrayOfAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ded59-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ded59-113">Attributes and elements</span></span>

<span data-ttu-id="ded59-114">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ded59-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ded59-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ded59-115">Attributes</span></span>

<span data-ttu-id="ded59-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ded59-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ded59-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ded59-117">Child elements</span></span>

|<span data-ttu-id="ded59-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ded59-118">**Element**</span></span>|<span data-ttu-id="ded59-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ded59-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded59-120">ункновнаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="ded59-120">UnknownAttendeeConflictData</span></span>](unknownattendeeconflictdata.md) <br/> |<span data-ttu-id="ded59-121">Представляет неразрешимого участника или участника, который не является пользователем, списком рассылки или контактом.</span><span class="sxs-lookup"><span data-stu-id="ded59-121">Represents an unresolvable attendee or an attendee that is not a user, distribution list, or contact.</span></span>  <br/> |
|[<span data-ttu-id="ded59-122">индивидуалаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="ded59-122">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md) <br/> |<span data-ttu-id="ded59-123">Содержит сведения о занятости пользователя или контакта для временного периода, выполняемого одновременно с указанным в элементе [предложение](suggestion.md) временем собрания.</span><span class="sxs-lookup"><span data-stu-id="ded59-123">Contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span>  <br/> |
|[<span data-ttu-id="ded59-124">тубигграупаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="ded59-124">TooBigGroupAttendeeConflictData</span></span>](toobiggroupattendeeconflictdata.md) <br/> |<span data-ttu-id="ded59-125">Представляет участника, которое разрешалось как список рассылки, который был слишком большим для расширения.</span><span class="sxs-lookup"><span data-stu-id="ded59-125">Represents an attendee that resolved as a distribution list that was too large to expand.</span></span>  <br/> |
|[<span data-ttu-id="ded59-126">граупаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="ded59-126">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md) <br/> |<span data-ttu-id="ded59-127">Содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и количестве пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ded59-127">Contains aggregate conflict information about the number of users available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ded59-128">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ded59-128">Parent elements</span></span>

|<span data-ttu-id="ded59-129">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ded59-129">**Element**</span></span>|<span data-ttu-id="ded59-130">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ded59-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ded59-131">Предложение</span><span class="sxs-lookup"><span data-stu-id="ded59-131">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="ded59-132">Представляет один вариант времени собрания.</span><span class="sxs-lookup"><span data-stu-id="ded59-132">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="ded59-133">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ded59-133">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ded59-134">Примечания</span><span class="sxs-lookup"><span data-stu-id="ded59-134">Remarks</span></span>

<span data-ttu-id="ded59-135">Положение каждого элемента в **аттендиконфликтдатааррай** соответствует положению запрашиваемых участников в элементе [маилбоксдатааррай](mailboxdataarray.md) .</span><span class="sxs-lookup"><span data-stu-id="ded59-135">The position of each element in the **AttendeeConflictDataArray** corresponds to the position of the queried attendees in the [MailboxDataArray](mailboxdataarray.md) element.</span></span> <span data-ttu-id="ded59-136">Каждый запрашиваемый Участник должен соответствовать одному из дочерних элементов **аттендиконфликтдатааррай** .</span><span class="sxs-lookup"><span data-stu-id="ded59-136">Each queried attendee must correspond to one of the **AttendeeConflictDataArray** child elements.</span></span> <span data-ttu-id="ded59-137">Эти элементы представляют один конфликт с предложенным временем собрания, указанным в элементе " [предложение](suggestion.md) ".</span><span class="sxs-lookup"><span data-stu-id="ded59-137">These elements represent a single conflict with the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="ded59-138">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ded59-138">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ded59-139">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ded59-139">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ded59-140">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ded59-140">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ded59-141">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ded59-141">Schema Name</span></span>  <br/> |<span data-ttu-id="ded59-142">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ded59-142">Types schema</span></span>  <br/> |
|<span data-ttu-id="ded59-143">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ded59-143">Validation File</span></span>  <br/> |<span data-ttu-id="ded59-144">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ded59-144">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ded59-145">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ded59-145">Can be Empty</span></span>  <br/> |<span data-ttu-id="ded59-146">False</span><span class="sxs-lookup"><span data-stu-id="ded59-146">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ded59-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ded59-147">See also</span></span>

- [<span data-ttu-id="ded59-148">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ded59-148">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="ded59-149">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ded59-149">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="ded59-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="ded59-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

