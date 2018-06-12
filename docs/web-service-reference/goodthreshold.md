---
title: GoodThreshold
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
description: Элемент GoodThreshold указывает процент участников, которые должны иметь периода времени, которые открываются в порядке в промежуток времени, в рамках программы как хороший предложенного собрания.
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833746"
---
# <a name="goodthreshold"></a><span data-ttu-id="f5452-103">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="f5452-103">GoodThreshold</span></span>

<span data-ttu-id="f5452-104">Элемент **GoodThreshold** указывает процент участников, которые должны иметь периода времени, которые открываются в порядке в промежуток времени, в рамках программы как хороший предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="f5452-104">The **GoodThreshold** element specifies the percentage of attendees that must have the time period open in order for the time period to qualify as a Good suggested meeting time.</span></span> 
  
[<span data-ttu-id="f5452-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="f5452-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="f5452-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f5452-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="f5452-107">GoodThreshold</span><span class="sxs-lookup"><span data-stu-id="f5452-107">GoodThreshold</span></span>](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
```

 <span data-ttu-id="f5452-108">**int**</span><span class="sxs-lookup"><span data-stu-id="f5452-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f5452-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f5452-109">Attributes and elements</span></span>

<span data-ttu-id="f5452-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f5452-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f5452-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f5452-111">Attributes</span></span>

<span data-ttu-id="f5452-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5452-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f5452-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f5452-113">Child elements</span></span>

<span data-ttu-id="f5452-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="f5452-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f5452-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f5452-115">Parent elements</span></span>

|<span data-ttu-id="f5452-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f5452-116">**Element**</span></span>|<span data-ttu-id="f5452-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f5452-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f5452-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="f5452-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="f5452-119">Содержит параметры для получения сведения о предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="f5452-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="f5452-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="f5452-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f5452-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f5452-121">Text value</span></span>

<span data-ttu-id="f5452-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="f5452-122">A text value is required.</span></span> <span data-ttu-id="f5452-123">Приведены значения параметра ожидаемое целое число от 0 до 50.</span><span class="sxs-lookup"><span data-stu-id="f5452-123">The expected integer values are between 0 and 50.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f5452-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="f5452-124">Remarks</span></span>

<span data-ttu-id="f5452-125">Этот элемент является обязательным, если используется элемент [SuggestionsViewOptions](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="f5452-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> <span data-ttu-id="f5452-126">Элемент **GoodThreshold** также определяет, какие собрания считаются объединение.</span><span class="sxs-lookup"><span data-stu-id="f5452-126">The **GoodThreshold** element also determines what meetings are considered Fair.</span></span> <span data-ttu-id="f5452-127">Он является процент участников с конфликтами меньше, чем хороший порог и выше, чем 50 процентов предложенного собрания определяется как объединение.</span><span class="sxs-lookup"><span data-stu-id="f5452-127">It the percentage of attendees with conflicts is less than the Good Threshold and higher than 50 percent, the suggested meeting time qualifies as Fair.</span></span> <span data-ttu-id="f5452-128">Хороший порог плюс 50 — это процент, который определяет хорошо/объединение пороговое значение.</span><span class="sxs-lookup"><span data-stu-id="f5452-128">The Good Threshold plus 50 equals the percentage that defines the Good/Fair threshold.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f5452-129">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f5452-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f5452-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f5452-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f5452-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f5452-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f5452-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f5452-132">Schema Name</span></span>  <br/> |<span data-ttu-id="f5452-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f5452-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f5452-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f5452-134">Validation File</span></span>  <br/> |<span data-ttu-id="f5452-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f5452-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f5452-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f5452-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="f5452-137">False</span><span class="sxs-lookup"><span data-stu-id="f5452-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f5452-138">См. также</span><span class="sxs-lookup"><span data-stu-id="f5452-138">See also</span></span>



[<span data-ttu-id="f5452-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f5452-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="f5452-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f5452-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

