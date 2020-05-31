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
ms.openlocfilehash: 7b75258a9e70f1ec6feed6a0b18beb76f356c7f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840111"
---
# <a name="suggestiondayresult"></a><span data-ttu-id="0b240-103">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="0b240-103">SuggestionDayResult</span></span>

<span data-ttu-id="0b240-104">Элемент **сугжестиондайресулт** представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="0b240-104">The **SuggestionDayResult** element represents a single day that contains suggested meeting times.</span></span> 
  
[<span data-ttu-id="0b240-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="0b240-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="0b240-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="0b240-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="0b240-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="0b240-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="0b240-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="0b240-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
```xml
<SuggestionDayResult>
   <Date>...</Date>
   <DayQuality>...</DayQuality>
   <SuggestionArray>...</SuggestionArray>
</SuggestionDayResult>
```

 <span data-ttu-id="0b240-109">**сугжестиондайресулт**</span><span class="sxs-lookup"><span data-stu-id="0b240-109">**SuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0b240-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0b240-110">Attributes and elements</span></span>

<span data-ttu-id="0b240-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0b240-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0b240-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0b240-112">Attributes</span></span>

<span data-ttu-id="0b240-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="0b240-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0b240-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0b240-114">Child elements</span></span>

|<span data-ttu-id="0b240-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b240-115">**Element**</span></span>|<span data-ttu-id="0b240-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b240-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b240-117">Date</span><span class="sxs-lookup"><span data-stu-id="0b240-117">Date</span></span>](date.md) <br/> |<span data-ttu-id="0b240-118">Представляет дату, которая содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="0b240-118">Represents the date that contains the suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="0b240-119">дайкуалити</span><span class="sxs-lookup"><span data-stu-id="0b240-119">DayQuality</span></span>](dayquality.md) <br/> |<span data-ttu-id="0b240-120">Представляет качество дня, в течение которого предлагается время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="0b240-120">Represents the quality of the day for containing quality suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="0b240-121">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="0b240-121">SuggestionArray</span></span>](suggestionarray.md) <br/> |<span data-ttu-id="0b240-122">Содержит массив предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="0b240-122">Contains an array of meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0b240-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0b240-123">Parent elements</span></span>

|<span data-ttu-id="0b240-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0b240-124">**Element**</span></span>|<span data-ttu-id="0b240-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0b240-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0b240-126">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="0b240-126">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="0b240-127">Содержит массив предложений собраний, организованных по дате.</span><span class="sxs-lookup"><span data-stu-id="0b240-127">Contains an array of meeting suggestions organized by date.</span></span>  <br/> <span data-ttu-id="0b240-128">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="0b240-128">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0b240-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="0b240-129">Remarks</span></span>

<span data-ttu-id="0b240-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="0b240-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0b240-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0b240-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0b240-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0b240-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0b240-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0b240-133">Schema Name</span></span>  <br/> |<span data-ttu-id="0b240-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0b240-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="0b240-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0b240-135">Validation File</span></span>  <br/> |<span data-ttu-id="0b240-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0b240-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0b240-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0b240-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="0b240-138">False</span><span class="sxs-lookup"><span data-stu-id="0b240-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0b240-139">См. также</span><span class="sxs-lookup"><span data-stu-id="0b240-139">See also</span></span>



[<span data-ttu-id="0b240-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="0b240-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="0b240-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="0b240-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="0b240-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="0b240-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

