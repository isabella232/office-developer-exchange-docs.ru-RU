---
title: индивидуалаттендиконфликтдата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IndividualAttendeeConflictData
api_type:
- schema
ms.assetid: d45d3c34-abe1-40da-afd3-23bc5c3ef474
description: Элемент Индивидуалаттендиконфликтдата содержит сведения о занятости пользователя или контакта для периода времени, выполняемого одновременно с предложенным временем собрания, указанным в элементе "предложение".
ms.openlocfilehash: 0bd164e08a6f3685415452b7c82a4220cf69d792
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833930"
---
# <a name="individualattendeeconflictdata"></a><span data-ttu-id="da169-103">индивидуалаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="da169-103">IndividualAttendeeConflictData</span></span>

<span data-ttu-id="da169-104">Элемент **индивидуалаттендиконфликтдата** содержит сведения о занятости пользователя или контакта для периода времени, выполняемого одновременно с предложенным временем собрания, указанным в элементе " [предложение](suggestion.md) ".</span><span class="sxs-lookup"><span data-stu-id="da169-104">The **IndividualAttendeeConflictData** element contains a user's or contact's free/busy status for a time window that occurs at the same time as the suggested meeting time identified in the [Suggestion](suggestion.md) element.</span></span> 
  
[<span data-ttu-id="da169-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="da169-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="da169-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="da169-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="da169-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="da169-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="da169-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="da169-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="da169-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="da169-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="da169-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="da169-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="da169-111">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="da169-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
  
[<span data-ttu-id="da169-112">индивидуалаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="da169-112">IndividualAttendeeConflictData</span></span>](individualattendeeconflictdata.md)
  
```xml
<IndividualAttendeeConflictData>
   <BusyType>...</BusyType>
</IndividualAttendeeConflictData>
```

 <span data-ttu-id="da169-113">**индивидуалаттендиконфликтдата**</span><span class="sxs-lookup"><span data-stu-id="da169-113">**IndividualAttendeeConflictData**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da169-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da169-114">Attributes and elements</span></span>

<span data-ttu-id="da169-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="da169-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da169-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da169-116">Attributes</span></span>

<span data-ttu-id="da169-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="da169-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da169-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da169-118">Child elements</span></span>

|<span data-ttu-id="da169-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da169-119">**Element**</span></span>|<span data-ttu-id="da169-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da169-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da169-121">буситипе</span><span class="sxs-lookup"><span data-stu-id="da169-121">BusyType</span></span>](busytype.md) <br/> |<span data-ttu-id="da169-122">Представляет сведения о доступности пользователя для предполагаемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="da169-122">Represents the free/busy status of a user for a suggested meeting time.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da169-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da169-123">Parent elements</span></span>

|<span data-ttu-id="da169-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da169-124">**Element**</span></span>|<span data-ttu-id="da169-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da169-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da169-126">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="da169-126">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="da169-127">Содержит массив данных о конфликтах для участников, идентифицируемых в [жетусераваилабилитирекуест](getuseravailabilityrequest.md).</span><span class="sxs-lookup"><span data-stu-id="da169-127">Contains an array of conflict data for attendees identified in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md).</span></span>  <br/> <span data-ttu-id="da169-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="da169-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da169-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="da169-129">Remarks</span></span>

<span data-ttu-id="da169-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="da169-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da169-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da169-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da169-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da169-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da169-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da169-133">Schema Name</span></span>  <br/> |<span data-ttu-id="da169-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da169-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="da169-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da169-135">Validation File</span></span>  <br/> |<span data-ttu-id="da169-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="da169-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da169-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da169-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="da169-138">False</span><span class="sxs-lookup"><span data-stu-id="da169-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da169-139">См. также</span><span class="sxs-lookup"><span data-stu-id="da169-139">See also</span></span>



[<span data-ttu-id="da169-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="da169-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="da169-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="da169-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="da169-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="da169-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

