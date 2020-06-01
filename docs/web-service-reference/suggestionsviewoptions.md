---
title: сугжестионсвиевоптионс
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
description: Элемент Сугжестионсвиевоптионс содержит параметры для получения сведений о предложении о собрании.
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433996"
---
# <a name="suggestionsviewoptions"></a><span data-ttu-id="b4fe5-103">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="b4fe5-103">SuggestionsViewOptions</span></span>

<span data-ttu-id="b4fe5-104">Элемент **сугжестионсвиевоптионс** содержит параметры для получения сведений о предложении о собрании.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-104">The **SuggestionsViewOptions** element contains the options for obtaining meeting suggestion information.</span></span> 
  
[<span data-ttu-id="b4fe5-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="b4fe5-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="b4fe5-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="b4fe5-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
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

 <span data-ttu-id="b4fe5-107">**сугжестионсвиевоптионстипе**</span><span class="sxs-lookup"><span data-stu-id="b4fe5-107">**SuggestionsViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b4fe5-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b4fe5-108">Attributes and elements</span></span>

<span data-ttu-id="b4fe5-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b4fe5-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b4fe5-110">Attributes</span></span>

<span data-ttu-id="b4fe5-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b4fe5-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b4fe5-112">Child elements</span></span>

|<span data-ttu-id="b4fe5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b4fe5-113">**Element**</span></span>|<span data-ttu-id="b4fe5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4fe5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4fe5-115">гудсрешолд</span><span class="sxs-lookup"><span data-stu-id="b4fe5-115">GoodThreshold</span></span>](goodthreshold.md) <br/> |<span data-ttu-id="b4fe5-116">Указывает процент участников, которые должны иметь период времени, который должен быть указан в качестве приемлемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-116">Specifies the percentage of attendees that must have the time period open for the time period to qualify as a good suggested meeting time.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-117">максимумресултсбидай</span><span class="sxs-lookup"><span data-stu-id="b4fe5-117">MaximumResultsByDay</span></span>](maximumresultsbyday.md) <br/> |<span data-ttu-id="b4fe5-118">Указывает количество предложенных собраний в день, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-118">Specifies the number of suggested meeting times per day returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-119">максимумнонворкхаурресултсбидай</span><span class="sxs-lookup"><span data-stu-id="b4fe5-119">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md) <br/> |<span data-ttu-id="b4fe5-120">Указывает количество предполагаемых результатов для времени проведения собрания, не входящих в число обычных рабочих часов в день.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-120">Specifies the number of suggested results for meeting times outside regular working hours per day.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-121">митингдуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="b4fe5-121">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md) <br/> |<span data-ttu-id="b4fe5-122">Указывает предполагаемую длину собрания.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-122">Specifies the length of the meeting to be suggested.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-123">минимумсугжестионкуалити</span><span class="sxs-lookup"><span data-stu-id="b4fe5-123">MinimumSuggestionQuality</span></span>](minimumsuggestionquality.md) <br/> |<span data-ttu-id="b4fe5-124">Указывает качество предложений собраний, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-124">Specifies the quality of meeting suggestions to be returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-125">детаиледсугжестионсвиндов</span><span class="sxs-lookup"><span data-stu-id="b4fe5-125">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="b4fe5-126">Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-126">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-127">куррентмитингтиме</span><span class="sxs-lookup"><span data-stu-id="b4fe5-127">CurrentMeetingTime</span></span>](currentmeetingtime.md) <br/> |<span data-ttu-id="b4fe5-128">Представляет время начала собрания, которое вы хотите обновить с учетом предложенного времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-128">Represents the start time of a meeting that you want to update with the suggested meeting time results.</span></span>  <br/> |
|[<span data-ttu-id="b4fe5-129">глобалобжектид</span><span class="sxs-lookup"><span data-stu-id="b4fe5-129">GlobalObjectId</span></span>](globalobjectid.md) <br/> |<span data-ttu-id="b4fe5-130">Этот элемент не используется.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-130">This element is not used.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b4fe5-131">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b4fe5-131">Parent elements</span></span>

|<span data-ttu-id="b4fe5-132">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b4fe5-132">**Element**</span></span>|<span data-ttu-id="b4fe5-133">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b4fe5-133">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b4fe5-134">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="b4fe5-134">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="b4fe5-135">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-135">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="b4fe5-136">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-136">This is a root element.</span></span>  <br/> <span data-ttu-id="b4fe5-137">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="b4fe5-137">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b4fe5-138">Примечания</span><span class="sxs-lookup"><span data-stu-id="b4fe5-138">Remarks</span></span>

<span data-ttu-id="b4fe5-139">Этот элемент не является обязательным и может быть использован только один раз.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-139">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="b4fe5-140">Это значение может быть равно null, если значение элемента [фрибусивиевоптионс](freebusyviewoptions.md) отлично от NULL.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-140">This value can be null if the value of the [FreeBusyViewOptions](freebusyviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b4fe5-141">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b4fe5-141">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b4fe5-142">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b4fe5-142">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b4fe5-143">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b4fe5-143">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b4fe5-144">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b4fe5-144">Schema Name</span></span>  <br/> |<span data-ttu-id="b4fe5-145">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b4fe5-145">Types schema</span></span>  <br/> |
|<span data-ttu-id="b4fe5-146">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b4fe5-146">Validation File</span></span>  <br/> |<span data-ttu-id="b4fe5-147">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b4fe5-147">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b4fe5-148">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b4fe5-148">Can be Empty</span></span>  <br/> |<span data-ttu-id="b4fe5-149">False</span><span class="sxs-lookup"><span data-stu-id="b4fe5-149">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b4fe5-150">См. также</span><span class="sxs-lookup"><span data-stu-id="b4fe5-150">See also</span></span>



[<span data-ttu-id="b4fe5-151">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b4fe5-151">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="b4fe5-152">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b4fe5-152">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

