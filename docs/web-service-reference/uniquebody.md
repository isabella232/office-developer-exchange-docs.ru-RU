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
description: Элемент UniqueBody представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.
ms.openlocfilehash: 0a8d52c7d4eb8bda9fd41c4c25e448523185df93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461921"
---
# <a name="uniquebody"></a><span data-ttu-id="79b2b-103">UniqueBody</span><span class="sxs-lookup"><span data-stu-id="79b2b-103">UniqueBody</span></span>

<span data-ttu-id="79b2b-104">Элемент **UniqueBody** представляет фрагмент HTML или обычный текст, представляющий уникальный основной текст этой беседы.</span><span class="sxs-lookup"><span data-stu-id="79b2b-104">The **UniqueBody** element represents an HTML fragment or plain text which represents the unique body of this conversation.</span></span> 
  
```XML
<UniqueBody BodyType=""/>
```

 <span data-ttu-id="79b2b-105">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="79b2b-105">**BodyType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="79b2b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="79b2b-106">Attributes and elements</span></span>

<span data-ttu-id="79b2b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="79b2b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79b2b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="79b2b-108">Attributes</span></span>

|<span data-ttu-id="79b2b-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="79b2b-109">**Attribute**</span></span>|<span data-ttu-id="79b2b-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79b2b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79b2b-111">**BodyType**</span><span class="sxs-lookup"><span data-stu-id="79b2b-111">**BodyType**</span></span> <br/> |<span data-ttu-id="79b2b-112">Описывает, как основной текст элемента хранится в элементе.</span><span class="sxs-lookup"><span data-stu-id="79b2b-112">Describes how the item body is stored in the item.</span></span>  <br/> |
   
#### <a name="bodytype-attribute"></a><span data-ttu-id="79b2b-113">Атрибут BodyType</span><span class="sxs-lookup"><span data-stu-id="79b2b-113">BodyType Attribute</span></span>

|<span data-ttu-id="79b2b-114">**Значение**</span><span class="sxs-lookup"><span data-stu-id="79b2b-114">**Value**</span></span>|<span data-ttu-id="79b2b-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79b2b-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="79b2b-116">**HTML**</span><span class="sxs-lookup"><span data-stu-id="79b2b-116">**HTML**</span></span> <br/> |<span data-ttu-id="79b2b-117">Преобразует все тексты в HTML.</span><span class="sxs-lookup"><span data-stu-id="79b2b-117">Converts all bodies to HTML.</span></span>  <br/> |
|<span data-ttu-id="79b2b-118">**Text**</span><span class="sxs-lookup"><span data-stu-id="79b2b-118">**Text**</span></span> <br/> |<span data-ttu-id="79b2b-119">Преобразует все тексты в обычный текст.</span><span class="sxs-lookup"><span data-stu-id="79b2b-119">Converts all bodies to plain text.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="79b2b-120">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="79b2b-120">Child elements</span></span>

<span data-ttu-id="79b2b-121">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="79b2b-121">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79b2b-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="79b2b-122">Parent elements</span></span>

|<span data-ttu-id="79b2b-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="79b2b-123">**Element**</span></span>|<span data-ttu-id="79b2b-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79b2b-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79b2b-125">календаритем</span><span class="sxs-lookup"><span data-stu-id="79b2b-125">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="79b2b-126">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-126">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-127">Контакт</span><span class="sxs-lookup"><span data-stu-id="79b2b-127">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="79b2b-128">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-128">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-129">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="79b2b-129">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="79b2b-130">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="79b2b-130">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-131">Элемент</span><span class="sxs-lookup"><span data-stu-id="79b2b-131">Item</span></span>](item.md) <br/> |<span data-ttu-id="79b2b-132">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-132">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-133">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="79b2b-133">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="79b2b-134">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-134">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-135">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="79b2b-135">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="79b2b-136">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-136">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-137">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="79b2b-137">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="79b2b-138">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-138">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-139">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="79b2b-139">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="79b2b-140">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-140">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-141">Message</span><span class="sxs-lookup"><span data-stu-id="79b2b-141">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="79b2b-142">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-142">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-143">PostItem</span><span class="sxs-lookup"><span data-stu-id="79b2b-143">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="79b2b-144">Представляет элемент POST в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-144">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-145">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="79b2b-145">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="79b2b-146">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-146">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="79b2b-147">Задача</span><span class="sxs-lookup"><span data-stu-id="79b2b-147">Task</span></span>](task.md) <br/> |<span data-ttu-id="79b2b-148">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-148">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79b2b-149">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="79b2b-149">Text value</span></span>

<span data-ttu-id="79b2b-150">Нет.</span><span class="sxs-lookup"><span data-stu-id="79b2b-150">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79b2b-151">Примечания</span><span class="sxs-lookup"><span data-stu-id="79b2b-151">Remarks</span></span>

<span data-ttu-id="79b2b-152">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="79b2b-152">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="79b2b-153">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="79b2b-153">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="79b2b-154">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="79b2b-154">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="79b2b-155">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="79b2b-155">Schema Name</span></span>  <br/> |<span data-ttu-id="79b2b-156">Схема Types</span><span class="sxs-lookup"><span data-stu-id="79b2b-156">Types schema</span></span>  <br/> |
|<span data-ttu-id="79b2b-157">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="79b2b-157">Validation File</span></span>  <br/> |<span data-ttu-id="79b2b-158">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="79b2b-158">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="79b2b-159">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="79b2b-159">Can be Empty</span></span>  <br/> |<span data-ttu-id="79b2b-160">False</span><span class="sxs-lookup"><span data-stu-id="79b2b-160">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="79b2b-161">См. также</span><span class="sxs-lookup"><span data-stu-id="79b2b-161">See also</span></span>



- [<span data-ttu-id="79b2b-162">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="79b2b-162">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

