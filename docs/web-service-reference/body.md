---
title: Body
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7851ea9b-9f87-4adc-a26f-7a27df4a9bca
description: Элемент Body указывает текст элемента.
ms.openlocfilehash: a4803c0e5ac3b027396983a5524241590eac35f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761583"
---
# <a name="body"></a><span data-ttu-id="242b2-103">Основной текст</span><span class="sxs-lookup"><span data-stu-id="242b2-103">Body</span></span>

<span data-ttu-id="242b2-104">Элемент **Body** указывает текст элемента.</span><span class="sxs-lookup"><span data-stu-id="242b2-104">The **Body** element specifies the body of an item.</span></span> 
  
```XML
<Body> BodyType="" IsTruncated="" </Body>
```

 <span data-ttu-id="242b2-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="242b2-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="242b2-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="242b2-106">Attributes and elements</span></span>

<span data-ttu-id="242b2-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="242b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="242b2-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="242b2-108">Attributes</span></span>

|<span data-ttu-id="242b2-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="242b2-109">**Attribute**</span></span>|<span data-ttu-id="242b2-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="242b2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="242b2-111">BodyType</span><span class="sxs-lookup"><span data-stu-id="242b2-111">BodyType</span></span>  <br/> |<span data-ttu-id="242b2-112">Указывает тип основного текста.</span><span class="sxs-lookup"><span data-stu-id="242b2-112">Specifies the type of the body.</span></span>  <br/> |
|<span data-ttu-id="242b2-113">Усечено</span><span class="sxs-lookup"><span data-stu-id="242b2-113">IsTruncated</span></span>  <br/> |<span data-ttu-id="242b2-114">Логическое значение, указывающее, обрезается ли текст сообщения.</span><span class="sxs-lookup"><span data-stu-id="242b2-114">Boolean value that indicates whether the body is truncated.</span></span>  <br/> |
   
#### <a name="bodytype"></a><span data-ttu-id="242b2-115">BodyType</span><span class="sxs-lookup"><span data-stu-id="242b2-115">BodyType</span></span>

|<span data-ttu-id="242b2-116">**Значение**</span><span class="sxs-lookup"><span data-stu-id="242b2-116">**Value**</span></span>|<span data-ttu-id="242b2-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="242b2-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="242b2-118">HTML</span><span class="sxs-lookup"><span data-stu-id="242b2-118">HTML</span></span>  <br/> |<span data-ttu-id="242b2-119">Указывает, что текст находится в HTML-коде.</span><span class="sxs-lookup"><span data-stu-id="242b2-119">Indicates that the body is in HTML.</span></span>  <br/> |
|<span data-ttu-id="242b2-120">Текст</span><span class="sxs-lookup"><span data-stu-id="242b2-120">Text</span></span>  <br/> |<span data-ttu-id="242b2-121">Указывает, что текст находится в тексте.</span><span class="sxs-lookup"><span data-stu-id="242b2-121">Indicates that the body is in text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="242b2-122">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="242b2-122">Child elements</span></span>

<span data-ttu-id="242b2-123">Нет.</span><span class="sxs-lookup"><span data-stu-id="242b2-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="242b2-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="242b2-124">Parent elements</span></span>

|<span data-ttu-id="242b2-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="242b2-125">**Element**</span></span>|<span data-ttu-id="242b2-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="242b2-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="242b2-127">календаритем</span><span class="sxs-lookup"><span data-stu-id="242b2-127">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="242b2-128">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-128">Represents an Exchange calendar item.</span></span>  <br/> |
|<span data-ttu-id="242b2-129">[контакт](contact.md);</span><span class="sxs-lookup"><span data-stu-id="242b2-129">[Contact](contact.md)</span></span> <br/> |<span data-ttu-id="242b2-130">Представляет элемент контакта в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-130">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="242b2-131">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="242b2-131">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="242b2-132">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="242b2-132">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="242b2-133">Элемент</span><span class="sxs-lookup"><span data-stu-id="242b2-133">Item</span></span>](item.md) <br/> |<span data-ttu-id="242b2-134">Представляет общий элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-134">Represents a generic item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="242b2-135">Сообщение</span><span class="sxs-lookup"><span data-stu-id="242b2-135">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="242b2-136">Представляет сообщение электронной почты Microsoft Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-136">Represents a Microsoft Exchange email message.</span></span>  <br/> |
|[<span data-ttu-id="242b2-137">PostItem</span><span class="sxs-lookup"><span data-stu-id="242b2-137">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="242b2-138">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-138">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="242b2-139">Задача</span><span class="sxs-lookup"><span data-stu-id="242b2-139">Task</span></span>](task.md) <br/> |<span data-ttu-id="242b2-140">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-140">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="242b2-141">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="242b2-141">Text value</span></span>

<span data-ttu-id="242b2-142">Текстовое значение элемента **Body** — это содержимое тела элемента.</span><span class="sxs-lookup"><span data-stu-id="242b2-142">The text value of the **Body** element is the body content of the item.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="242b2-143">Примечания</span><span class="sxs-lookup"><span data-stu-id="242b2-143">Remarks</span></span>

<span data-ttu-id="242b2-144">Этот элемент появился в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="242b2-144">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="242b2-145">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="242b2-145">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="242b2-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="242b2-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="242b2-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="242b2-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="242b2-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="242b2-148">Schema Name</span></span>  <br/> |<span data-ttu-id="242b2-149">Схема типа</span><span class="sxs-lookup"><span data-stu-id="242b2-149">Type schema</span></span>  <br/> |
|<span data-ttu-id="242b2-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="242b2-150">Validation File</span></span>  <br/> |<span data-ttu-id="242b2-151">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="242b2-151">types.xsd</span></span>  <br/> |
|<span data-ttu-id="242b2-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="242b2-152">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="242b2-153">См. также</span><span class="sxs-lookup"><span data-stu-id="242b2-153">See also</span></span>



- [<span data-ttu-id="242b2-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="242b2-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

