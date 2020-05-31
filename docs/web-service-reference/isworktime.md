---
title: исворктиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsWorkTime
api_type:
- schema
ms.assetid: 5243dd19-3593-4a81-bb2d-90496e04cb98
description: Элемент Исворктиме указывает, встречается ли предложенное время собрания в запланированные рабочие часы.
ms.openlocfilehash: c687b29df226ebb28cdf01d3a2da62590f790924
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834135"
---
# <a name="isworktime"></a><span data-ttu-id="e8205-103">исворктиме</span><span class="sxs-lookup"><span data-stu-id="e8205-103">IsWorkTime</span></span>

<span data-ttu-id="e8205-104">Элемент **исворктиме** указывает, встречается ли предложенное время собрания в запланированные рабочие часы.</span><span class="sxs-lookup"><span data-stu-id="e8205-104">The **IsWorkTime** element represents whether the suggested meeting time occurs during scheduled work hours.</span></span> 
  
[<span data-ttu-id="e8205-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e8205-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e8205-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e8205-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="e8205-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="e8205-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="e8205-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="e8205-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="e8205-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="e8205-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="e8205-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="e8205-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="e8205-111">исворктиме</span><span class="sxs-lookup"><span data-stu-id="e8205-111">IsWorkTime</span></span>](isworktime.md)
  
```xml
<IsWorkTime>true or false</IsWorkTime>
```

 <span data-ttu-id="e8205-112">**boolean**</span><span class="sxs-lookup"><span data-stu-id="e8205-112">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8205-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8205-113">Attributes and elements</span></span>

<span data-ttu-id="e8205-114">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e8205-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8205-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8205-115">Attributes</span></span>

<span data-ttu-id="e8205-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8205-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8205-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8205-117">Child elements</span></span>

<span data-ttu-id="e8205-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8205-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8205-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8205-119">Parent elements</span></span>

|<span data-ttu-id="e8205-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8205-120">**Element**</span></span>|<span data-ttu-id="e8205-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8205-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8205-122">Предложение</span><span class="sxs-lookup"><span data-stu-id="e8205-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="e8205-123">Представляет один вариант времени собрания.</span><span class="sxs-lookup"><span data-stu-id="e8205-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="e8205-124">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e8205-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8205-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e8205-125">Text value</span></span>

<span data-ttu-id="e8205-126">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="e8205-126">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8205-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="e8205-127">Remarks</span></span>

<span data-ttu-id="e8205-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8205-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8205-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8205-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8205-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8205-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8205-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8205-131">Schema Name</span></span>  <br/> |<span data-ttu-id="e8205-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e8205-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8205-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8205-133">Validation File</span></span>  <br/> |<span data-ttu-id="e8205-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e8205-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8205-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8205-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8205-136">False</span><span class="sxs-lookup"><span data-stu-id="e8205-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8205-137">См. также</span><span class="sxs-lookup"><span data-stu-id="e8205-137">See also</span></span>



[<span data-ttu-id="e8205-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e8205-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e8205-139">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e8205-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e8205-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e8205-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

