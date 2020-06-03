---
title: митингтиме
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingTime
api_type:
- schema
ms.assetid: 6e6d2d8b-e8a2-43e6-a715-0fc7d6dd44b9
description: Элемент Митингтиме представляет предполагаемое время проведения собрания.
ms.openlocfilehash: 3a7031e70eb8b22adc8030c1cec09d33399332ee
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530452"
---
# <a name="meetingtime"></a><span data-ttu-id="54aaf-103">митингтиме</span><span class="sxs-lookup"><span data-stu-id="54aaf-103">MeetingTime</span></span>

<span data-ttu-id="54aaf-104">Элемент **митингтиме** представляет предполагаемое время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="54aaf-104">The **MeetingTime** element represents a suggested meeting time.</span></span> 
  
[<span data-ttu-id="54aaf-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="54aaf-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="54aaf-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="54aaf-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="54aaf-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="54aaf-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
[<span data-ttu-id="54aaf-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="54aaf-108">SuggestionDayResult</span></span>](suggestiondayresult.md)
  
[<span data-ttu-id="54aaf-109">сугжестионаррай</span><span class="sxs-lookup"><span data-stu-id="54aaf-109">SuggestionArray</span></span>](suggestionarray.md)
  
[<span data-ttu-id="54aaf-110">Предложение</span><span class="sxs-lookup"><span data-stu-id="54aaf-110">Suggestion</span></span>](suggestion.md)
  
[<span data-ttu-id="54aaf-111">митингтиме</span><span class="sxs-lookup"><span data-stu-id="54aaf-111">MeetingTime</span></span>](meetingtime.md)
  
```xml
<MeetingTime>...</MeetingTime
```

 <span data-ttu-id="54aaf-112">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="54aaf-112">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="54aaf-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="54aaf-113">Attributes and elements</span></span>

<span data-ttu-id="54aaf-114">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="54aaf-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="54aaf-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="54aaf-115">Attributes</span></span>

<span data-ttu-id="54aaf-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54aaf-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="54aaf-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="54aaf-117">Child elements</span></span>

<span data-ttu-id="54aaf-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="54aaf-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="54aaf-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="54aaf-119">Parent elements</span></span>

|<span data-ttu-id="54aaf-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="54aaf-120">**Element**</span></span>|<span data-ttu-id="54aaf-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="54aaf-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="54aaf-122">Предложение</span><span class="sxs-lookup"><span data-stu-id="54aaf-122">Suggestion</span></span>](suggestion.md) <br/> |<span data-ttu-id="54aaf-123">Представляет один вариант времени собрания.</span><span class="sxs-lookup"><span data-stu-id="54aaf-123">Represents a single meeting time suggestion.</span></span>  <br/> <span data-ttu-id="54aaf-124">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="54aaf-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="54aaf-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="54aaf-125">Text value</span></span>

<span data-ttu-id="54aaf-126">Необходимо указать текстовое значение, представляющее значение **DateTime** .</span><span class="sxs-lookup"><span data-stu-id="54aaf-126">A text value that represents a **dateTime** value is required.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="54aaf-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="54aaf-127">Remarks</span></span>

<span data-ttu-id="54aaf-128">Элемент [митингтиме](meetingtime.md) является обязательным дочерним элементом элемента [предложения](suggestion.md) .</span><span class="sxs-lookup"><span data-stu-id="54aaf-128">The [MeetingTime](meetingtime.md) element is a required child element of the [Suggestion](suggestion.md) element.</span></span> 
  
<span data-ttu-id="54aaf-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="54aaf-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="54aaf-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="54aaf-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="54aaf-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="54aaf-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="54aaf-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="54aaf-132">Schema Name</span></span>  <br/> |<span data-ttu-id="54aaf-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="54aaf-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="54aaf-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="54aaf-134">Validation File</span></span>  <br/> |<span data-ttu-id="54aaf-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="54aaf-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="54aaf-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="54aaf-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="54aaf-137">False</span><span class="sxs-lookup"><span data-stu-id="54aaf-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="54aaf-138">См. также</span><span class="sxs-lookup"><span data-stu-id="54aaf-138">See also</span></span>



[<span data-ttu-id="54aaf-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="54aaf-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="54aaf-140">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="54aaf-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="54aaf-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="54aaf-141">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

