---
title: Точка
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
description: Элемент периода определяет имя, смещение времени и уникальный идентификатор для конкретного этапа часового пояса.
ms.openlocfilehash: 3b5d5877e6d9baffdfe536a0feec3b25b6d2883f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834726"
---
# <a name="period"></a><span data-ttu-id="1074f-103">Точка</span><span class="sxs-lookup"><span data-stu-id="1074f-103">Period</span></span>

<span data-ttu-id="1074f-104">Элемент **периода** определяет имя, смещение времени и уникальный идентификатор для конкретного этапа часового пояса.</span><span class="sxs-lookup"><span data-stu-id="1074f-104">The **Period** element defines the name, time offset, and unique identifier for a specific stage of the time zone.</span></span> 
  
```xml
<Period Bias="" Name="" Id=""/>
```

 <span data-ttu-id="1074f-105">**PeriodType**</span><span class="sxs-lookup"><span data-stu-id="1074f-105">**PeriodType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1074f-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1074f-106">Attributes and elements</span></span>

<span data-ttu-id="1074f-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1074f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1074f-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1074f-108">Attributes</span></span>

|<span data-ttu-id="1074f-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1074f-109">**Attribute**</span></span>|<span data-ttu-id="1074f-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1074f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1074f-111">Bias</span><span class="sxs-lookup"><span data-stu-id="1074f-111">Bias</span></span>  <br/> |<span data-ttu-id="1074f-112">Значение xs:duration, представляющий смещение времени в формате UTC для периода.</span><span class="sxs-lookup"><span data-stu-id="1074f-112">An xs:duration value that represents the time offset from Coordinated Universal Time (UTC) for the period.</span></span>  <br/> |
|<span data-ttu-id="1074f-113">Имя</span><span class="sxs-lookup"><span data-stu-id="1074f-113">Name</span></span>  <br/> |<span data-ttu-id="1074f-114">Строковое значение, представляющее описательное имя периода.</span><span class="sxs-lookup"><span data-stu-id="1074f-114">A string value that represents the descriptive name of the period.</span></span>  <br/> |
|<span data-ttu-id="1074f-115">Id</span><span class="sxs-lookup"><span data-stu-id="1074f-115">Id</span></span>  <br/> |<span data-ttu-id="1074f-116">Строковое значение, представляющее идентификатор для периода.</span><span class="sxs-lookup"><span data-stu-id="1074f-116">A string value that represents the identifier for the period.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1074f-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1074f-117">Child elements</span></span>

<span data-ttu-id="1074f-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="1074f-118">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1074f-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1074f-119">Parent elements</span></span>

|<span data-ttu-id="1074f-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1074f-120">**Element**</span></span>|<span data-ttu-id="1074f-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1074f-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1074f-122">Периоды</span><span class="sxs-lookup"><span data-stu-id="1074f-122">Periods</span></span>](periods.md) <br/> |<span data-ttu-id="1074f-123">Представляет массив периодов, которые определяют смещение времени на различных этапах часового пояса.</span><span class="sxs-lookup"><span data-stu-id="1074f-123">Represents an array of periods that define the time offset at different stages of the time zone.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1074f-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1074f-124">Text value</span></span>

<span data-ttu-id="1074f-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="1074f-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1074f-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="1074f-126">Remarks</span></span>

<span data-ttu-id="1074f-127">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1074f-127">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1074f-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1074f-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1074f-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1074f-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1074f-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1074f-130">Schema Name</span></span>  <br/> |<span data-ttu-id="1074f-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1074f-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="1074f-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1074f-132">Validation File</span></span>  <br/> |<span data-ttu-id="1074f-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1074f-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1074f-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1074f-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="1074f-135">False</span><span class="sxs-lookup"><span data-stu-id="1074f-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1074f-136">См. также</span><span class="sxs-lookup"><span data-stu-id="1074f-136">See also</span></span>



- [<span data-ttu-id="1074f-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1074f-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

