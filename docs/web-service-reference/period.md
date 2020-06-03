---
title: Period
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Period
api_type:
- schema
ms.assetid: 2f9cf6af-c531-4d7d-90c9-1a1db504d890
description: Элемент period определяет имя, смещение времени и уникальный идентификатор для определенного этапа часового пояса.
ms.openlocfilehash: a7c36a9de01fd0484a7df75de3b5525992ef7ee7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459723"
---
# <a name="period"></a><span data-ttu-id="b5846-103">Period</span><span class="sxs-lookup"><span data-stu-id="b5846-103">Period</span></span>

<span data-ttu-id="b5846-104">Элемент **period** определяет имя, смещение времени и уникальный идентификатор для определенного этапа часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b5846-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="b5846-105">**периодтипе**</span><span class="sxs-lookup"><span data-stu-id="b5846-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b5846-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b5846-106">Attributes and elements</span></span>

<span data-ttu-id="b5846-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b5846-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b5846-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b5846-108">Attributes</span></span>

|<span data-ttu-id="b5846-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="b5846-109">**Attribute**</span></span>|<span data-ttu-id="b5846-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5846-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b5846-111">Bias</span><span class="sxs-lookup"><span data-stu-id="b5846-111">Bias</span></span>  <br/> |<span data-ttu-id="b5846-112">Значение xs: Duration, представляющее смещение времени относительно времени в формате UTC для точки.</span><span class="sxs-lookup"><span data-stu-id="b5846-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="b5846-113">Имя</span><span class="sxs-lookup"><span data-stu-id="b5846-113">Name</span></span>  <br/> |<span data-ttu-id="b5846-114">Строковое значение, представляющее описательное имя точки.</span><span class="sxs-lookup"><span data-stu-id="b5846-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="b5846-115">Id</span><span class="sxs-lookup"><span data-stu-id="b5846-115">Id</span></span>  <br/> |<span data-ttu-id="b5846-116">Строковое значение, представляющее идентификатор точки.</span><span class="sxs-lookup"><span data-stu-id="b5846-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b5846-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b5846-117">Child elements</span></span>

<span data-ttu-id="b5846-118">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b5846-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b5846-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b5846-119">Parent elements</span></span>

|<span data-ttu-id="b5846-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b5846-120">**Element**</span></span>|<span data-ttu-id="b5846-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b5846-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b5846-122">Periods</span><span class="sxs-lookup"><span data-stu-id="b5846-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="b5846-123">Представляет массив периодов, которые определяют смещение времени на разных стадиях часового пояса.</span><span class="sxs-lookup"><span data-stu-id="b5846-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b5846-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b5846-124">Text value</span></span>

<span data-ttu-id="b5846-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="b5846-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b5846-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="b5846-126">Remarks</span></span>

<span data-ttu-id="b5846-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="b5846-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b5846-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b5846-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b5846-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b5846-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b5846-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b5846-130">Schema Name</span></span>  <br/> |<span data-ttu-id="b5846-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b5846-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="b5846-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b5846-132">Validation File</span></span>  <br/> |<span data-ttu-id="b5846-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b5846-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b5846-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b5846-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="b5846-135">False</span><span class="sxs-lookup"><span data-stu-id="b5846-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b5846-136">См. также</span><span class="sxs-lookup"><span data-stu-id="b5846-136">See also</span></span>



- [<span data-ttu-id="b5846-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="b5846-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

