---
title: DetailedSuggestionsWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DetailedSuggestionsWindow
api_type:
- schema
ms.assetid: 7b348d63-6a7d-45f4-9562-5c42243d63a5
description: Элемент DetailedSuggestionsWindow указывает промежуток времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.
ms.openlocfilehash: 8a3af0178d0c96b50f4dd641716a9f7a7be8f7a2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762082"
---
# <a name="detailedsuggestionswindow"></a><span data-ttu-id="57d0f-103">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="57d0f-103">DetailedSuggestionsWindow</span></span>

<span data-ttu-id="57d0f-104">Элемент **DetailedSuggestionsWindow** указывает промежуток времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="57d0f-104">The **DetailedSuggestionsWindow** element identifies the time span that is queried for detailed information about suggested meeting times.</span></span> 
  
- [<span data-ttu-id="57d0f-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="57d0f-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) 
- [<span data-ttu-id="57d0f-106">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="57d0f-106">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) 
- [<span data-ttu-id="57d0f-107">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="57d0f-107">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md)
  
```xml
<DetailedSuggestionsWindow>
   <StartTime>...</StartTime>
   <EndTime>...</EndTime>
</DetailedSuggestionsWindow>
```

 <span data-ttu-id="57d0f-108">**Срок действия**</span><span class="sxs-lookup"><span data-stu-id="57d0f-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57d0f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57d0f-109">Attributes and elements</span></span>

<span data-ttu-id="57d0f-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="57d0f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57d0f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57d0f-111">Attributes</span></span>

<span data-ttu-id="57d0f-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="57d0f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57d0f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57d0f-113">Child elements</span></span>

|<span data-ttu-id="57d0f-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57d0f-114">**Element**</span></span>|<span data-ttu-id="57d0f-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57d0f-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d0f-116">Время начала</span><span class="sxs-lookup"><span data-stu-id="57d0f-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="57d0f-117">Представляет начало интервала времени, запрос для получения дополнительных сведений о времени предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="57d0f-117">Represents the start of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
|[<span data-ttu-id="57d0f-118">Время окончания</span><span class="sxs-lookup"><span data-stu-id="57d0f-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="57d0f-119">Представляет окончания интервала времени, запрос для получения дополнительных сведений о времени предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="57d0f-119">Represents the end of the time span queried for detailed information about suggested meeting times.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57d0f-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57d0f-120">Parent elements</span></span>

|<span data-ttu-id="57d0f-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57d0f-121">**Element**</span></span>|<span data-ttu-id="57d0f-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57d0f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57d0f-123">SuggestionsViewOptions</span><span class="sxs-lookup"><span data-stu-id="57d0f-123">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="57d0f-124">Содержит параметры для получения сведения о предложения о собрании.</span><span class="sxs-lookup"><span data-stu-id="57d0f-124">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> <span data-ttu-id="57d0f-125">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="57d0f-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="57d0f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="57d0f-126">Remarks</span></span>

<span data-ttu-id="57d0f-127">Этот элемент не требуется.</span><span class="sxs-lookup"><span data-stu-id="57d0f-127">This element is not required.</span></span>
  
> [!NOTE]
> <span data-ttu-id="57d0f-128">Схема с описанием этого элемента находится в каталоге /EWS/ на компьютере, на котором запущено приложение MicrosoftExchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="57d0f-128">The schema that describes this element is located in the /EWS/ directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="57d0f-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57d0f-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57d0f-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57d0f-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57d0f-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57d0f-131">Schema Name</span></span>  <br/> |<span data-ttu-id="57d0f-132">Схема Types</span><span class="sxs-lookup"><span data-stu-id="57d0f-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="57d0f-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57d0f-133">Validation File</span></span>  <br/> |<span data-ttu-id="57d0f-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="57d0f-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57d0f-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57d0f-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="57d0f-136">False</span><span class="sxs-lookup"><span data-stu-id="57d0f-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57d0f-137">См. также</span><span class="sxs-lookup"><span data-stu-id="57d0f-137">See also</span></span>

- [<span data-ttu-id="57d0f-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="57d0f-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="57d0f-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="57d0f-139">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

