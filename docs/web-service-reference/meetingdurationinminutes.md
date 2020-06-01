---
title: митингдуратионинминутес
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
description: Элемент Митингдуратионинминутес указывает продолжительность собрания.
ms.openlocfilehash: b41e234be40c2ad8b28047ae2e812edfd66af644
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44467489"
---
# <a name="meetingdurationinminutes"></a><span data-ttu-id="9e028-103">митингдуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="9e028-103">MeetingDurationInMinutes</span></span>

<span data-ttu-id="9e028-104">Элемент **митингдуратионинминутес** указывает продолжительность собрания.</span><span class="sxs-lookup"><span data-stu-id="9e028-104">The **MeetingDurationInMinutes** element specifies the duration of the meeting to be suggested.</span></span> 
  
[<span data-ttu-id="9e028-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="9e028-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="9e028-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="9e028-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="9e028-107">митингдуратионинминутес</span><span class="sxs-lookup"><span data-stu-id="9e028-107">MeetingDurationInMinutes</span></span>](meetingdurationinminutes.md)
  
```xml
<MeetingDurationInMinutes>...</MeetingDurationInMinutes>
```

 <span data-ttu-id="9e028-108">**int**</span><span class="sxs-lookup"><span data-stu-id="9e028-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e028-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9e028-109">Attributes and elements</span></span>

<span data-ttu-id="9e028-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9e028-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e028-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9e028-111">Attributes</span></span>

<span data-ttu-id="9e028-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e028-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9e028-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9e028-113">Child elements</span></span>

<span data-ttu-id="9e028-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9e028-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9e028-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9e028-115">Parent elements</span></span>

|<span data-ttu-id="9e028-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9e028-116">**Element**</span></span>|<span data-ttu-id="9e028-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9e028-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e028-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="9e028-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="9e028-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="9e028-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="9e028-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9e028-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e028-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9e028-121">Text value</span></span>

<span data-ttu-id="9e028-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="9e028-122">A text value is required.</span></span> <span data-ttu-id="9e028-123">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="9e028-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e028-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="9e028-124">Remarks</span></span>

<span data-ttu-id="9e028-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="9e028-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9e028-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9e028-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9e028-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9e028-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e028-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9e028-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9e028-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9e028-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9e028-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9e028-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9e028-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9e028-131">Validation File</span></span>  <br/> |<span data-ttu-id="9e028-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9e028-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9e028-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9e028-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e028-134">False</span><span class="sxs-lookup"><span data-stu-id="9e028-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e028-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9e028-135">See also</span></span>



[<span data-ttu-id="9e028-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9e028-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="9e028-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="9e028-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

