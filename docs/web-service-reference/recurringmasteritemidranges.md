---
title: RecurringMasterItemIdRanges
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: Элемент RecurringMasterItemIdRanges указывает массив диапазонов вхождение.
ms.openlocfilehash: 60d987f475bed5d630a1238550e4d14578ebd0d5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835016"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="1a754-103">RecurringMasterItemIdRanges</span><span class="sxs-lookup"><span data-stu-id="1a754-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="1a754-104">Элемент **RecurringMasterItemIdRanges** указывает массив диапазонов вхождение.</span><span class="sxs-lookup"><span data-stu-id="1a754-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="1a754-105">**RecurringMasterItemIdRangesType**</span><span class="sxs-lookup"><span data-stu-id="1a754-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1a754-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1a754-106">Attributes and elements</span></span>

<span data-ttu-id="1a754-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1a754-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1a754-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1a754-108">Attributes</span></span>

|<span data-ttu-id="1a754-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="1a754-109">**Attribute**</span></span>|<span data-ttu-id="1a754-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1a754-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1a754-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="1a754-111">**Id**</span></span> <br/> |<span data-ttu-id="1a754-112">Текстовое значение атрибута **Id** — уникальный идентификатор элемента повторяющихся шаблона.</span><span class="sxs-lookup"><span data-stu-id="1a754-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="1a754-113">Это значение типа **string** .</span><span class="sxs-lookup"><span data-stu-id="1a754-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="1a754-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="1a754-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="1a754-115">Текстовое значение атрибута **ChangeKey** является повторяющейся главной элемент изменить ключ.</span><span class="sxs-lookup"><span data-stu-id="1a754-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="1a754-116">Это значение типа **string** .</span><span class="sxs-lookup"><span data-stu-id="1a754-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1a754-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1a754-117">Child elements</span></span>

[<span data-ttu-id="1a754-118">Диапазоны</span><span class="sxs-lookup"><span data-stu-id="1a754-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="1a754-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1a754-119">Parent elements</span></span>

<span data-ttu-id="1a754-120">[Что ItemID](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="1a754-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1a754-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="1a754-121">Remarks</span></span>

<span data-ttu-id="1a754-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1a754-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1a754-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="1a754-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1a754-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1a754-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1a754-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1a754-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1a754-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1a754-126">Schema name</span></span>  <br/> |<span data-ttu-id="1a754-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="1a754-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="1a754-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1a754-128">Validation file</span></span>  <br/> |<span data-ttu-id="1a754-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="1a754-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1a754-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1a754-130">Can be empty</span></span>  <br/> ||
   

