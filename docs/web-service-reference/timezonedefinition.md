---
title: тимезонедефинитион
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinition
api_type:
- schema
ms.assetid: b005a80c-addb-4409-beff-e5162076752c
description: Элемент Тимезонедефинитион указывает точки и переходы, определяющие часовой пояс.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840200"
---
# <a name="timezonedefinition"></a><span data-ttu-id="e342c-103">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="e342c-103">TimeZoneDefinition</span></span>

<span data-ttu-id="e342c-104">Элемент **тимезонедефинитион** указывает точки и переходы, определяющие часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="e342c-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="e342c-105">**тимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="e342c-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e342c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e342c-106">Attributes and elements</span></span>

<span data-ttu-id="e342c-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e342c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e342c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e342c-108">Attributes</span></span>

|<span data-ttu-id="e342c-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e342c-109">**Attribute**</span></span>|<span data-ttu-id="e342c-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e342c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e342c-111">Id</span><span class="sxs-lookup"><span data-stu-id="e342c-111">Id</span></span>  <br/> |<span data-ttu-id="e342c-112">Представляет уникальный идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e342c-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="e342c-113">Имя</span><span class="sxs-lookup"><span data-stu-id="e342c-113">Name</span></span>  <br/> |<span data-ttu-id="e342c-114">Представляет описательное имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e342c-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e342c-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e342c-115">Child elements</span></span>

|<span data-ttu-id="e342c-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e342c-116">**Element**</span></span>|<span data-ttu-id="e342c-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e342c-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e342c-118">Periods</span><span class="sxs-lookup"><span data-stu-id="e342c-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="e342c-119">Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e342c-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="e342c-120">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="e342c-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="e342c-121">Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e342c-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e342c-122">Выполняет</span><span class="sxs-lookup"><span data-stu-id="e342c-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e342c-123">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e342c-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e342c-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e342c-124">Parent elements</span></span>

|<span data-ttu-id="e342c-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e342c-125">**Element**</span></span>|<span data-ttu-id="e342c-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e342c-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e342c-127">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="e342c-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="e342c-128">Представляет массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="e342c-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="e342c-129">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="e342c-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="e342c-130">Представляет определение часового пояса по умолчанию, которое будет использоваться для определения свойств DateTime объектов, которые создаются, обновляются и извлекаются с помощью веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="e342c-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e342c-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="e342c-131">Remarks</span></span>

<span data-ttu-id="e342c-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e342c-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e342c-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e342c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e342c-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e342c-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e342c-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e342c-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e342c-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e342c-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e342c-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e342c-137">Validation File</span></span>  <br/> |<span data-ttu-id="e342c-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="e342c-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e342c-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e342c-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e342c-140">False</span><span class="sxs-lookup"><span data-stu-id="e342c-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e342c-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e342c-141">See also</span></span>



- [<span data-ttu-id="e342c-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e342c-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

