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
ms.openlocfilehash: 69ab4e0b23f85e5b8786ba2dd934850cadc88f0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834381"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="e2d68-103">максимумресултсбидай</span><span class="sxs-lookup"><span data-stu-id="e2d68-103">MaximumResultsByDay</span></span>

<span data-ttu-id="e2d68-104">Элемент **максимумресултсбидай** указывает количество предложенных времени проведения собрания в день, возвращенный в ответе.</span><span class="sxs-lookup"><span data-stu-id="e2d68-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="e2d68-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="e2d68-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="e2d68-106">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="e2d68-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="e2d68-107">максимумресултсбидай</span><span class="sxs-lookup"><span data-stu-id="e2d68-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="e2d68-108">**int**</span><span class="sxs-lookup"><span data-stu-id="e2d68-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="e2d68-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e2d68-109">Attributes and elements</span></span>

<span data-ttu-id="e2d68-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e2d68-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2d68-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e2d68-111">Attributes</span></span>

<span data-ttu-id="e2d68-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2d68-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2d68-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e2d68-113">Child elements</span></span>

<span data-ttu-id="e2d68-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="e2d68-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2d68-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e2d68-115">Parent elements</span></span>

|<span data-ttu-id="e2d68-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e2d68-116">**Element**</span></span>|<span data-ttu-id="e2d68-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e2d68-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2d68-118">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="e2d68-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="e2d68-119">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="e2d68-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="e2d68-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="e2d68-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2d68-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e2d68-121">Text value</span></span>

<span data-ttu-id="e2d68-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="e2d68-122">A text value is required.</span></span> <span data-ttu-id="e2d68-123">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="e2d68-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2d68-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="e2d68-124">Remarks</span></span>

<span data-ttu-id="e2d68-125">Этот элемент является обязательным, если используется элемент [сугжестионсвиевоптионс](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="e2d68-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e2d68-126">Схема, описывающая этот элемент, находится в виртуальном каталоге EWS компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e2d68-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="e2d68-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e2d68-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2d68-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e2d68-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2d68-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e2d68-129">Schema Name</span></span>  <br/> |<span data-ttu-id="e2d68-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e2d68-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2d68-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e2d68-131">Validation File</span></span>  <br/> |<span data-ttu-id="e2d68-132">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e2d68-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2d68-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e2d68-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2d68-134">False</span><span class="sxs-lookup"><span data-stu-id="e2d68-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2d68-135">См. также</span><span class="sxs-lookup"><span data-stu-id="e2d68-135">See also</span></span>

- [<span data-ttu-id="e2d68-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="e2d68-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="e2d68-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="e2d68-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

