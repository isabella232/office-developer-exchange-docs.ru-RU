---
title: MaximumResultsByDay
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
description: Элемент MaximumResultsByDay указывает, сколько раз предложенного собрания в день, возвращаемого в ответе.
ms.openlocfilehash: 69ab4e0b23f85e5b8786ba2dd934850cadc88f0e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834381"
---
# <a name="maximumresultsbyday"></a><span data-ttu-id="d0763-103">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="d0763-103">MaximumResultsByDay</span></span>

<span data-ttu-id="d0763-104">Элемент **MaximumResultsByDay** указывает, сколько раз предложенного собрания в день, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="d0763-104">The **MaximumResultsByDay** element specifies the number of suggested meeting times per a day returned in the response.</span></span> 
  
[<span data-ttu-id="d0763-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d0763-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="d0763-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="d0763-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md)
  
[<span data-ttu-id="d0763-107">MaximumResultsByDay</span><span class="sxs-lookup"><span data-stu-id="d0763-107">MaximumResultsByDay</span></span>](maximumresultsbyday.md)
  
```xml
<MaximumResultsByDay>...</MaximumResultsByDay>
```

<span data-ttu-id="d0763-108">**int**</span><span class="sxs-lookup"><span data-stu-id="d0763-108">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d0763-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d0763-109">Attributes and elements</span></span>

<span data-ttu-id="d0763-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d0763-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0763-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d0763-111">Attributes</span></span>

<span data-ttu-id="d0763-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="d0763-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0763-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d0763-113">Child elements</span></span>

<span data-ttu-id="d0763-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="d0763-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d0763-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d0763-115">Parent elements</span></span>

|<span data-ttu-id="d0763-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d0763-116">**Element**</span></span>|<span data-ttu-id="d0763-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d0763-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0763-118">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="d0763-118">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="d0763-119">Содержит параметры для получения сведения о предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="d0763-119">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="d0763-120">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d0763-120">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d0763-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d0763-121">Text value</span></span>

<span data-ttu-id="d0763-122">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d0763-122">A text value is required.</span></span> <span data-ttu-id="d0763-123">Текстовое значение представляет собой целое число.</span><span class="sxs-lookup"><span data-stu-id="d0763-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d0763-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="d0763-124">Remarks</span></span>

<span data-ttu-id="d0763-125">Этот элемент является обязательным, если используется элемент [SuggestionsViewOptions](suggestionsviewoptions.md) .</span><span class="sxs-lookup"><span data-stu-id="d0763-125">This element is required if the [SuggestionsViewOptions](suggestionsviewoptions.md) element is used.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d0763-126">Схема, описывающая этот элемент находится в виртуальном каталоге EWS компьютера, на котором выполняется Microsoft® Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d0763-126">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d0763-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d0763-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0763-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d0763-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0763-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d0763-129">Schema Name</span></span>  <br/> |<span data-ttu-id="d0763-130">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d0763-130">Types schema</span></span>  <br/> |
|<span data-ttu-id="d0763-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d0763-131">Validation File</span></span>  <br/> |<span data-ttu-id="d0763-132">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0763-132">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0763-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d0763-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="d0763-134">False</span><span class="sxs-lookup"><span data-stu-id="d0763-134">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d0763-135">См. также</span><span class="sxs-lookup"><span data-stu-id="d0763-135">See also</span></span>

- [<span data-ttu-id="d0763-136">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d0763-136">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="d0763-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d0763-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

