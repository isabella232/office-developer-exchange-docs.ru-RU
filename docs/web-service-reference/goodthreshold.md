---
title: гудсрешолд
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: Элемент Гудсрешолд указывает процент участников, для которых должен быть открыт период времени, чтобы определить, какой период времени должен быть приемлемым для предполагаемого времени проведения собрания.
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833746"
---
# <a name="goodthreshold"></a><span data-ttu-id="33159-103">гудсрешолд</span><span class="sxs-lookup"><span data-stu-id="33159-103">GoodThreshold</span></span>

<span data-ttu-id="33159-104">Элемент **гудсрешолд** указывает процент участников, для которых должен быть открыт период времени, чтобы определить, какой период времени должен быть приемлемым для предполагаемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="33159-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="33159-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="33159-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="33159-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="33159-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="33159-107">гудсрешолд</span><span class="sxs-lookup"><span data-stu-id="33159-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="33159-108">**int**</span><span class="sxs-lookup"><span data-stu-id="33159-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="33159-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="33159-109">Attributes and elements</span></span>

<span data-ttu-id="33159-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="33159-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="33159-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="33159-111">Attributes</span></span>

<span data-ttu-id="33159-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="33159-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="33159-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="33159-113">Child elements</span></span>

<span data-ttu-id="33159-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="33159-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="33159-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="33159-115">Parent elements</span></span>

|<span data-ttu-id="33159-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="33159-116">**Element**</span></span>|<span data-ttu-id="33159-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="33159-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="33159-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="33159-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="33159-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="33159-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="33159-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="33159-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="33159-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="33159-121">Text value</span></span>

<span data-ttu-id="33159-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="33159-122">A text value is required.</span></span> <span data-ttu-id="33159-123">Ожидаемые целые значения находятся в диапазоне от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="33159-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="33159-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="33159-124">Remarks</span></span>

<span data-ttu-id="33159-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="33159-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="33159-126">Элемент **гудсрешолд** также определяет, что встречами считается удовлетворительно.</span><span class="sxs-lookup"><span data-stu-id="33159-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="33159-127">В процентах от участников с конфликтами меньше, чем на 50 процентов, рекомендуемое время проведения собрания определено как справедливое.</span><span class="sxs-lookup"><span data-stu-id="33159-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="33159-128">Хорошее пороговое значение плюс 50 соответствует проценту, определяющему хорошее/приемлемое пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="33159-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="33159-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="33159-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="33159-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="33159-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="33159-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="33159-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="33159-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="33159-132">Schema Name</span></span>  <br/> |<span data-ttu-id="33159-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="33159-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="33159-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="33159-134">Validation File</span></span>  <br/> |<span data-ttu-id="33159-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="33159-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="33159-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="33159-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="33159-137">False</span><span class="sxs-lookup"><span data-stu-id="33159-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="33159-138">См. также</span><span class="sxs-lookup"><span data-stu-id="33159-138">See also</span></span>



[<span data-ttu-id="33159-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="33159-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="33159-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="33159-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

