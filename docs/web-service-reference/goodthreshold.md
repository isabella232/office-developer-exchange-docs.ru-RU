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
ms.openlocfilehash: 34ea433ad7315d61df8cf8e22bae1166d3210af3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457314"
---
# <a name="goodthreshold"></a><span data-ttu-id="b0f95-103">гудсрешолд</span><span class="sxs-lookup"><span data-stu-id="b0f95-103">GoodThreshold</span></span>

<span data-ttu-id="b0f95-104">Элемент **гудсрешолд** указывает процент участников, для которых должен быть открыт период времени, чтобы определить, какой период времени должен быть приемлемым для предполагаемого времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="b0f95-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="b0f95-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="b0f95-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="b0f95-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="b0f95-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="b0f95-107">гудсрешолд</span><span class="sxs-lookup"><span data-stu-id="b0f95-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="b0f95-108">**int**</span><span class="sxs-lookup"><span data-stu-id="b0f95-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b0f95-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b0f95-109">Attributes and elements</span></span>

<span data-ttu-id="b0f95-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b0f95-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b0f95-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b0f95-111">Attributes</span></span>

<span data-ttu-id="b0f95-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b0f95-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b0f95-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b0f95-113">Child elements</span></span>

<span data-ttu-id="b0f95-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b0f95-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b0f95-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b0f95-115">Parent elements</span></span>

|<span data-ttu-id="b0f95-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b0f95-116">**Element**</span></span>|<span data-ttu-id="b0f95-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b0f95-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b0f95-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="b0f95-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="b0f95-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="b0f95-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="b0f95-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="b0f95-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b0f95-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b0f95-121">Text value</span></span>

<span data-ttu-id="b0f95-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="b0f95-122">A text value is required.</span></span> <span data-ttu-id="b0f95-123">Ожидаемые целые значения находятся в диапазоне от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="b0f95-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b0f95-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="b0f95-124">Remarks</span></span>

<span data-ttu-id="b0f95-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="b0f95-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="b0f95-126">Элемент **гудсрешолд** также определяет, что встречами считается удовлетворительно.</span><span class="sxs-lookup"><span data-stu-id="b0f95-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="b0f95-127">В процентах от участников с конфликтами меньше, чем на 50 процентов, рекомендуемое время проведения собрания определено как справедливое.</span><span class="sxs-lookup"><span data-stu-id="b0f95-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="b0f95-128">Хорошее пороговое значение плюс 50 соответствует проценту, определяющему хорошее/приемлемое пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="b0f95-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="b0f95-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b0f95-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="b0f95-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b0f95-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b0f95-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b0f95-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b0f95-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b0f95-132">Schema Name</span></span>  <br/> |<span data-ttu-id="b0f95-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b0f95-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="b0f95-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b0f95-134">Validation File</span></span>  <br/> |<span data-ttu-id="b0f95-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b0f95-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b0f95-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b0f95-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="b0f95-137">False</span><span class="sxs-lookup"><span data-stu-id="b0f95-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b0f95-138">См. также</span><span class="sxs-lookup"><span data-stu-id="b0f95-138">See also</span></span>



[<span data-ttu-id="b0f95-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b0f95-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="b0f95-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b0f95-140">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

