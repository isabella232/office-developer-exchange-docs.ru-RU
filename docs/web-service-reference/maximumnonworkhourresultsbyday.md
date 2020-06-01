---
title: максимумнонворкхаурресултсбидай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumNonWorkHourResultsByDay
api_type:
- schema
ms.assetid: 9fb7314d-779c-4b1f-9d7c-b5cb092ed134
description: Элемент Максимумнонворкхаурресултсбидай указывает количество предполагаемых результатов для времени проведения собрания, которое не превышает обычные рабочие часы в день.
ms.openlocfilehash: 410d6bd84838d979af6bc53ca47f445ae55a09e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465501"
---
# <a name="maximumnonworkhourresultsbyday"></a><span data-ttu-id="f23fd-103">максимумнонворкхаурресултсбидай</span><span class="sxs-lookup"><span data-stu-id="f23fd-103">MaximumNonWorkHourResultsByDay</span></span>

<span data-ttu-id="f23fd-104">Элемент **максимумнонворкхаурресултсбидай** указывает количество предполагаемых результатов для времени проведения собрания, которое не превышает обычные рабочие часы в день.</span><span class="sxs-lookup"><span data-stu-id="f23fd-104">The **MaximumNonWorkHourResultsByDay** element specifies the number of suggested results for meeting times outside regular working hours per day.</span></span> 
  
[<span data-ttu-id="f23fd-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="f23fd-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="f23fd-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="f23fd-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="f23fd-107">максимумнонворкхаурресултсбидай</span><span class="sxs-lookup"><span data-stu-id="f23fd-107">MaximumNonWorkHourResultsByDay</span></span>](maximumnonworkhourresultsbyday.md)
  
```xml
<MaximumNonWorkHourResultsByDay>...</MaximumNonWorkHourResultsByDay>
```

 <span data-ttu-id="f23fd-108">**int**</span><span class="sxs-lookup"><span data-stu-id="f23fd-108">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f23fd-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f23fd-109">Attributes and elements</span></span>

<span data-ttu-id="f23fd-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f23fd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f23fd-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f23fd-111">Attributes</span></span>

<span data-ttu-id="f23fd-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f23fd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f23fd-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f23fd-113">Child elements</span></span>

<span data-ttu-id="f23fd-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f23fd-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f23fd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f23fd-115">Parent elements</span></span>

|<span data-ttu-id="f23fd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f23fd-116">**Element**</span></span>|<span data-ttu-id="f23fd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f23fd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f23fd-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="f23fd-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="f23fd-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="f23fd-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="f23fd-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="f23fd-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f23fd-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f23fd-121">Text value</span></span>

<span data-ttu-id="f23fd-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="f23fd-122">A text value is required.</span></span> <span data-ttu-id="f23fd-123">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="f23fd-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f23fd-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="f23fd-124">Remarks</span></span>

<span data-ttu-id="f23fd-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="f23fd-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f23fd-126">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f23fd-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f23fd-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f23fd-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f23fd-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f23fd-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f23fd-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f23fd-129">Schema Name</span></span>  <br/> |<span data-ttu-id="f23fd-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f23fd-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="f23fd-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f23fd-131">Validation File</span></span>  <br/> |<span data-ttu-id="f23fd-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f23fd-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f23fd-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f23fd-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="f23fd-134">False</span><span class="sxs-lookup"><span data-stu-id="f23fd-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f23fd-135">См. также</span><span class="sxs-lookup"><span data-stu-id="f23fd-135">See also</span></span>



[<span data-ttu-id="f23fd-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f23fd-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="f23fd-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f23fd-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

