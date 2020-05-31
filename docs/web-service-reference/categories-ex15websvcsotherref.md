---
title: Категории
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Categories
api_type:
- schema
ms.assetid: d84d4927-b524-4e62-bf3d-1f12fec8c21a
description: Элемент Categories содержит коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.
ms.openlocfilehash: 8f112a9a736ff4f242b9dfb084b3ad7541cc493d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761673"
---
# <a name="categories"></a><span data-ttu-id="3ca47-103">Категории</span><span class="sxs-lookup"><span data-stu-id="3ca47-103">Categories</span></span>

<span data-ttu-id="3ca47-104">Элемент **Categories** содержит коллекцию строк, определяющих категории, к которым относится элемент в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3ca47-104">The **Categories** element contains a collection of strings that identify the categories to which an item in the mailbox belongs.</span></span> 
  
```XML
<Categories>
   <String/>
</Categories>
```

 <span data-ttu-id="3ca47-105">**аррайофстрингстипе**</span><span class="sxs-lookup"><span data-stu-id="3ca47-105">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3ca47-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3ca47-106">Attributes and elements</span></span>

<span data-ttu-id="3ca47-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3ca47-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3ca47-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3ca47-108">Attributes</span></span>

<span data-ttu-id="3ca47-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3ca47-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3ca47-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3ca47-110">Child elements</span></span>

|<span data-ttu-id="3ca47-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3ca47-111">**Element**</span></span>|<span data-ttu-id="3ca47-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3ca47-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ca47-113">Строка</span><span class="sxs-lookup"><span data-stu-id="3ca47-113">String</span></span>](string.md) <br/> |<span data-ttu-id="3ca47-114">Содержит строку, определяющую одну категорию.</span><span class="sxs-lookup"><span data-stu-id="3ca47-114">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3ca47-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3ca47-115">Parent elements</span></span>

|<span data-ttu-id="3ca47-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3ca47-116">**Element**</span></span>|<span data-ttu-id="3ca47-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3ca47-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3ca47-118">Элемент</span><span class="sxs-lookup"><span data-stu-id="3ca47-118">Item</span></span>](item.md) <br/> |<span data-ttu-id="3ca47-119">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-119">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-120">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="3ca47-120">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="3ca47-121">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-121">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-122">Message</span><span class="sxs-lookup"><span data-stu-id="3ca47-122">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3ca47-123">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-123">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-124">Задача</span><span class="sxs-lookup"><span data-stu-id="3ca47-124">Task</span></span>](task.md) <br/> |<span data-ttu-id="3ca47-125">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-125">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-126">календаритем</span><span class="sxs-lookup"><span data-stu-id="3ca47-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="3ca47-127">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-128">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="3ca47-128">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="3ca47-129">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="3ca47-129">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-130">митингмессаже</span><span class="sxs-lookup"><span data-stu-id="3ca47-130">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="3ca47-131">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-131">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-132">Свойство meetingrequest</span><span class="sxs-lookup"><span data-stu-id="3ca47-132">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="3ca47-133">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-133">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-134">митингреспонсе</span><span class="sxs-lookup"><span data-stu-id="3ca47-134">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="3ca47-135">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-135">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-136">митингканцеллатион</span><span class="sxs-lookup"><span data-stu-id="3ca47-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="3ca47-137">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-138">Контакт</span><span class="sxs-lookup"><span data-stu-id="3ca47-138">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="3ca47-139">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-139">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-140">дистрибутионлист</span><span class="sxs-lookup"><span data-stu-id="3ca47-140">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3ca47-141">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="3ca47-141">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-142">Условия</span><span class="sxs-lookup"><span data-stu-id="3ca47-142">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3ca47-143">Представляет условия, которые, если удовлетворены, запускают действия правила для правила.</span><span class="sxs-lookup"><span data-stu-id="3ca47-143">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-144">Исключения</span><span class="sxs-lookup"><span data-stu-id="3ca47-144">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3ca47-145">Представляет все доступные условия исключения правила для правила папки "Входящие".</span><span class="sxs-lookup"><span data-stu-id="3ca47-145">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
|[<span data-ttu-id="3ca47-146">конверсатионактион</span><span class="sxs-lookup"><span data-stu-id="3ca47-146">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="3ca47-147">Содержит одно действие, которое будет применено к одной беседе.</span><span class="sxs-lookup"><span data-stu-id="3ca47-147">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3ca47-148">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3ca47-148">Text value</span></span>

<span data-ttu-id="3ca47-149">Нет.</span><span class="sxs-lookup"><span data-stu-id="3ca47-149">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3ca47-150">Примечания</span><span class="sxs-lookup"><span data-stu-id="3ca47-150">Remarks</span></span>

<span data-ttu-id="3ca47-151">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="3ca47-151">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3ca47-152">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3ca47-152">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3ca47-153">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3ca47-153">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3ca47-154">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3ca47-154">Schema Name</span></span>  <br/> |<span data-ttu-id="3ca47-155">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3ca47-155">Types schema</span></span>  <br/> |
|<span data-ttu-id="3ca47-156">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3ca47-156">Validation File</span></span>  <br/> |<span data-ttu-id="3ca47-157">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3ca47-157">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3ca47-158">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3ca47-158">Can be Empty</span></span>  <br/> |<span data-ttu-id="3ca47-159">False</span><span class="sxs-lookup"><span data-stu-id="3ca47-159">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3ca47-160">См. также</span><span class="sxs-lookup"><span data-stu-id="3ca47-160">See also</span></span>



- [<span data-ttu-id="3ca47-161">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3ca47-161">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

