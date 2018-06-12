---
title: BlockStatus
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: Элемент BlockStatus указывает состояние блокировки элемента.
ms.openlocfilehash: 5733738d733578c47b849b9d7c62c9b66cd8922e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761573"
---
# <a name="blockstatus"></a><span data-ttu-id="5cc42-103">BlockStatus</span><span class="sxs-lookup"><span data-stu-id="5cc42-103">BlockStatus</span></span>

<span data-ttu-id="5cc42-104">Элемент **BlockStatus** указывает состояние блокировки элемента.</span><span class="sxs-lookup"><span data-stu-id="5cc42-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="5cc42-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5cc42-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cc42-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5cc42-106">Attributes and elements</span></span>

<span data-ttu-id="5cc42-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5cc42-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cc42-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5cc42-108">Attributes</span></span>

<span data-ttu-id="5cc42-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="5cc42-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cc42-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5cc42-110">Child elements</span></span>

<span data-ttu-id="5cc42-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="5cc42-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5cc42-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5cc42-112">Parent elements</span></span>

|<span data-ttu-id="5cc42-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5cc42-113">**Element**</span></span>|<span data-ttu-id="5cc42-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5cc42-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cc42-115">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="5cc42-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5cc42-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cc42-116">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5cc42-117">Контакт</span><span class="sxs-lookup"><span data-stu-id="5cc42-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5cc42-118">Представляет контакт в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cc42-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5cc42-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="5cc42-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5cc42-120">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="5cc42-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5cc42-121">Элемент</span><span class="sxs-lookup"><span data-stu-id="5cc42-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="5cc42-122">Представляет универсальный элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cc42-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5cc42-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5cc42-123">Text value</span></span>

<span data-ttu-id="5cc42-124">Текстовое значение **true** для элемента **BlockStatus** указывает, что элемент заблокирован.</span><span class="sxs-lookup"><span data-stu-id="5cc42-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="5cc42-125">Значение **false** указывает, что элемент не блокируются.</span><span class="sxs-lookup"><span data-stu-id="5cc42-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5cc42-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="5cc42-126">Remarks</span></span>

<span data-ttu-id="5cc42-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5cc42-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5cc42-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5cc42-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cc42-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5cc42-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cc42-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5cc42-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cc42-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5cc42-131">Schema Name</span></span>  <br/> |<span data-ttu-id="5cc42-132">Схема типа</span><span class="sxs-lookup"><span data-stu-id="5cc42-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="5cc42-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5cc42-133">Validation File</span></span>  <br/> |<span data-ttu-id="5cc42-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cc42-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cc42-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5cc42-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5cc42-136">См. также</span><span class="sxs-lookup"><span data-stu-id="5cc42-136">See also</span></span>



- [<span data-ttu-id="5cc42-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5cc42-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

