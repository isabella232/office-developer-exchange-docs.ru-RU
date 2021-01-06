---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: Элемент SuggestionsViewOptions содержит параметры для получения сведений о предложении собрания.
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44433996"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="da3f7-103">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="da3f7-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="da3f7-104">Элемент **SuggestionsViewOptions** содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="da3f7-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="da3f7-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="da3f7-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="da3f7-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="da3f7-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 <span data-ttu-id="da3f7-107">**SuggestionsViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="da3f7-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da3f7-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da3f7-108">Attributes and elements</span></span>

<span data-ttu-id="da3f7-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="da3f7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da3f7-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da3f7-110">Attributes</span></span>

<span data-ttu-id="da3f7-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="da3f7-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da3f7-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da3f7-112">Child elements</span></span>

|<span data-ttu-id="da3f7-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da3f7-113">**Element**</span></span>|<span data-ttu-id="da3f7-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da3f7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da3f7-115">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="da3f7-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="da3f7-116">Указывает процент участников, которые должны иметь период времени, открытый для периода времени, чтобы квалифицироваться как рекомендуемый период собрания.</span><span class="sxs-lookup"><span data-stu-id="da3f7-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-117">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="da3f7-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="da3f7-118">Указывает число рекомендуемого времени собрания в день, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="da3f7-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-119">MaximumNonWorkHourResultsByDay</span><span class="sxs-lookup"><span data-stu-id="da3f7-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="da3f7-120">Указывает количество предлагаемых результатов для времени собрания вне обычного рабочего времени в день.</span><span class="sxs-lookup"><span data-stu-id="da3f7-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-121">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="da3f7-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="da3f7-122">Указывает длительность предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="da3f7-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-123">MinimumSuggestionQuality</span><span class="sxs-lookup"><span data-stu-id="da3f7-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="da3f7-124">Указывает качество предложений собрания, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="da3f7-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-125">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="da3f7-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="da3f7-126">Определяет промежуток времени, в течение который запрашивается подробная информация о рекомендуемом времени собрания.</span><span class="sxs-lookup"><span data-stu-id="da3f7-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-127">CurrentMeetingTime</span><span class="sxs-lookup"><span data-stu-id="da3f7-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="da3f7-128">Представляет время начала собрания, которое вы хотите обновить с помощью предложенных результатов.</span><span class="sxs-lookup"><span data-stu-id="da3f7-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="da3f7-129">GlobalObjectId</span><span class="sxs-lookup"><span data-stu-id="da3f7-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="da3f7-130">Этот элемент не используется.</span><span class="sxs-lookup"><span data-stu-id="da3f7-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="da3f7-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da3f7-131">Parent elements</span></span>

|<span data-ttu-id="da3f7-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da3f7-132">**Element**</span></span>|<span data-ttu-id="da3f7-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da3f7-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da3f7-134">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="da3f7-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="da3f7-135">Содержит аргументы, используемые для получения сведений о доступности пользователей.</span><span class="sxs-lookup"><span data-stu-id="da3f7-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="da3f7-136">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="da3f7-136">This is a root element.</span></span>  <br/> <span data-ttu-id="da3f7-137">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="da3f7-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="da3f7-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="da3f7-138">Remarks</span></span>

<span data-ttu-id="da3f7-139">Этот элемент не требуется и может возникать только один раз, если он используется.</span><span class="sxs-lookup"><span data-stu-id="da3f7-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="da3f7-140">Это значение может иметь значение null, если значение элемента [FreeBusyViewOptions](freebusyviewoptions.md) не null.</span><span class="sxs-lookup"><span data-stu-id="da3f7-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="da3f7-141">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="da3f7-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="da3f7-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da3f7-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da3f7-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da3f7-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da3f7-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da3f7-144">Schema Name</span></span>  <br/> |<span data-ttu-id="da3f7-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da3f7-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="da3f7-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da3f7-146">Validation File</span></span>  <br/> |<span data-ttu-id="da3f7-147">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="da3f7-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da3f7-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da3f7-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="da3f7-149">False</span><span class="sxs-lookup"><span data-stu-id="da3f7-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da3f7-150">См. также</span><span class="sxs-lookup"><span data-stu-id="da3f7-150">See also</span></span>



[<span data-ttu-id="da3f7-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="da3f7-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="da3f7-152">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="da3f7-152">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

