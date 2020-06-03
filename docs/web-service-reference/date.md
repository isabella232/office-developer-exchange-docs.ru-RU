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
ms.openlocfilehash: bcc152ed6aba94907189b5579b998815be45db16
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44443790"
---
# <a name="date"></a><span data-ttu-id="fa695-103">Дата</span><span class="sxs-lookup"><span data-stu-id="fa695-103">Date</span></span>

<span data-ttu-id="fa695-104">Элемент **Date** представляет дату, которая содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="fa695-104">The **Date** element represents the date that contains the suggested meeting times.</span></span> 
  
- [<span data-ttu-id="fa695-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="fa695-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) 
- [<span data-ttu-id="fa695-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="fa695-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="fa695-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="fa695-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="fa695-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="fa695-108">SuggestionDayResult</span></span>](suggestiondayresult.md)  
- [<span data-ttu-id="fa695-109">Date</span><span class="sxs-lookup"><span data-stu-id="fa695-109">Date</span></span>](date.md)
  
```xml
<Date>...</Date>
```

<span data-ttu-id="fa695-110">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="fa695-110">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fa695-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fa695-111">Attributes and elements</span></span>

<span data-ttu-id="fa695-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fa695-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa695-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fa695-113">Attributes</span></span>

<span data-ttu-id="fa695-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa695-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa695-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fa695-115">Child elements</span></span>

<span data-ttu-id="fa695-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fa695-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa695-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fa695-117">Parent elements</span></span>

|<span data-ttu-id="fa695-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fa695-118">**Element**</span></span>|<span data-ttu-id="fa695-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fa695-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa695-120">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="fa695-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="fa695-121">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="fa695-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="fa695-122">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="fa695-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa695-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="fa695-123">Text value</span></span>

<span data-ttu-id="fa695-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="fa695-124">A text value is required.</span></span> <span data-ttu-id="fa695-125">Изучите рекомендации консорциума типов данных схемы консорциума W3C для формата данных примитива dateTime.</span><span class="sxs-lookup"><span data-stu-id="fa695-125">Review the World Wide Web Consortium (W3C) schema datatype recommendations for the format of the dateTime primitive datatype.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa695-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="fa695-126">Remarks</span></span>

<span data-ttu-id="fa695-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fa695-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa695-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fa695-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa695-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fa695-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa695-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fa695-130">Schema Name</span></span>  <br/> |<span data-ttu-id="fa695-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="fa695-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa695-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fa695-132">Validation File</span></span>  <br/> |<span data-ttu-id="fa695-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="fa695-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa695-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fa695-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="fa695-135">False</span><span class="sxs-lookup"><span data-stu-id="fa695-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa695-136">См. также</span><span class="sxs-lookup"><span data-stu-id="fa695-136">See also</span></span>

- [<span data-ttu-id="fa695-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fa695-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md) 
- [<span data-ttu-id="fa695-138">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="fa695-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="fa695-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="fa695-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

