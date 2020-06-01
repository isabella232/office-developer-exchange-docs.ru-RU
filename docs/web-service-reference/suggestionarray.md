---
title: сугжестионаррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionArray
api_type:
- schema
ms.assetid: c1c26008-7b14-4563-8db5-bceb0f475b1b
description: Элемент Сугжестионаррай содержит массив предложений о собрании.
ms.openlocfilehash: ec982417c39569820beef82ae837eacbe316740c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466677"
---
# <a name="suggestionarray"></a><span data-ttu-id="a83ae-103">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="a83ae-103">SuggestionArray</span></span>

<span data-ttu-id="a83ae-104">Элемент **сугжестионаррай** содержит массив предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="a83ae-104">The **SuggestionArray** element contains an array of meeting suggestions.</span></span> 
  
[<span data-ttu-id="a83ae-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a83ae-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a83ae-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="a83ae-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="a83ae-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="a83ae-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="a83ae-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="a83ae-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="a83ae-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="a83ae-109">SuggestionArray</span></span>](suggestionarray.md)
  
```xml
<SuggestionArray>
   <Suggestion>...</Suggestion>
</SuggestionArray>
```

 <span data-ttu-id="a83ae-110">**аррайофсугжестион**</span><span class="sxs-lookup"><span data-stu-id="a83ae-110">**ArrayOfSuggestion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a83ae-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a83ae-111">Attributes and elements</span></span>

<span data-ttu-id="a83ae-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a83ae-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a83ae-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a83ae-113">Attributes</span></span>

<span data-ttu-id="a83ae-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a83ae-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a83ae-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a83ae-115">Child elements</span></span>

|<span data-ttu-id="a83ae-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a83ae-116">**Element**</span></span>|<span data-ttu-id="a83ae-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a83ae-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a83ae-118">Предложение</span><span class="sxs-lookup"><span data-stu-id="a83ae-118">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="a83ae-119">Представляет одно предложение собрания.</span><span class="sxs-lookup"><span data-stu-id="a83ae-119">Represents a single meeting suggestion.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a83ae-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a83ae-120">Parent elements</span></span>

|<span data-ttu-id="a83ae-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a83ae-121">**Element**</span></span>|<span data-ttu-id="a83ae-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a83ae-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a83ae-123">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="a83ae-123">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="a83ae-124">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="a83ae-124">Represents a single day that contains suggested meeting times.</span></span>  <br/> <span data-ttu-id="a83ae-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a83ae-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a83ae-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="a83ae-126">Remarks</span></span>

<span data-ttu-id="a83ae-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a83ae-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a83ae-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a83ae-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a83ae-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a83ae-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a83ae-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a83ae-130">Schema Name</span></span>  <br/> |<span data-ttu-id="a83ae-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a83ae-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a83ae-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a83ae-132">Validation File</span></span>  <br/> |<span data-ttu-id="a83ae-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a83ae-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a83ae-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a83ae-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="a83ae-135">False</span><span class="sxs-lookup"><span data-stu-id="a83ae-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a83ae-136">См. также</span><span class="sxs-lookup"><span data-stu-id="a83ae-136">See also</span></span>



[<span data-ttu-id="a83ae-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a83ae-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a83ae-138">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a83ae-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a83ae-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a83ae-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

