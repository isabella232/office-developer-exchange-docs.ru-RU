---
title: Определение часового пояса
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
description: Элемент определение часового пояса указывает периодов и переходы, определяющие часового пояса.
ms.openlocfilehash: ffd5ed0c862af794e4aff2387f508849b1d5fd5d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840200"
---
# <a name="timezonedefinition"></a><span data-ttu-id="e8990-103">Определение часового пояса</span><span class="sxs-lookup"><span data-stu-id="e8990-103">TimeZoneDefinition</span></span>

<span data-ttu-id="e8990-104">Элемент **Определение часового пояса** указывает периодов и переходы, определяющие часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="e8990-105">**TimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="e8990-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8990-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8990-106">Attributes and elements</span></span>

<span data-ttu-id="e8990-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="e8990-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8990-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8990-108">Attributes</span></span>

|<span data-ttu-id="e8990-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="e8990-109">**Attribute**</span></span>|<span data-ttu-id="e8990-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8990-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e8990-111">Id</span><span class="sxs-lookup"><span data-stu-id="e8990-111">Id</span></span>  <br/> |<span data-ttu-id="e8990-112">Представляет уникальный идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="e8990-113">Имя</span><span class="sxs-lookup"><span data-stu-id="e8990-113">Name</span></span>  <br/> |<span data-ttu-id="e8990-114">Представляет описательное имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e8990-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8990-115">Child elements</span></span>

|<span data-ttu-id="e8990-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8990-116">**Element**</span></span>|<span data-ttu-id="e8990-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8990-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8990-118">Периоды</span><span class="sxs-lookup"><span data-stu-id="e8990-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="e8990-119">Представляет массив элементов [периода времени](period.md) , которые определяют смещение времени на различных этапах часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="e8990-120">TransitionsGroups</span><span class="sxs-lookup"><span data-stu-id="e8990-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="e8990-121">Представляет массив [TransitionsGroup](transitionsgroup.md) элементов, которые задают переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="e8990-122">Переходы между</span><span class="sxs-lookup"><span data-stu-id="e8990-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="e8990-123">Представляет массив переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e8990-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8990-124">Parent elements</span></span>

|<span data-ttu-id="e8990-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8990-125">**Element**</span></span>|<span data-ttu-id="e8990-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8990-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8990-127">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="e8990-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="e8990-128">Представляет собой массив из определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="e8990-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="e8990-129">TimeZoneContext</span><span class="sxs-lookup"><span data-stu-id="e8990-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="e8990-130">Представляет определение часового пояса по умолчанию, который будет использоваться для областей свойства даты и времени объектов, которые создаются, обновить и получить с помощью веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="e8990-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e8990-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="e8990-131">Remarks</span></span>

<span data-ttu-id="e8990-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="e8990-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8990-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="e8990-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8990-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="e8990-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8990-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="e8990-135">Schema Name</span></span>  <br/> |<span data-ttu-id="e8990-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="e8990-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8990-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="e8990-137">Validation File</span></span>  <br/> |<span data-ttu-id="e8990-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e8990-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8990-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="e8990-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8990-140">False</span><span class="sxs-lookup"><span data-stu-id="e8990-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8990-141">См. также</span><span class="sxs-lookup"><span data-stu-id="e8990-141">See also</span></span>



- [<span data-ttu-id="e8990-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e8990-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

