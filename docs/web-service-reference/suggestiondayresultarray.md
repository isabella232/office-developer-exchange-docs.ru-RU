---
title: сугжестиондайресултаррай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionDayResultArray
api_type:
- schema
ms.assetid: eeba9eff-5eca-4002-b5a5-8fb794feaba1
description: Элемент Сугжестиондайресултаррай содержит массив предложений о собрании, организованных по дате.
ms.openlocfilehash: c208104356606a5d9961461ad8743a772d2410d8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840113"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="6b02a-103">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="6b02a-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="6b02a-104">Элемент **сугжестиондайресултаррай** содержит массив предложений о собрании, организованных по дате.</span><span class="sxs-lookup"><span data-stu-id="6b02a-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="6b02a-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b02a-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="6b02a-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b02a-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="6b02a-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="6b02a-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="6b02a-108">**аррайофсугжестиондайресулт**</span><span class="sxs-lookup"><span data-stu-id="6b02a-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b02a-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6b02a-109">Attributes and elements</span></span>

<span data-ttu-id="6b02a-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6b02a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b02a-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6b02a-111">Attributes</span></span>

<span data-ttu-id="6b02a-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="6b02a-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b02a-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6b02a-113">Child elements</span></span>

|<span data-ttu-id="6b02a-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b02a-114">**Element**</span></span>|<span data-ttu-id="6b02a-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b02a-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b02a-116">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="6b02a-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="6b02a-117">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="6b02a-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6b02a-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6b02a-118">Parent elements</span></span>

|<span data-ttu-id="6b02a-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b02a-119">**Element**</span></span>|<span data-ttu-id="6b02a-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b02a-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b02a-121">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b02a-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="6b02a-122">Содержит данные ответа и предложения для запрошенных предложений о собрании</span><span class="sxs-lookup"><span data-stu-id="6b02a-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="6b02a-123">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="6b02a-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6b02a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="6b02a-124">Remarks</span></span>

<span data-ttu-id="6b02a-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6b02a-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b02a-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6b02a-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b02a-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6b02a-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b02a-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6b02a-128">Schema Name</span></span>  <br/> |<span data-ttu-id="6b02a-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="6b02a-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b02a-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6b02a-130">Validation File</span></span>  <br/> |<span data-ttu-id="6b02a-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="6b02a-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b02a-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6b02a-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b02a-133">False</span><span class="sxs-lookup"><span data-stu-id="6b02a-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b02a-134">См. также</span><span class="sxs-lookup"><span data-stu-id="6b02a-134">See also</span></span>



[<span data-ttu-id="6b02a-135">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="6b02a-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="6b02a-136">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="6b02a-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="6b02a-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="6b02a-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

