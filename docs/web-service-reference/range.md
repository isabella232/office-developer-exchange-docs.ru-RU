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
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465312"
---
# <a name="range"></a><span data-ttu-id="c5b3b-103">Диапазон</span><span class="sxs-lookup"><span data-stu-id="c5b3b-103">Range</span></span>

<span data-ttu-id="c5b3b-104">Элемент **Range** указывает диапазон вхождений элемента календаря для повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-104">The **Range** element specifies a range of calendar item occurrences for a repeating calendar item.</span></span> 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 <span data-ttu-id="c5b3b-105">**оккурренцесранжетипе**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-105">**OccurrencesRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c5b3b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c5b3b-106">Attributes and elements</span></span>

<span data-ttu-id="c5b3b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c5b3b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c5b3b-108">Attributes</span></span>

|<span data-ttu-id="c5b3b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-109">**Attribute**</span></span>|<span data-ttu-id="c5b3b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c5b3b-111">**Начало**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-111">**Start**</span></span> <br/> |<span data-ttu-id="c5b3b-112">Текстовое значение **начального** атрибута — Начальная дата диапазона повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-112">The text value of the **Start** attribute is the start date of the recurring item range.</span></span> <span data-ttu-id="c5b3b-113">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="c5b3b-113">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="c5b3b-114">**End**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-114">**End**</span></span> <br/> |<span data-ttu-id="c5b3b-115">Текстовое значение атрибута **End** — конечная дата диапазона повторяющихся элементов.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-115">The text value of the **End** attribute is the end date of the recurring item range.</span></span> <span data-ttu-id="c5b3b-116">Это значение **даты и времени** .</span><span class="sxs-lookup"><span data-stu-id="c5b3b-116">This is a **dateTime** value.</span></span>  <br/> |
|<span data-ttu-id="c5b3b-117">**Count**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-117">**Count**</span></span> <br/> |<span data-ttu-id="c5b3b-118">Текстовое значение атрибута **Count** — это количество повторений повторяющегося элемента.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-118">The text value of the **Count** attribute is the number of occurrences of the recurring item.</span></span> <span data-ttu-id="c5b3b-119">Это **целое** значение.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-119">This is an **integer** value.</span></span>  <br/> |
|<span data-ttu-id="c5b3b-120">**компареоригиналстарттиме**</span><span class="sxs-lookup"><span data-stu-id="c5b3b-120">**CompareOriginalStartTime**</span></span> <br/> |<span data-ttu-id="c5b3b-121">Текстовое значение **true** для атрибута **компареоригиналстарттиме** указывает на то, что клиент должен сравнить исходное время начала с новым временем начала.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-121">The text value of **true** for the **CompareOriginalStartTime** attribute indicates that the client should compare the original start time with the new start time.</span></span> <span data-ttu-id="c5b3b-122">Значение **false** указывает, что клиенту не требуется сравнивать исходное время начала с новым временем начала.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-122">A value of **false** indicates that the client does not need to compare the original start time with the new start time.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c5b3b-123">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c5b3b-123">Child elements</span></span>

<span data-ttu-id="c5b3b-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-124">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c5b3b-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c5b3b-125">Parent elements</span></span>

[<span data-ttu-id="c5b3b-126">Ranges</span><span class="sxs-lookup"><span data-stu-id="c5b3b-126">Ranges</span></span>](ranges.md)
  
## <a name="remarks"></a><span data-ttu-id="c5b3b-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="c5b3b-127">Remarks</span></span>

<span data-ttu-id="c5b3b-128">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-128">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c5b3b-129">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="c5b3b-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c5b3b-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c5b3b-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c5b3b-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c5b3b-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c5b3b-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c5b3b-132">Schema name</span></span>  <br/> |<span data-ttu-id="c5b3b-133">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c5b3b-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="c5b3b-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c5b3b-134">Validation file</span></span>  <br/> |<span data-ttu-id="c5b3b-135">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c5b3b-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c5b3b-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c5b3b-136">Can be empty</span></span>  <br/> ||
   

