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
ms.openlocfilehash: 277d4cf71c31aba26cbff6f598eaa62769cae552
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457986"
---
# <a name="suggestiondayresultarray"></a><span data-ttu-id="7af8d-103">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="7af8d-103">SuggestionDayResultArray</span></span>

<span data-ttu-id="7af8d-104">Элемент **сугжестиондайресултаррай** содержит массив предложений о собрании, организованных по дате.</span><span class="sxs-lookup"><span data-stu-id="7af8d-104">The **SuggestionDayResultArray** element contains an array of meeting suggestions organized by date.</span></span> 
  
[<span data-ttu-id="7af8d-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="7af8d-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="7af8d-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="7af8d-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
[<span data-ttu-id="7af8d-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="7af8d-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)
  
```xml
<SuggestionDayResultArray>
   <SuggestionDayResult>...</SuggestionDayResult>
</SuggestionDayResultArray>
```

 <span data-ttu-id="7af8d-108">**аррайофсугжестиондайресулт**</span><span class="sxs-lookup"><span data-stu-id="7af8d-108">**ArrayOfSuggestionDayResult**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7af8d-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7af8d-109">Attributes and elements</span></span>

<span data-ttu-id="7af8d-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7af8d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7af8d-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7af8d-111">Attributes</span></span>

<span data-ttu-id="7af8d-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7af8d-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7af8d-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7af8d-113">Child elements</span></span>

|<span data-ttu-id="7af8d-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7af8d-114">**Element**</span></span>|<span data-ttu-id="7af8d-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7af8d-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7af8d-116">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="7af8d-116">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="7af8d-117">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="7af8d-117">Represents a single day that contains suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7af8d-118">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7af8d-118">Parent elements</span></span>

|<span data-ttu-id="7af8d-119">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7af8d-119">**Element**</span></span>|<span data-ttu-id="7af8d-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7af8d-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7af8d-121">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="7af8d-121">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="7af8d-122">Содержит данные ответа и предложения для запрошенных предложений о собрании</span><span class="sxs-lookup"><span data-stu-id="7af8d-122">Contains response information and suggestion data for requested meeting suggestions</span></span>  <br/> <span data-ttu-id="7af8d-123">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="7af8d-123">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7af8d-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="7af8d-124">Remarks</span></span>

<span data-ttu-id="7af8d-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7af8d-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7af8d-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7af8d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7af8d-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7af8d-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7af8d-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7af8d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="7af8d-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="7af8d-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7af8d-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7af8d-130">Validation File</span></span>  <br/> |<span data-ttu-id="7af8d-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="7af8d-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7af8d-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7af8d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="7af8d-133">False</span><span class="sxs-lookup"><span data-stu-id="7af8d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7af8d-134">См. также</span><span class="sxs-lookup"><span data-stu-id="7af8d-134">See also</span></span>



[<span data-ttu-id="7af8d-135">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="7af8d-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="7af8d-136">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="7af8d-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="7af8d-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="7af8d-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

