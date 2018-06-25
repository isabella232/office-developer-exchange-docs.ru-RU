---
title: Range
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Элемент Range указывает диапазон вхождения элемента календаря для повторяющегося элемента календаря.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834946"
---
# <a name="range"></a><span data-ttu-id="f24f8-103">Range</span><span class="sxs-lookup"><span data-stu-id="f24f8-103">Range</span></span>

<span data-ttu-id="f24f8-104">Элемент **Range** указывает диапазон вхождения элемента календаря для повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="f24f8-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="f24f8-105">**OccurrencesRangeType**</span><span class="sxs-lookup"><span data-stu-id="f24f8-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f24f8-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f24f8-106">Attributes and elements</span></span>

<span data-ttu-id="f24f8-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="f24f8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f24f8-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f24f8-108">Attributes</span></span>

|<span data-ttu-id="f24f8-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="f24f8-109">**Attribute**</span></span>|<span data-ttu-id="f24f8-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f24f8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f24f8-111">**Start**</span><span class="sxs-lookup"><span data-stu-id="f24f8-111">**Start**</span></span> <br/> |<span data-ttu-id="f24f8-112">Текстовое значение атрибута **Начать** — это дата начала диапазона повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="f24f8-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="f24f8-113">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="f24f8-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="f24f8-114">**End**</span><span class="sxs-lookup"><span data-stu-id="f24f8-114">**End**</span></span> <br/> |<span data-ttu-id="f24f8-115">Текстовое значение атрибута **окончания** — это дата окончания диапазона повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="f24f8-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="f24f8-116">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="f24f8-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="f24f8-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="f24f8-117">**Count**</span></span> <br/> |<span data-ttu-id="f24f8-118">Текстовое значение атрибута **счетчика** — это число вхождений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="f24f8-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="f24f8-119">Это значение типа **integer** .</span><span class="sxs-lookup"><span data-stu-id="f24f8-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="f24f8-120">**CompareOriginalStartTime**</span><span class="sxs-lookup"><span data-stu-id="f24f8-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="f24f8-121">Текстовое значение **true** для атрибута **CompareOriginalStartTime** указывает, что клиент должен сравнить исходное время начала с новое время начала.</span><span class="sxs-lookup"><span data-stu-id="f24f8-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="f24f8-122">Значение **false** указывает, что клиент не нужно сравнить исходное время начала с новое время начала.</span><span class="sxs-lookup"><span data-stu-id="f24f8-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f24f8-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f24f8-123">Child elements</span></span>

<span data-ttu-id="f24f8-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="f24f8-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f24f8-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f24f8-125">Parent elements</span></span>

[<span data-ttu-id="f24f8-126">Диапазоны</span><span class="sxs-lookup"><span data-stu-id="f24f8-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="f24f8-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="f24f8-127">Remarks</span></span>

<span data-ttu-id="f24f8-128">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="f24f8-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f24f8-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="f24f8-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f24f8-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f24f8-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f24f8-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f24f8-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f24f8-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f24f8-132">Schema name</span></span>  <br/> |<span data-ttu-id="f24f8-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f24f8-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="f24f8-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f24f8-134">Validation file</span></span>  <br/> |<span data-ttu-id="f24f8-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="f24f8-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f24f8-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f24f8-136">Can be empty</span></span>  <br/> ||
   

