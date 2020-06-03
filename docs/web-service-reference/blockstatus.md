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
ms.openlocfilehash: e88236274bfa70216e872025c2a94231f837df1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462278"
---
# <a name="blockstatus"></a><span data-ttu-id="657b4-103">блоккстатус</span><span class="sxs-lookup"><span data-stu-id="657b4-103">BlockStatus</span></span>

<span data-ttu-id="657b4-104">Элемент **блоккстатус** указывает состояние блокировки элемента.</span><span class="sxs-lookup"><span data-stu-id="657b4-104">The **BlockStatus** element specifies the block status of an item.</span></span> 
  
```XML
<BlockStatus> true | false </BlockStatus
```

 <span data-ttu-id="657b4-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="657b4-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="657b4-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="657b4-106">Attributes and elements</span></span>

<span data-ttu-id="657b4-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="657b4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="657b4-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="657b4-108">Attributes</span></span>

<span data-ttu-id="657b4-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="657b4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="657b4-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="657b4-110">Child elements</span></span>

<span data-ttu-id="657b4-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="657b4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="657b4-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="657b4-112">Parent elements</span></span>

|<span data-ttu-id="657b4-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="657b4-113">**Element**</span></span>|<span data-ttu-id="657b4-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="657b4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="657b4-115">календаритем</span><span class="sxs-lookup"><span data-stu-id="657b4-115">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="657b4-116">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="657b4-116">Represents an Exchange calendar item.</span></span>  <br/> |
|<span data-ttu-id="657b4-117">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="657b4-117">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="657b4-118">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="657b4-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="657b4-119">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="657b4-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="657b4-120">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="657b4-120">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="657b4-121">Ресурс</span><span class="sxs-lookup"><span data-stu-id="657b4-121">Item</span></span>](item.md) <br/> |<span data-ttu-id="657b4-122">Представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="657b4-122">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="657b4-123">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="657b4-123">Text value</span></span>

<span data-ttu-id="657b4-124">Текстовое значение **true** для элемента **блоккстатус** указывает на то, что элемент заблокирован.</span><span class="sxs-lookup"><span data-stu-id="657b4-124">A text value of **true** for the **BlockStatus** element indicates that an item is blocked.</span></span> <span data-ttu-id="657b4-125">Значение **false** указывает на то, что элемент не блокируется.</span><span class="sxs-lookup"><span data-stu-id="657b4-125">A value of **false** indicates that an item is not blocked.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="657b4-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="657b4-126">Remarks</span></span>

<span data-ttu-id="657b4-127">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="657b4-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="657b4-128">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="657b4-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="657b4-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="657b4-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="657b4-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="657b4-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="657b4-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="657b4-131">Schema Name</span></span>  <br/> |<span data-ttu-id="657b4-132">Схема типа</span><span class="sxs-lookup"><span data-stu-id="657b4-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="657b4-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="657b4-133">Validation File</span></span>  <br/> |<span data-ttu-id="657b4-134">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="657b4-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="657b4-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="657b4-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="657b4-136">См. также</span><span class="sxs-lookup"><span data-stu-id="657b4-136">See also</span></span>



- [<span data-ttu-id="657b4-137">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="657b4-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

