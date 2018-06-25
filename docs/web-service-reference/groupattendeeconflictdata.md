---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: Элемент GroupAttendeeConflictData содержит конфликта статистические сведения о количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в рассылки списка для Предлагаемое время собрания.
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833757"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="c2dea-103">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c2dea-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="c2dea-104">Элемент **GroupAttendeeConflictData** содержит конфликта статистические сведения о количество пользователей, которые доступны, количество пользователей, конфликтов и количество пользователей, у которых нет сведений о доступности в список рассылки для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="c2dea-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="c2dea-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c2dea-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="c2dea-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="c2dea-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="c2dea-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="c2dea-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="c2dea-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="c2dea-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="c2dea-109">SuggestionArray</span><span class="sxs-lookup"><span data-stu-id="c2dea-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="c2dea-110">Предложения</span><span class="sxs-lookup"><span data-stu-id="c2dea-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="c2dea-111">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c2dea-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="c2dea-112">GroupAttendeeConflictData</span><span class="sxs-lookup"><span data-stu-id="c2dea-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="c2dea-113">**GroupAttendeeConflictData**</span><span class="sxs-lookup"><span data-stu-id="c2dea-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c2dea-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c2dea-114">Attributes and elements</span></span>

<span data-ttu-id="c2dea-115">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dea-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2dea-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c2dea-116">Attributes</span></span>

<span data-ttu-id="c2dea-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="c2dea-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c2dea-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c2dea-118">Child elements</span></span>

|<span data-ttu-id="c2dea-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2dea-119">**Element**</span></span>|<span data-ttu-id="c2dea-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2dea-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2dea-121">NumberOfMembers</span><span class="sxs-lookup"><span data-stu-id="c2dea-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="c2dea-122">Представляет число пользователей, ресурсов и помещения в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="c2dea-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="c2dea-123">NumberOfMembersAvailable</span><span class="sxs-lookup"><span data-stu-id="c2dea-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="c2dea-124">Представляет число членов списка рассылки, которые доступны для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="c2dea-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="c2dea-125">Этот элемент представляет элементы, для которых состояние — **бесплатными**.</span><span class="sxs-lookup"><span data-stu-id="c2dea-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="c2dea-126">NumberOfMembersWithConflict</span><span class="sxs-lookup"><span data-stu-id="c2dea-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="c2dea-127">Представляет число членов списка рассылки, конфликт с временем предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="c2dea-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="c2dea-128">Этот элемент представляет работников, которые имеют состояние **«занят»**, **об отсутствии на работе**или **под вопросом** .</span><span class="sxs-lookup"><span data-stu-id="c2dea-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="c2dea-129">NumberOfMembersWithNoData</span><span class="sxs-lookup"><span data-stu-id="c2dea-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="c2dea-130">Представляет число членов группы, у которых нет опубликованных данных о доступности для сравнения для предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="c2dea-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="c2dea-131">Этот элемент представляет членов списка рассылки слишком большого размера или участники, которые имеют состояние **Нет данных** .</span><span class="sxs-lookup"><span data-stu-id="c2dea-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2dea-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c2dea-132">Parent elements</span></span>

|<span data-ttu-id="c2dea-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c2dea-133">**Element**</span></span>|<span data-ttu-id="c2dea-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c2dea-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2dea-135">AttendeeConflictDataArray</span><span class="sxs-lookup"><span data-stu-id="c2dea-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="c2dea-136">Содержит массив данных конфликта запрашиваемого участников, определенный в [операция GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="c2dea-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="c2dea-137">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="c2dea-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c2dea-138">Замечания</span><span class="sxs-lookup"><span data-stu-id="c2dea-138">Remarks</span></span>

<span data-ttu-id="c2dea-139">Элемент **GroupAttendeeConflictData** присутствует в ответе, когда участник в [GetUserAvailabilityRequest](getuseravailabilityrequest.md) разрешена в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="c2dea-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="c2dea-140">Элемент **GroupAttendeeConflictData** определяет три состояния для членов списка рассылки: доступны, конфликта, или без данных.</span><span class="sxs-lookup"><span data-stu-id="c2dea-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="c2dea-141">Раскрытие списка рассылки будет поддерживает до 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dea-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="c2dea-142">Таким образом элемент [NumberOfMembers](numberofmembers.md) может содержать не более 100 участников.</span><span class="sxs-lookup"><span data-stu-id="c2dea-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="c2dea-143">Раскрытие списка рассылки — это рекурсивный.</span><span class="sxs-lookup"><span data-stu-id="c2dea-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="c2dea-144">Если список рассылки содержит список рассылки дочерним, которая расширяет членства общий родительский более 100 членов, списка рассылки дочерним не развернуто и будет считаться одной операции из [NumberOfMembersWithNoData](numberofmemberswithnodata.md) счетчик элементов.</span><span class="sxs-lookup"><span data-stu-id="c2dea-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="c2dea-145">Если членства общий родительский не разворачивается до более 100 членов списка рассылки дочерним могут быть развернуты, принадлежность развертывается, и число элементов добавляются дочерние элементы элемента **GroupAttendeeConflictData** .</span><span class="sxs-lookup"><span data-stu-id="c2dea-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="c2dea-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c2dea-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2dea-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c2dea-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2dea-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c2dea-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c2dea-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c2dea-149">Schema Name</span></span>  <br/> |<span data-ttu-id="c2dea-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c2dea-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="c2dea-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c2dea-151">Validation File</span></span>  <br/> |<span data-ttu-id="c2dea-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c2dea-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c2dea-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c2dea-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2dea-154">False</span><span class="sxs-lookup"><span data-stu-id="c2dea-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2dea-155">См. также</span><span class="sxs-lookup"><span data-stu-id="c2dea-155">See also</span></span>

- [<span data-ttu-id="c2dea-156">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c2dea-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c2dea-157">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="c2dea-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="c2dea-158">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="c2dea-158">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

