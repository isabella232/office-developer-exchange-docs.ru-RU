---
title: MeetingDurationInMinutes
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MeetingDurationInMinutes
api_type:
- schema
ms.assetid: bb86b275-9c29-4daf-8196-8d505b87a4f4
description: Элемент MeetingDurationInMinutes указывает продолжительность собрания предлагаются.
ms.openlocfilehash: 2ff60b69fb352c2ac7316f1ca231bb04da67ead2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834433"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="9e04f-103">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="9e04f-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="9e04f-104">Элемент **MeetingDurationInMinutes** указывает продолжительность собрания предлагаются.</span><span class="sxs-lookup"><span data-stu-id="9e04f-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="9e04f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="9e04f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="9e04f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="9e04f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="9e04f-107">MeetingDurationInMinutes</span><span class="sxs-lookup"><span data-stu-id="9e04f-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="9e04f-108">**int**</span><span class="sxs-lookup"><span data-stu-id="9e04f-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e04f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e04f-109">Attributes and elements</span></span>

<span data-ttu-id="9e04f-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="9e04f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e04f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e04f-111">Attributes</span></span>

<span data-ttu-id="9e04f-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e04f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e04f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e04f-113">Child elements</span></span>

<span data-ttu-id="9e04f-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="9e04f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e04f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e04f-115">Parent elements</span></span>

|<span data-ttu-id="9e04f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e04f-116">**Element**</span></span>|<span data-ttu-id="9e04f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e04f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e04f-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="9e04f-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="9e04f-119">Содержит параметры для получения сведения о предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="9e04f-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="9e04f-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9e04f-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e04f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9e04f-121">Text value</span></span>

<span data-ttu-id="9e04f-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="9e04f-122">A text value is required.</span></span> <span data-ttu-id="9e04f-123">Текстовое значение представляет собой целое число.</span><span class="sxs-lookup"><span data-stu-id="9e04f-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e04f-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="9e04f-124">Remarks</span></span>

<span data-ttu-id="9e04f-125">Этот элемент является обязательным, если используется элемент [SuggestionsViewOptions](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="9e04f-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9e04f-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9e04f-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9e04f-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e04f-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e04f-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e04f-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e04f-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e04f-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9e04f-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9e04f-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e04f-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e04f-131">Validation File</span></span>  <br/> |<span data-ttu-id="9e04f-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9e04f-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e04f-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e04f-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e04f-134">False</span><span class="sxs-lookup"><span data-stu-id="9e04f-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e04f-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9e04f-135">See also</span></span>



[<span data-ttu-id="9e04f-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9e04f-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="9e04f-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="9e04f-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

