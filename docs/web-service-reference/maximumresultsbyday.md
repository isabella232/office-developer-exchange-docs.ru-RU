---
title: максимумресултсбидай
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaximumResultsByDay
api_type:
- schema
ms.assetid: d581a12a-2b8e-4960-ae14-c8c4aa0b1849
description: Элемент Максимумресултсбидай указывает количество предложенных времени проведения собрания в день, возвращенный в ответе.
ms.openlocfilehash: 46d5c35a83034b8b968901fbc4ee57d046b6c164
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/01/2020
ms.locfileid: "44468420"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="9799a-103">максимумресултсбидай</span><span class="sxs-lookup"><span data-stu-id="9799a-103">MaximumResultsByDay</span></span>

<span data-ttu-id="9799a-104">Элемент **максимумресултсбидай** указывает количество предложенных времени проведения собрания в день, возвращенный в ответе.</span><span class="sxs-lookup"><span data-stu-id="9799a-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="9799a-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="9799a-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="9799a-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="9799a-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="9799a-107">максимумресултсбидай</span><span class="sxs-lookup"><span data-stu-id="9799a-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="9799a-108">**int**</span><span class="sxs-lookup"><span data-stu-id="9799a-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9799a-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9799a-109">Attributes and elements</span></span>

<span data-ttu-id="9799a-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9799a-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9799a-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9799a-111">Attributes</span></span>

<span data-ttu-id="9799a-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9799a-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9799a-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9799a-113">Child elements</span></span>

<span data-ttu-id="9799a-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9799a-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9799a-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9799a-115">Parent elements</span></span>

|<span data-ttu-id="9799a-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9799a-116">**Element**</span></span>|<span data-ttu-id="9799a-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9799a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9799a-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="9799a-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="9799a-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="9799a-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="9799a-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="9799a-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9799a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9799a-121">Text value</span></span>

<span data-ttu-id="9799a-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="9799a-122">A text value is required.</span></span> <span data-ttu-id="9799a-123">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="9799a-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9799a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="9799a-124">Remarks</span></span>

<span data-ttu-id="9799a-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="9799a-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9799a-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9799a-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="9799a-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9799a-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9799a-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9799a-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9799a-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9799a-129">Schema Name</span></span>  <br/> |<span data-ttu-id="9799a-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9799a-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="9799a-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9799a-131">Validation File</span></span>  <br/> |<span data-ttu-id="9799a-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9799a-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9799a-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9799a-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="9799a-134">False</span><span class="sxs-lookup"><span data-stu-id="9799a-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9799a-135">См. также</span><span class="sxs-lookup"><span data-stu-id="9799a-135">See also</span></span>

- [<span data-ttu-id="9799a-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="9799a-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="9799a-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="9799a-137">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

