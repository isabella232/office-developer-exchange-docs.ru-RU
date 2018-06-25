---
title: UniqueBody
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UniqueBody
api_type:
- schema
ms.assetid: 06bc95d7-121c-433b-bd27-c2b0eb8c011f
description: Элемент UniqueBody представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.
ms.openlocfilehash: 49d3607926e0b985074d79cde76cad084f537f01
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840277"
---
# <a name="uniquebody"></a><span data-ttu-id="17aa6-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="17aa6-103">UniqueBody</span></span>

<span data-ttu-id="17aa6-104">Элемент **UniqueBody** представляет фрагмент HTML или обычный текст, который представляет уникальное body эту беседу.</span><span class="sxs-lookup"><span data-stu-id="17aa6-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="17aa6-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="17aa6-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="17aa6-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="17aa6-106">Attributes and elements</span></span>

<span data-ttu-id="17aa6-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="17aa6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="17aa6-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="17aa6-108">Attributes</span></span>

|<span data-ttu-id="17aa6-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="17aa6-109">**Attribute**</span></span>|<span data-ttu-id="17aa6-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17aa6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17aa6-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="17aa6-111">**BodyType**</span></span> <br/> |<span data-ttu-id="17aa6-112">Описание хранения основной текст элемента в элементе.</span><span class="sxs-lookup"><span data-stu-id="17aa6-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="17aa6-113">Атрибут типа текста сообщения</span><span class="sxs-lookup"><span data-stu-id="17aa6-113">BodyType Attribute</span></span>

|<span data-ttu-id="17aa6-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="17aa6-114">**Value**</span></span>|<span data-ttu-id="17aa6-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17aa6-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="17aa6-116">**HTML-КОД**</span><span class="sxs-lookup"><span data-stu-id="17aa6-116">**HTML**</span></span> <br/> |<span data-ttu-id="17aa6-117">Преобразует все тексты в HTML-код.</span><span class="sxs-lookup"><span data-stu-id="17aa6-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="17aa6-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="17aa6-118">**Text**</span></span> <br/> |<span data-ttu-id="17aa6-119">Преобразует все тексты в обычный текст.</span><span class="sxs-lookup"><span data-stu-id="17aa6-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="17aa6-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="17aa6-120">Child elements</span></span>

<span data-ttu-id="17aa6-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="17aa6-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="17aa6-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="17aa6-122">Parent elements</span></span>

|<span data-ttu-id="17aa6-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="17aa6-123">**Element**</span></span>|<span data-ttu-id="17aa6-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="17aa6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="17aa6-125">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="17aa6-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="17aa6-126">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-127">Контакт</span><span class="sxs-lookup"><span data-stu-id="17aa6-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="17aa6-128">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-129">DistributionList</span><span class="sxs-lookup"><span data-stu-id="17aa6-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="17aa6-130">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="17aa6-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-131">Элемент</span><span class="sxs-lookup"><span data-stu-id="17aa6-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="17aa6-132">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-133">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="17aa6-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="17aa6-134">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-135">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="17aa6-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="17aa6-136">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-137">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="17aa6-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="17aa6-138">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-139">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="17aa6-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="17aa6-140">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-141">Message</span><span class="sxs-lookup"><span data-stu-id="17aa6-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="17aa6-142">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-143">PostItem</span><span class="sxs-lookup"><span data-stu-id="17aa6-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="17aa6-144">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="17aa6-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="17aa6-146">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="17aa6-147">Задача</span><span class="sxs-lookup"><span data-stu-id="17aa6-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="17aa6-148">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="17aa6-149">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="17aa6-149">Text value</span></span>

<span data-ttu-id="17aa6-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="17aa6-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="17aa6-151">Замечания</span><span class="sxs-lookup"><span data-stu-id="17aa6-151">Remarks</span></span>

<span data-ttu-id="17aa6-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="17aa6-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="17aa6-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="17aa6-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="17aa6-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="17aa6-154">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="17aa6-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="17aa6-155">Schema Name</span></span>  <br/> |<span data-ttu-id="17aa6-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="17aa6-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="17aa6-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="17aa6-157">Validation File</span></span>  <br/> |<span data-ttu-id="17aa6-158">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="17aa6-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="17aa6-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="17aa6-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="17aa6-160">False</span><span class="sxs-lookup"><span data-stu-id="17aa6-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="17aa6-161">См. также</span><span class="sxs-lookup"><span data-stu-id="17aa6-161">See also</span></span>



- [<span data-ttu-id="17aa6-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="17aa6-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

