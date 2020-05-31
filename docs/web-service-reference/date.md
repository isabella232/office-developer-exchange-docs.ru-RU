---
title: Дата
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Date
api_type:
- schema
ms.assetid: 2f6bc090-fff4-45b1-8d7e-8fd6e060cce2
description: Элемент Date представляет дату, которая содержит предложенное время проведения собрания.
ms.openlocfilehash: 98dc9d6c599222c819b2c9ed1bacd05758ae1655
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761969"
---
# <a name="date"></a><span data-ttu-id="85652-103">Дата</span><span class="sxs-lookup"><span data-stu-id="85652-103">Date</span></span>

<span data-ttu-id="85652-104">Элемент **Date** представляет дату, которая содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="85652-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="85652-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="85652-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="85652-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="85652-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="85652-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="85652-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="85652-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="85652-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="85652-109">Date</span><span class="sxs-lookup"><span data-stu-id="85652-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="85652-110">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="85652-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="85652-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="85652-111">Attributes and elements</span></span>

<span data-ttu-id="85652-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="85652-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85652-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="85652-113">Attributes</span></span>

<span data-ttu-id="85652-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="85652-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85652-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="85652-115">Child elements</span></span>

<span data-ttu-id="85652-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="85652-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="85652-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="85652-117">Parent elements</span></span>

|<span data-ttu-id="85652-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="85652-118">**Element**</span></span>|<span data-ttu-id="85652-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="85652-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85652-120">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="85652-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="85652-121">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="85652-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="85652-122">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="85652-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="85652-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="85652-123">Text value</span></span>

<span data-ttu-id="85652-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="85652-124">A text value is required.</span></span> <span data-ttu-id="85652-125">Изучите рекомендации консорциума типов данных схемы консорциума W3C для формата данных примитива dateTime.</span><span class="sxs-lookup"><span data-stu-id="85652-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85652-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="85652-126">Remarks</span></span>

<span data-ttu-id="85652-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="85652-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85652-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="85652-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85652-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="85652-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="85652-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="85652-130">Schema Name</span></span>  <br/> |<span data-ttu-id="85652-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="85652-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="85652-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="85652-132">Validation File</span></span>  <br/> |<span data-ttu-id="85652-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="85652-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="85652-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="85652-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="85652-135">False</span><span class="sxs-lookup"><span data-stu-id="85652-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="85652-136">См. также</span><span class="sxs-lookup"><span data-stu-id="85652-136">See also</span></span>

- [<span data-ttu-id="85652-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="85652-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="85652-138">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="85652-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="85652-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="85652-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

