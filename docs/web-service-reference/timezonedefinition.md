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
ms.openlocfilehash: 58d34556686bfc77244b5829798eada51a1df843
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466068"
---
# <a name="timezonedefinition"></a><span data-ttu-id="08ce6-103">тимезонедефинитион</span><span class="sxs-lookup"><span data-stu-id="08ce6-103">TimeZoneDefinition</span></span>

<span data-ttu-id="08ce6-104">Элемент **тимезонедефинитион** указывает точки и переходы, определяющие часовой пояс.</span><span class="sxs-lookup"><span data-stu-id="08ce6-104">The **TimeZoneDefinition** element specifies the periods and transitions that define a time zone.</span></span> 
  
```XML
<TimeZoneDefinition Id="" Name="">
   <Periods/>
   <TransitionsGroups/>
   <Transitions/>
</TimeZoneDefinition>

```

 <span data-ttu-id="08ce6-105">**тимезонедефинитионтипе**</span><span class="sxs-lookup"><span data-stu-id="08ce6-105">**TimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08ce6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="08ce6-106">Attributes and elements</span></span>

<span data-ttu-id="08ce6-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="08ce6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08ce6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="08ce6-108">Attributes</span></span>

|<span data-ttu-id="08ce6-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="08ce6-109">**Attribute**</span></span>|<span data-ttu-id="08ce6-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ce6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="08ce6-111">Id</span><span class="sxs-lookup"><span data-stu-id="08ce6-111">Id</span></span>  <br/> |<span data-ttu-id="08ce6-112">Представляет уникальный идентификатор часового пояса.</span><span class="sxs-lookup"><span data-stu-id="08ce6-112">Represents the unique identifier of the time zone.</span></span>  <br/> |
|<span data-ttu-id="08ce6-113">Имя</span><span class="sxs-lookup"><span data-stu-id="08ce6-113">Name</span></span>  <br/> |<span data-ttu-id="08ce6-114">Представляет описательное имя часового пояса.</span><span class="sxs-lookup"><span data-stu-id="08ce6-114">Represents the descriptive name of the time zone.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="08ce6-115">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="08ce6-115">Child elements</span></span>

|<span data-ttu-id="08ce6-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08ce6-116">**Element**</span></span>|<span data-ttu-id="08ce6-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ce6-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ce6-118">Periods</span><span class="sxs-lookup"><span data-stu-id="08ce6-118">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="08ce6-119">Представляет массив элементов [period](period.md) , определяющий смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="08ce6-119">Represents an array of [Period](period.md) elements that define the time offset at different stages of the time zone.</span></span>  <br/> |
|[<span data-ttu-id="08ce6-120">транситионсграупс</span><span class="sxs-lookup"><span data-stu-id="08ce6-120">TransitionsGroups</span></span>](transitionsgroups.md) <br/> |<span data-ttu-id="08ce6-121">Представляет массив элементов [транситионсграуп](transitionsgroup.md) , определяющих переходы часового пояса.</span><span class="sxs-lookup"><span data-stu-id="08ce6-121">Represents an array of [TransitionsGroup](transitionsgroup.md) elements that specify time zone transitions.</span></span>  <br/> |
|[<span data-ttu-id="08ce6-122">Выполняет</span><span class="sxs-lookup"><span data-stu-id="08ce6-122">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="08ce6-123">Представляет массив переходов часового пояса.</span><span class="sxs-lookup"><span data-stu-id="08ce6-123">Represents an array of time zone transitions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="08ce6-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="08ce6-124">Parent elements</span></span>

|<span data-ttu-id="08ce6-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="08ce6-125">**Element**</span></span>|<span data-ttu-id="08ce6-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="08ce6-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08ce6-127">тимезонедефинитионс</span><span class="sxs-lookup"><span data-stu-id="08ce6-127">TimeZoneDefinitions</span></span>](timezonedefinitions.md) <br/> |<span data-ttu-id="08ce6-128">Представляет массив определений часовых поясов.</span><span class="sxs-lookup"><span data-stu-id="08ce6-128">Represents an array of time zone definitions.</span></span>  <br/> |
|[<span data-ttu-id="08ce6-129">тимезонеконтекст</span><span class="sxs-lookup"><span data-stu-id="08ce6-129">TimeZoneContext</span></span>](timezonecontext.md) <br/> |<span data-ttu-id="08ce6-130">Представляет определение часового пояса по умолчанию, которое будет использоваться для определения свойств DateTime объектов, которые создаются, обновляются и извлекаются с помощью веб-служб Exchange (EWS).</span><span class="sxs-lookup"><span data-stu-id="08ce6-130">Represents the default time zone definition that is to be used for scoping the DateTime properties of objects that are created, updated, and retrieved by using Exchange Web Services (EWS).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="08ce6-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="08ce6-131">Remarks</span></span>

<span data-ttu-id="08ce6-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="08ce6-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08ce6-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="08ce6-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08ce6-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="08ce6-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08ce6-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="08ce6-135">Schema Name</span></span>  <br/> |<span data-ttu-id="08ce6-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="08ce6-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="08ce6-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="08ce6-137">Validation File</span></span>  <br/> |<span data-ttu-id="08ce6-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="08ce6-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08ce6-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="08ce6-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="08ce6-140">False</span><span class="sxs-lookup"><span data-stu-id="08ce6-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08ce6-141">См. также</span><span class="sxs-lookup"><span data-stu-id="08ce6-141">See also</span></span>



- [<span data-ttu-id="08ce6-142">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="08ce6-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

