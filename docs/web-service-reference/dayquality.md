---
title: DayQuality
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
description: Элемент DayQuality представляет качества день, содержащий раз качества предложенного собрания.
ms.openlocfilehash: 156d5bc58d481c9c812793da4722272ac76adaad
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762001"
---
# <a name="dayquality"></a><span data-ttu-id="a4925-103">DayQuality</span><span class="sxs-lookup"><span data-stu-id="a4925-103">DayQuality</span></span>

<span data-ttu-id="a4925-104">Элемент **DayQuality** представляет качества день, содержащий качество, предлагаемое время собрания.</span><span class="sxs-lookup"><span data-stu-id="a4925-104">The **DayQuality** element represents the quality of the day for containing quality suggested meeting times.</span></span> 
  
- [<span data-ttu-id="a4925-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a4925-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)  
- [<span data-ttu-id="a4925-106">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="a4925-106">SuggestionsResponse</span></span>](suggestionsresponse.md) 
- [<span data-ttu-id="a4925-107">SuggestionDayResultArray</span><span class="sxs-lookup"><span data-stu-id="a4925-107">SuggestionDayResultArray</span></span>](suggestiondayresultarray.md)  
- [<span data-ttu-id="a4925-108">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a4925-108">SuggestionDayResult</span></span>](suggestiondayresult.md) 
- [<span data-ttu-id="a4925-109">DayQuality</span><span class="sxs-lookup"><span data-stu-id="a4925-109">DayQuality</span></span>](dayquality.md)
  
```xml
<DayQuality>Excellent or Good or Fair or Poor</DayQuality>
```

<span data-ttu-id="a4925-110">**SuggestionQuality**</span><span class="sxs-lookup"><span data-stu-id="a4925-110">**SuggestionQuality**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a4925-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a4925-111">Attributes and elements</span></span>

<span data-ttu-id="a4925-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a4925-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4925-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a4925-113">Attributes</span></span>

<span data-ttu-id="a4925-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4925-114">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4925-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a4925-115">Child elements</span></span>

<span data-ttu-id="a4925-116">Нет.</span><span class="sxs-lookup"><span data-stu-id="a4925-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a4925-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a4925-117">Parent elements</span></span>

|<span data-ttu-id="a4925-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a4925-118">**Element**</span></span>|<span data-ttu-id="a4925-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a4925-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4925-120">SuggestionDayResult</span><span class="sxs-lookup"><span data-stu-id="a4925-120">SuggestionDayResult</span></span>](suggestiondayresult.md) <br/> |<span data-ttu-id="a4925-121">Представляет один день, который содержит время предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="a4925-121">Represents a single day that contains suggested meeting times.</span></span>  <br/><br/><span data-ttu-id="a4925-122">Ниже приведен выражение XPath 2.0 для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a4925-122">The following is the XPath 2.0 expression to this element:</span></span><br/><br/>`/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a4925-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a4925-123">Text value</span></span>

<span data-ttu-id="a4925-124">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a4925-124">A text value is required.</span></span> <span data-ttu-id="a4925-125">Ниже приведены возможные значения для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a4925-125">The following are the possible values for this element:</span></span>
  
- <span data-ttu-id="a4925-126">**Отлично**</span><span class="sxs-lookup"><span data-stu-id="a4925-126">**Excellent**</span></span>   
- <span data-ttu-id="a4925-127">**Хороший**</span><span class="sxs-lookup"><span data-stu-id="a4925-127">**Good**</span></span>    
- <span data-ttu-id="a4925-128">**Обычное**</span><span class="sxs-lookup"><span data-stu-id="a4925-128">**Fair**</span></span>    
- <span data-ttu-id="a4925-129">**Низкий**</span><span class="sxs-lookup"><span data-stu-id="a4925-129">**Poor**</span></span>
    
## <a name="remarks"></a><span data-ttu-id="a4925-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="a4925-130">Remarks</span></span>

<span data-ttu-id="a4925-131">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a4925-131">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4925-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a4925-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4925-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a4925-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a4925-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a4925-134">Schema Name</span></span>  <br/> |<span data-ttu-id="a4925-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a4925-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="a4925-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a4925-136">Validation File</span></span>  <br/> |<span data-ttu-id="a4925-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a4925-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a4925-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a4925-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="a4925-139">False</span><span class="sxs-lookup"><span data-stu-id="a4925-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4925-140">См. также</span><span class="sxs-lookup"><span data-stu-id="a4925-140">See also</span></span>

- [<span data-ttu-id="a4925-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a4925-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="a4925-142">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a4925-142">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="a4925-143">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a4925-143">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

