---
title: дайкуалити
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayQuality
api_type:
- schema
ms.assetid: cd0eb239-6e7f-4a5a-b245-659f170550b7
description: Элемент Дайкуалити представляет качество дня, в котором для качества предлагается время проведения собрания.
ms.openlocfilehash: 41cc8313dccb1a5172fefc167e6ed90a21109ec5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455116"
---
# <a name="dayquality"></a><span data-ttu-id="8ae74-103">дайкуалити</span><span class="sxs-lookup"><span data-stu-id="8ae74-103">DayQuality</span></span>

<span data-ttu-id="8ae74-104">Элемент **дайкуалити** представляет качество дня, в котором для качества предлагается время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="8ae74-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="8ae74-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="8ae74-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="8ae74-106">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="8ae74-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="8ae74-107">сугжестиондайресултаррай</span><span class="sxs-lookup"><span data-stu-id="8ae74-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="8ae74-108">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="8ae74-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="8ae74-109">дайкуалити</span><span class="sxs-lookup"><span data-stu-id="8ae74-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="8ae74-110">**сугжестионкуалити**</span><span class="sxs-lookup"><span data-stu-id="8ae74-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="8ae74-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8ae74-111">Attributes and elements</span></span>

<span data-ttu-id="8ae74-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8ae74-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8ae74-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8ae74-113">Attributes</span></span>

<span data-ttu-id="8ae74-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8ae74-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8ae74-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8ae74-115">Child elements</span></span>

<span data-ttu-id="8ae74-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8ae74-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8ae74-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8ae74-117">Parent elements</span></span>

|<span data-ttu-id="8ae74-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8ae74-118">**Element**</span></span>|<span data-ttu-id="8ae74-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8ae74-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8ae74-120">сугжестиондайресулт</span><span class="sxs-lookup"><span data-stu-id="8ae74-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="8ae74-121">Представляет один день, который содержит предложенное время проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="8ae74-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="8ae74-122">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="8ae74-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8ae74-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8ae74-123">Text value</span></span>

<span data-ttu-id="8ae74-124">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="8ae74-124">A text value is required.</span></span> <span data-ttu-id="8ae74-125">Ниже приведены возможные значения для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="8ae74-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="8ae74-126">**Отличная**</span><span class="sxs-lookup"><span data-stu-id="8ae74-126">**Excellent**</span></span>   
- <span data-ttu-id="8ae74-127">**Good**</span><span class="sxs-lookup"><span data-stu-id="8ae74-127">**Good**</span></span>    
- <span data-ttu-id="8ae74-128">**Честно**</span><span class="sxs-lookup"><span data-stu-id="8ae74-128">**Fair**</span></span>    
- <span data-ttu-id="8ae74-129">**Плохо**</span><span class="sxs-lookup"><span data-stu-id="8ae74-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="8ae74-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="8ae74-130">Remarks</span></span>

<span data-ttu-id="8ae74-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8ae74-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8ae74-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8ae74-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8ae74-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8ae74-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8ae74-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8ae74-134">Schema Name</span></span>  <br/> |<span data-ttu-id="8ae74-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="8ae74-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="8ae74-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8ae74-136">Validation File</span></span>  <br/> |<span data-ttu-id="8ae74-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="8ae74-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8ae74-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8ae74-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="8ae74-139">False</span><span class="sxs-lookup"><span data-stu-id="8ae74-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8ae74-140">См. также</span><span class="sxs-lookup"><span data-stu-id="8ae74-140">See also</span></span>

- [<span data-ttu-id="8ae74-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="8ae74-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="8ae74-142">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="8ae74-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="8ae74-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="8ae74-143">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

