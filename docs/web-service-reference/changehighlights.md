---
title: чанжехигхлигхтс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f9bd7323-44db-4d2f-aaaa-94c2dfdeead6
description: Элемент Чанжехигхлигхтс указывает, что изменилось между двумя версиями сообщения с приглашением на собрание.
ms.openlocfilehash: 5fe7aa95f60ae95f1af24e8f7a0463ad49716f65
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761675"
---
# <a name="changehighlights"></a><span data-ttu-id="22087-103">чанжехигхлигхтс</span><span class="sxs-lookup"><span data-stu-id="22087-103">ChangeHighlights</span></span>

<span data-ttu-id="22087-104">Элемент **чанжехигхлигхтс** указывает, что изменилось между двумя версиями сообщения с приглашением на собрание.</span><span class="sxs-lookup"><span data-stu-id="22087-104">The **ChangeHighlights** element specifies what has changed between two versions of a meeting request message.</span></span> 
  
```XML
<ChangeHighlights>
    <HasLocationChanged></HasLocationChanged>
    <Location></Location>
    <HasStartTimeChanged></HasStartTimeChanged>
    <Start></Start>
    <HasEndTimeChanged></HasEndTimeChanged>
    <End></End>
</ChangeHighlights>
```

 <span data-ttu-id="22087-105">**чанжехигхлигхтстипе**</span><span class="sxs-lookup"><span data-stu-id="22087-105">**ChangeHighlightsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="22087-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="22087-106">Attributes and elements</span></span>

<span data-ttu-id="22087-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="22087-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="22087-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="22087-108">Attributes</span></span>

<span data-ttu-id="22087-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="22087-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="22087-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="22087-110">Child elements</span></span>

|<span data-ttu-id="22087-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22087-111">**Element**</span></span>|<span data-ttu-id="22087-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22087-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22087-113">хаслокатиончанжед</span><span class="sxs-lookup"><span data-stu-id="22087-113">HasLocationChanged</span></span>](haslocationchanged.md) <br/> |<span data-ttu-id="22087-114">Указывает, изменилось ли свойство Location на собрании.</span><span class="sxs-lookup"><span data-stu-id="22087-114">Specifies whether the location property of a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="22087-115">Location</span><span class="sxs-lookup"><span data-stu-id="22087-115">Location</span></span>](location.md) <br/> |<span data-ttu-id="22087-116">Представляет место собрания или встречи.</span><span class="sxs-lookup"><span data-stu-id="22087-116">Represents the location of a meeting or appointment.</span></span>  <br/> |
|[<span data-ttu-id="22087-117">хасстарттимечанжед</span><span class="sxs-lookup"><span data-stu-id="22087-117">HasStartTimeChanged</span></span>](hasstarttimechanged.md) <br/> |<span data-ttu-id="22087-118">Указывает, изменилось ли время начала собрания.</span><span class="sxs-lookup"><span data-stu-id="22087-118">Specifies whether the start time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="22087-119">Начало</span><span class="sxs-lookup"><span data-stu-id="22087-119">Start</span></span>](start.md) <br/> |<span data-ttu-id="22087-120">Представляет начало длительности.</span><span class="sxs-lookup"><span data-stu-id="22087-120">Represents the start of a duration.</span></span>  <br/> |
|[<span data-ttu-id="22087-121">хасендтимечанжед</span><span class="sxs-lookup"><span data-stu-id="22087-121">HasEndTimeChanged</span></span>](hasendtimechanged.md) <br/> |<span data-ttu-id="22087-122">Указывает, изменилось ли время окончания собрания.</span><span class="sxs-lookup"><span data-stu-id="22087-122">Specifies whether the end time for a meeting has changed.</span></span>  <br/> |
|[<span data-ttu-id="22087-123">Оканчиваться</span><span class="sxs-lookup"><span data-stu-id="22087-123">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="22087-124">Представляет конец длительности.</span><span class="sxs-lookup"><span data-stu-id="22087-124">Represents the end of a duration.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="22087-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="22087-125">Parent elements</span></span>

|<span data-ttu-id="22087-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="22087-126">**Element**</span></span>|<span data-ttu-id="22087-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="22087-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="22087-128">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="22087-128">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="22087-129">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="22087-129">Represents a meeting request in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="22087-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="22087-130">Remarks</span></span>

<span data-ttu-id="22087-131">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="22087-131">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="22087-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="22087-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="22087-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="22087-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="22087-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="22087-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="22087-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="22087-135">Schema Name</span></span>  <br/> |<span data-ttu-id="22087-136">Схема типа</span><span class="sxs-lookup"><span data-stu-id="22087-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="22087-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="22087-137">Validation File</span></span>  <br/> |<span data-ttu-id="22087-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="22087-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="22087-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="22087-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="22087-140">См. также</span><span class="sxs-lookup"><span data-stu-id="22087-140">See also</span></span>



- [<span data-ttu-id="22087-141">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="22087-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

