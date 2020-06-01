---
title: сугжестиондайресулт
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResult
api_type:
- schema
ms.assetid: 916b1cbb-f2e3-471d-84b0-e33467616652
description: Элемент Сугжестиондайресулт представляет один день, который содержит предложенное время проведения собрания.
ms.openlocfilehash: af907b62acefb4913814907722b98d326bd0535b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457993"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="ac25f-103">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="ac25f-103">SuggestionDayResult</span></span>

<span data-ttu-id="ac25f-104">Элемент **сугжестиондайресулт** представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ac25f-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="ac25f-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ac25f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ac25f-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="ac25f-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="ac25f-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="ac25f-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="ac25f-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="ac25f-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="ac25f-109">**сугжестиондайресулт**</span><span class="sxs-lookup"><span data-stu-id="ac25f-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ac25f-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ac25f-110">Attributes and elements</span></span>

<span data-ttu-id="ac25f-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ac25f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ac25f-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ac25f-112">Attributes</span></span>

<span data-ttu-id="ac25f-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ac25f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ac25f-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ac25f-114">Child elements</span></span>

|<span data-ttu-id="ac25f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ac25f-115">**Element**</span></span>|<span data-ttu-id="ac25f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ac25f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac25f-117">Date</span><span class="sxs-lookup"><span data-stu-id="ac25f-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="ac25f-118">Представляет дату, которая содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ac25f-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="ac25f-119">дайкуалити</span><span class="sxs-lookup"><span data-stu-id="ac25f-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="ac25f-120">Представляет качество дня, в течение которого предлагается время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="ac25f-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="ac25f-121">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="ac25f-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="ac25f-122">Содержит массив предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="ac25f-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ac25f-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ac25f-123">Parent elements</span></span>

|<span data-ttu-id="ac25f-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ac25f-124">**Element**</span></span>|<span data-ttu-id="ac25f-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ac25f-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ac25f-126">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="ac25f-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="ac25f-127">Содержит массив предложений собраний, организованных по дате.</span><span class="sxs-lookup"><span data-stu-id="ac25f-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="ac25f-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ac25f-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ac25f-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="ac25f-129">Remarks</span></span>

<span data-ttu-id="ac25f-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ac25f-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ac25f-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ac25f-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ac25f-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ac25f-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ac25f-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ac25f-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ac25f-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ac25f-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ac25f-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ac25f-135">Validation File</span></span>  <br/> |<span data-ttu-id="ac25f-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ac25f-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ac25f-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ac25f-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ac25f-138">False</span><span class="sxs-lookup"><span data-stu-id="ac25f-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ac25f-139">См. также</span><span class="sxs-lookup"><span data-stu-id="ac25f-139">See also</span></span>



[<span data-ttu-id="ac25f-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ac25f-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ac25f-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ac25f-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ac25f-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="ac25f-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

