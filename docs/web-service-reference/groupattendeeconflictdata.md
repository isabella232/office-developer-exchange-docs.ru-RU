---
title: граупаттендиконфликтдата
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
description: Элемент Граупаттендиконфликтдата содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и числе пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462931"
---
# <a name="groupattendeeconflictdata"></a><span data-ttu-id="a1e3b-103">граупаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="a1e3b-103">GroupAttendeeConflictData</span></span>

<span data-ttu-id="a1e3b-104">Элемент **граупаттендиконфликтдата** содержит статистические сведения о количестве доступных пользователей, количестве пользователей с конфликтами и числе пользователей, не имеющих сведений о доступности, в списке рассылки для предполагаемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-104">The **GroupAttendeeConflictData** element contains aggregate conflict information about the number of users who are available, the number of users who have conflicts, and the number of users who do not have availability information in a distribution list for a suggested meeting time.</span></span> 
  
- [<span data-ttu-id="a1e3b-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1e3b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a1e3b-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1e3b-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
- [<span data-ttu-id="a1e3b-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="a1e3b-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
- [<span data-ttu-id="a1e3b-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="a1e3b-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
- [<span data-ttu-id="a1e3b-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="a1e3b-109">SuggestionArray</span></span>](suggestionarray.md)
- [<span data-ttu-id="a1e3b-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="a1e3b-110">Suggestion</span></span>](suggestion.md)
- [<span data-ttu-id="a1e3b-111">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="a1e3b-111">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md)
- [<span data-ttu-id="a1e3b-112">граупаттендиконфликтдата</span><span class="sxs-lookup"><span data-stu-id="a1e3b-112">GroupAttendeeConflictData</span></span>](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

<span data-ttu-id="a1e3b-113">**граупаттендиконфликтдата**</span><span class="sxs-lookup"><span data-stu-id="a1e3b-113">**GroupAttendeeConflictData**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a1e3b-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1e3b-114">Attributes and elements</span></span>

<span data-ttu-id="a1e3b-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1e3b-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1e3b-116">Attributes</span></span>

<span data-ttu-id="a1e3b-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1e3b-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1e3b-118">Child elements</span></span>

|<span data-ttu-id="a1e3b-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1e3b-119">**Element**</span></span>|<span data-ttu-id="a1e3b-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1e3b-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1e3b-121">нумберофмемберс</span><span class="sxs-lookup"><span data-stu-id="a1e3b-121">NumberOfMembers</span></span>](numberofmembers.md) <br/> |<span data-ttu-id="a1e3b-122">Представляет количество пользователей, ресурсов и комнат в списке рассылки.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-122">Represents the number of users, resources, and rooms in a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="a1e3b-123">нумберофмемберсаваилабле</span><span class="sxs-lookup"><span data-stu-id="a1e3b-123">NumberOfMembersAvailable</span></span>](numberofmembersavailable.md) <br/> |<span data-ttu-id="a1e3b-124">Представляет количество участников списка рассылки, доступных для предложенного времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-124">Represents the number of distribution list members who are available for a suggested meeting time.</span></span> <span data-ttu-id="a1e3b-125">Этот элемент представляет элементы, состояние которых **свободно**.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-125">This element represents members for whom the status is **Free**.</span></span>  <br/> |
|[<span data-ttu-id="a1e3b-126">нумберофмемберсвисконфликт</span><span class="sxs-lookup"><span data-stu-id="a1e3b-126">NumberOfMembersWithConflict</span></span>](numberofmemberswithconflict.md) <br/> |<span data-ttu-id="a1e3b-127">Представляет количество участников списка рассылки, у которых возник конфликт с предложенным временем собрания.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-127">Represents the number of distribution list members who have a conflict with a suggested meeting time.</span></span> <span data-ttu-id="a1e3b-128">Этот элемент представляет элементы со статусом " **занято**", " **отсутствие**на работе" или " **под вопросом** ".</span><span class="sxs-lookup"><span data-stu-id="a1e3b-128">This element represents members who have a **Busy**, **OOF**, or **Tentative** status.</span></span>  <br/> |
|[<span data-ttu-id="a1e3b-129">нумберофмемберсвиснодата</span><span class="sxs-lookup"><span data-stu-id="a1e3b-129">NumberOfMembersWithNoData</span></span>](numberofmemberswithnodata.md) <br/> |<span data-ttu-id="a1e3b-130">Представляет количество участников группы, у которых нет опубликованных сведений о доступности, для сравнения с предложенным временем собрания.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-130">Represents the number of group members who do not have published free/busy data to compare to a suggested meeting time.</span></span> <span data-ttu-id="a1e3b-131">Этот элемент представляет слишком большое количество элементов списка рассылки или членов, у которых нет состояния **данных** .</span><span class="sxs-lookup"><span data-stu-id="a1e3b-131">This element represents members of a distribution list that is too large or members who have **No Data** status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1e3b-132">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1e3b-132">Parent elements</span></span>

|<span data-ttu-id="a1e3b-133">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1e3b-133">**Element**</span></span>|<span data-ttu-id="a1e3b-134">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1e3b-134">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1e3b-135">аттендиконфликтдатааррай</span><span class="sxs-lookup"><span data-stu-id="a1e3b-135">AttendeeConflictDataArray</span></span>](attendeeconflictdataarray.md) <br/> |<span data-ttu-id="a1e3b-136">Содержит массив данных о конфликтах для запрашиваемых участников, идентифицированных в [операции GetUserAvailability](getuseravailability-operation.md).</span><span class="sxs-lookup"><span data-stu-id="a1e3b-136">Contains an array of conflict data for queried attendees identified in the [GetUserAvailability operation](getuseravailability-operation.md).</span></span>  <br/> <span data-ttu-id="a1e3b-137">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a1e3b-137">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1e3b-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1e3b-138">Remarks</span></span>

<span data-ttu-id="a1e3b-139">Элемент **граупаттендиконфликтдата** присутствует в отклике, когда участник в [жетусераваилабилитирекуест](getuseravailabilityrequest.md) разрешается в список рассылки.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-139">The **GroupAttendeeConflictData** element is present in the response when an attendee in the [GetUserAvailabilityRequest](getuseravailabilityrequest.md) is resolved to a distribution list.</span></span> <span data-ttu-id="a1e3b-140">Элемент **граупаттендиконфликтдата** определяет три состояния для членов списка рассылки: Available, конфликтовали или No Data.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-140">The **GroupAttendeeConflictData** element identifies three states for members of a distribution list: available, conflicted, or no data.</span></span> <span data-ttu-id="a1e3b-141">Расширение списка рассылки будет поддерживать до 100 членов.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-141">Distribution list expansion will support up to 100 members.</span></span> <span data-ttu-id="a1e3b-142">Таким образом, элемент [нумберофмемберс](numberofmembers.md) может содержать не более 100 элементов.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-142">Therefore, the [NumberOfMembers](numberofmembers.md) element can contain a maximum of 100 members.</span></span> <span data-ttu-id="a1e3b-143">Расширение списка рассылки является рекурсивным.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-143">Distribution list expansion is recursive.</span></span> <span data-ttu-id="a1e3b-144">Если список рассылки содержит дочерний список рассылки, расширяющий общее родительское членство на 100 элементов, дочерний список рассылки не будет расширен и будет считаться одной записью числа элементов [нумберофмемберсвиснодата](numberofmemberswithnodata.md) .</span><span class="sxs-lookup"><span data-stu-id="a1e3b-144">If a distribution list contains a child distribution list that expands the total parent membership to over 100 members, the child distribution list will not be expanded and will count as a single entry of the [NumberOfMembersWithNoData](numberofmemberswithnodata.md) element count.</span></span> <span data-ttu-id="a1e3b-145">Если дочерний список рассылки можно развернуть, а общее родительское членство не разворачивается до 100 элементов, его членство разворачивается, и счетчики элементов добавляются в дочерние элементы элемента **граупаттендиконфликтдата** .</span><span class="sxs-lookup"><span data-stu-id="a1e3b-145">If a child distribution list can be expanded and the total parent membership does not expand to over 100 members, its membership is expanded and the member counts are added to the child elements of the **GroupAttendeeConflictData** element.</span></span> 
  
<span data-ttu-id="a1e3b-146">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1e3b-146">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1e3b-147">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1e3b-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1e3b-148">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1e3b-148">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1e3b-149">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1e3b-149">Schema Name</span></span>  <br/> |<span data-ttu-id="a1e3b-150">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a1e3b-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1e3b-151">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1e3b-151">Validation File</span></span>  <br/> |<span data-ttu-id="a1e3b-152">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1e3b-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1e3b-153">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1e3b-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1e3b-154">False</span><span class="sxs-lookup"><span data-stu-id="a1e3b-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1e3b-155">См. также</span><span class="sxs-lookup"><span data-stu-id="a1e3b-155">See also</span></span>

- [<span data-ttu-id="a1e3b-156">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a1e3b-156">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a1e3b-157">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1e3b-157">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a1e3b-158">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a1e3b-158">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

