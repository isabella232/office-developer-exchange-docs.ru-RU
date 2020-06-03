---
title: рекуррингмастеритемидранжес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c9c89b5-4ce8-437b-a332-fa7ed35c8388
description: Элемент Рекуррингмастеритемидранжес указывает массив диапазонов вхождений.
ms.openlocfilehash: 784676844c5c58c65b8cc6177843bf26d351b7d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528757"
---
# <a name="recurringmasteritemidranges"></a><span data-ttu-id="9fa15-103">рекуррингмастеритемидранжес</span><span class="sxs-lookup"><span data-stu-id="9fa15-103">RecurringMasterItemIdRanges</span></span>

<span data-ttu-id="9fa15-104">Элемент **рекуррингмастеритемидранжес** указывает массив диапазонов вхождений.</span><span class="sxs-lookup"><span data-stu-id="9fa15-104">The **RecurringMasterItemIdRanges** element specifies an array of occurrence ranges.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="9fa15-105">**рекуррингмастеритемидранжестипе**</span><span class="sxs-lookup"><span data-stu-id="9fa15-105">**RecurringMasterItemIdRangesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fa15-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9fa15-106">Attributes and elements</span></span>

<span data-ttu-id="9fa15-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9fa15-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fa15-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9fa15-108">Attributes</span></span>

|<span data-ttu-id="9fa15-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="9fa15-109">**Attribute**</span></span>|<span data-ttu-id="9fa15-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9fa15-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9fa15-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="9fa15-111">**Id**</span></span> <br/> |<span data-ttu-id="9fa15-112">Текстовое значение атрибута **ID** — это уникальный идентификатор повторяющегося элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="9fa15-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="9fa15-113">Это **строковое** значение.</span><span class="sxs-lookup"><span data-stu-id="9fa15-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="9fa15-114">**чанжекэй**</span><span class="sxs-lookup"><span data-stu-id="9fa15-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="9fa15-115">Текстовое значение атрибута **чанжекэй** является ключом повторяющегося изменения элемента шаблона.</span><span class="sxs-lookup"><span data-stu-id="9fa15-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="9fa15-116">Это **строковое** значение.</span><span class="sxs-lookup"><span data-stu-id="9fa15-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9fa15-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9fa15-117">Child elements</span></span>

[<span data-ttu-id="9fa15-118">Ranges</span><span class="sxs-lookup"><span data-stu-id="9fa15-118">Ranges</span></span>](ranges.md)
  
### <a name="parent-elements"></a><span data-ttu-id="9fa15-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9fa15-119">Parent elements</span></span>

<span data-ttu-id="9fa15-120">[Итемидс](itemids.md)  |  [Глобалитемидс](globalitemids.md)  |  [Драфтитемидс](draftitemids.md)  |  [Контактидс](contactids.md)  |  [Граупидс](groupids.md)</span><span class="sxs-lookup"><span data-stu-id="9fa15-120">[ItemIds](itemids.md) | [GlobalItemIds](globalitemids.md) | [DraftItemIds](draftitemids.md) | [ContactIds](contactids.md) | [GroupIds](groupids.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9fa15-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="9fa15-121">Remarks</span></span>

<span data-ttu-id="9fa15-122">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="9fa15-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9fa15-123">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="9fa15-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fa15-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="9fa15-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fa15-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="9fa15-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fa15-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="9fa15-126">Schema name</span></span>  <br/> |<span data-ttu-id="9fa15-127">Схема Types</span><span class="sxs-lookup"><span data-stu-id="9fa15-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9fa15-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="9fa15-128">Validation file</span></span>  <br/> |<span data-ttu-id="9fa15-129">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="9fa15-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fa15-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="9fa15-130">Can be empty</span></span>  <br/> ||
   

