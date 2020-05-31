---
title: сугжестионсреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsResponse
api_type:
- schema
ms.assetid: d25ca143-f80c-4458-b669-346fda29a5a7
description: Элемент Сугжестионсреспонсе содержит сведения о состоянии ответа и данные предложения для запрошенных предложений о собрании.
ms.openlocfilehash: 614b58a1df8e340c6be468ccddd3b37537d32591
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840114"
---
# <a name="suggestionsresponse"></a><span data-ttu-id="e505f-103">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e505f-103">SuggestionsResponse</span></span>

<span data-ttu-id="e505f-104">Элемент **сугжестионсреспонсе** содержит сведения о состоянии ответа и данные предложения для запрошенных предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="e505f-104">The **SuggestionsResponse** element contains response status information and suggestion data for requested meeting suggestions.</span></span> 
  
[<span data-ttu-id="e505f-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e505f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="e505f-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="e505f-106">SuggestionsResponse</span></span>](suggestionsresponse.md)
  
```xml
<SuggestionsResponse>
   <ResponseMessage>...</ResponseMessage>
   <SuggestionDayResultArray>...</SuggestionDayResultArray>
</SuggestionsResponse>
```

 <span data-ttu-id="e505f-107">**сугжестионсреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="e505f-107">**SuggestionsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e505f-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e505f-108">Attributes and elements</span></span>

<span data-ttu-id="e505f-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e505f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e505f-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e505f-110">Attributes</span></span>

<span data-ttu-id="e505f-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="e505f-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e505f-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e505f-112">Child elements</span></span>

|<span data-ttu-id="e505f-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e505f-113">**Element**</span></span>|<span data-ttu-id="e505f-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e505f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e505f-115">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="e505f-115">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="e505f-116">Предоставляет описательные сведения о состоянии отклика.</span><span class="sxs-lookup"><span data-stu-id="e505f-116">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="e505f-117">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="e505f-117">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md) <br/> |<span data-ttu-id="e505f-118">Содержит массив предложений собраний, организованных по дате.</span><span class="sxs-lookup"><span data-stu-id="e505f-118">Contains an array of meeting suggestions organized by date.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e505f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e505f-119">Parent elements</span></span>

|<span data-ttu-id="e505f-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e505f-120">**Element**</span></span>|<span data-ttu-id="e505f-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e505f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e505f-122">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e505f-122">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="e505f-123">Содержит сведения о доступности запрошенных пользователей.</span><span class="sxs-lookup"><span data-stu-id="e505f-123">Contains the requested users' availability information.</span></span>  <br/> <span data-ttu-id="e505f-124">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e505f-124">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e505f-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="e505f-125">Remarks</span></span>

<span data-ttu-id="e505f-126">Этот элемент не включается в ответ GetUserAvailability, если [сугжестионсвиевоптионс](suggestionsviewoptions.md) не задан в сообщении запроса GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="e505f-126">This element is not included in a GetUserAvailability response if [SuggestionsViewOptions](suggestionsviewoptions.md) is not set in the GetUserAvailability request message.</span></span> 
  
<span data-ttu-id="e505f-127">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e505f-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e505f-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e505f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e505f-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e505f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e505f-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e505f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="e505f-131">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="e505f-131">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e505f-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e505f-132">Validation File</span></span>  <br/> |<span data-ttu-id="e505f-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="e505f-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e505f-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e505f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="e505f-135">False</span><span class="sxs-lookup"><span data-stu-id="e505f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e505f-136">См. также</span><span class="sxs-lookup"><span data-stu-id="e505f-136">See also</span></span>



[<span data-ttu-id="e505f-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e505f-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="e505f-138">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="e505f-138">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="e505f-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e505f-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

