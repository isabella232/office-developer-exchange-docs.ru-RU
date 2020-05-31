---
title: блоккстатус
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 08556ee9-0923-437c-99a4-bb630f04e973
description: Элемент Блоккстатус указывает состояние блокировки элемента.
ms.openlocfilehash: 5733738d733578c47b849b9d7c62c9b66cd8922e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761573"
---
# <a name="blockstatus"></a><span data-ttu-id="2d43b-103">блоккстатус</span><span class="sxs-lookup"><span data-stu-id="2d43b-103">BlockStatus</span></span>

<span data-ttu-id="2d43b-104">Элемент **блоккстатус** указывает состояние блокировки элемента.</span><span class="sxs-lookup"><span data-stu-id="2d43b-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="2d43b-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="2d43b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d43b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2d43b-106">Attributes and elements</span></span>

<span data-ttu-id="2d43b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2d43b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d43b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2d43b-108">Attributes</span></span>

<span data-ttu-id="2d43b-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d43b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d43b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2d43b-110">Child elements</span></span>

<span data-ttu-id="2d43b-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="2d43b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d43b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2d43b-112">Parent elements</span></span>

|<span data-ttu-id="2d43b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2d43b-113">**Element**</span></span>|<span data-ttu-id="2d43b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2d43b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d43b-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="2d43b-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="2d43b-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d43b-116">Represents an Exchange calendar item.</span></span>  <br/> |
|<span data-ttu-id="2d43b-117">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="2d43b-117">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="2d43b-118">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d43b-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="2d43b-119">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="2d43b-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="2d43b-120">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="2d43b-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="2d43b-121">Элемент</span><span class="sxs-lookup"><span data-stu-id="2d43b-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="2d43b-122">Представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d43b-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d43b-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2d43b-123">Text value</span></span>

<span data-ttu-id="2d43b-124">Текстовое значение **true** для элемента **блоккстатус** указывает на то, что элемент заблокирован.</span><span class="sxs-lookup"><span data-stu-id="2d43b-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="2d43b-125">Значение **false** указывает на то, что элемент не блокируется.</span><span class="sxs-lookup"><span data-stu-id="2d43b-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2d43b-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="2d43b-126">Remarks</span></span>

<span data-ttu-id="2d43b-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="2d43b-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2d43b-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="2d43b-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d43b-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="2d43b-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d43b-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="2d43b-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d43b-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="2d43b-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2d43b-132">Схема типа</span><span class="sxs-lookup"><span data-stu-id="2d43b-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="2d43b-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="2d43b-133">Validation File</span></span>  <br/> |<span data-ttu-id="2d43b-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="2d43b-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d43b-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="2d43b-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2d43b-136">См. также</span><span class="sxs-lookup"><span data-stu-id="2d43b-136">See also</span></span>



- [<span data-ttu-id="2d43b-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="2d43b-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

