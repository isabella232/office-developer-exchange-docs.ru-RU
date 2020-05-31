---
title: Диапазон
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Элемент Range указывает диапазон вхождений элемента календаря для повторяющегося элемента календаря.
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834946"
---
# <a name="range"></a><span data-ttu-id="0a9a1-103">Диапазон</span><span class="sxs-lookup"><span data-stu-id="0a9a1-103">Range</span></span>

<span data-ttu-id="0a9a1-104">Элемент **Range** указывает диапазон вхождений элемента календаря для повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="0a9a1-105">**оккурренцесранжетипе**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0a9a1-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0a9a1-106">Attributes and elements</span></span>

<span data-ttu-id="0a9a1-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a9a1-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0a9a1-108">Attributes</span></span>

|<span data-ttu-id="0a9a1-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-109">**Attribute**</span></span>|<span data-ttu-id="0a9a1-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0a9a1-111">**Начало**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-111">**Start**</span></span> <br/> |<span data-ttu-id="0a9a1-112">Текстовое значение **начального** атрибута — Начальная дата диапазона повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="0a9a1-113">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="0a9a1-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="0a9a1-114">**End**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-114">**End**</span></span> <br/> |<span data-ttu-id="0a9a1-115">Текстовое значение атрибута **End** — конечная дата диапазона повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="0a9a1-116">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="0a9a1-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="0a9a1-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-117">**Count**</span></span> <br/> |<span data-ttu-id="0a9a1-118">Текстовое значение атрибута **Count** — это количество повторений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="0a9a1-119">Это **целое** значение.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="0a9a1-120">**компареоригиналстарттиме**</span><span class="sxs-lookup"><span data-stu-id="0a9a1-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="0a9a1-121">Текстовое значение **true** для атрибута **компареоригиналстарттиме** указывает на то, что клиент должен сравнить исходное время начала с новым временем начала.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="0a9a1-122">Значение **false** указывает, что клиенту не требуется сравнивать исходное время начала с новым временем начала.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0a9a1-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0a9a1-123">Child elements</span></span>

<span data-ttu-id="0a9a1-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a9a1-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0a9a1-125">Parent elements</span></span>

[<span data-ttu-id="0a9a1-126">Ranges</span><span class="sxs-lookup"><span data-stu-id="0a9a1-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="0a9a1-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="0a9a1-127">Remarks</span></span>

<span data-ttu-id="0a9a1-128">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="0a9a1-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="0a9a1-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0a9a1-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0a9a1-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0a9a1-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0a9a1-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0a9a1-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0a9a1-132">Schema name</span></span>  <br/> |<span data-ttu-id="0a9a1-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="0a9a1-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="0a9a1-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0a9a1-134">Validation file</span></span>  <br/> |<span data-ttu-id="0a9a1-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="0a9a1-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0a9a1-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0a9a1-136">Can be empty</span></span>  <br/> ||
   

