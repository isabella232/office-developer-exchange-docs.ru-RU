---
title: ConversationId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ConversationId
api_type:
- schema
ms.assetid: d5f1ddb3-9af3-4677-a6ba-111b304a951e
description: Элемент ConversationId содержит идентификатор элемента или беседы.
ms.openlocfilehash: 1f82e6ade60fb70db4a9f026fd72d9f11cc63821
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761814"
---
# <a name="conversationid"></a><span data-ttu-id="5d049-103">ConversationId</span><span class="sxs-lookup"><span data-stu-id="5d049-103">ConversationId</span></span>

<span data-ttu-id="5d049-104">Элемент **ConversationId** содержит идентификатор элемента или беседы.</span><span class="sxs-lookup"><span data-stu-id="5d049-104">The **ConversationId** element contains the identifier of an item or conversation.</span></span> 
  
```XML
<ConversationId Id="" ChangeKey="" />
```

 <span data-ttu-id="5d049-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="5d049-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d049-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5d049-106">Attributes and elements</span></span>

<span data-ttu-id="5d049-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5d049-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d049-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5d049-108">Attributes</span></span>

|<span data-ttu-id="5d049-109">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="5d049-109">**Attribute**</span></span>|<span data-ttu-id="5d049-110">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d049-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5d049-111">
  **Id**</span><span class="sxs-lookup"><span data-stu-id="5d049-111">**Id**</span></span> <br/> |<span data-ttu-id="5d049-112">Идентифицирует определенного элемента в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-112">Identifies a specific item in the Exchange store.</span></span>  <br/> |
|<span data-ttu-id="5d049-113">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="5d049-113">**ChangeKey**</span></span> <br/> | <span data-ttu-id="5d049-114">Идентифицирует определенной версии элемента.</span><span class="sxs-lookup"><span data-stu-id="5d049-114">Identifies a specific version of an item.</span></span> <span data-ttu-id="5d049-115">**ChangeKey** является обязательным для следующих сценариев:</span><span class="sxs-lookup"><span data-stu-id="5d049-115">A **ChangeKey** is required for the following scenarios:</span></span>  <br/><br/><span data-ttu-id="5d049-116">- [UpdateItem](updateitem.md) , которого требует элемент **ChangeKey** Если атрибут **ConflictResolution** имеет значение автоматического разрешения конфликтов.</span><span class="sxs-lookup"><span data-stu-id="5d049-116">- The [UpdateItem](updateitem.md) element requires a **ChangeKey** if the **ConflictResolution** attribute is set to AutoResolve.</span></span> <span data-ttu-id="5d049-117">Автоматическое разрешение — это значение по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5d049-117">AutoResolve is a default value.</span></span> <span data-ttu-id="5d049-118">Если атрибут **ChangeKey** не указан, ответ вернет значение [ResponseCode](responsecode.md) равно **ErrorChangeKeyRequired**.</span><span class="sxs-lookup"><span data-stu-id="5d049-118">If the **ChangeKey** attribute is not included, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorChangeKeyRequired**.</span></span><br/><br/><span data-ttu-id="5d049-119">- Элементы [SendItem](senditem.md), [DeleteItem](deleteitem.md)и [DeleteFolder](deletefolder.md) требуется **ChangeKey** для проверки, является ли операцию будет действовать после последней версии элемента.</span><span class="sxs-lookup"><span data-stu-id="5d049-119">- [SendItem](senditem.md), [DeleteItem](deleteitem.md), and [DeleteFolder](deletefolder.md) elements require a **ChangeKey** to test whether the attempted operation will act upon the most recent version of an item.</span></span> <span data-ttu-id="5d049-120">Если атрибут **ChangeKey** не включен в **ItemId** или **ChangeKey** пуст, ответ вернет значение [ResponseCode](responsecode.md) равно **ErrorStaleObject**.</span><span class="sxs-lookup"><span data-stu-id="5d049-120">If the **ChangeKey** attribute is not included in the **ItemId** or if the **ChangeKey** is empty, the response will return a [ResponseCode](responsecode.md) value equal to **ErrorStaleObject**.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5d049-121">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5d049-121">Child elements</span></span>

<span data-ttu-id="5d049-122">Нет.</span><span class="sxs-lookup"><span data-stu-id="5d049-122">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d049-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5d049-123">Parent elements</span></span>

|<span data-ttu-id="5d049-124">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5d049-124">**Element**</span></span>|<span data-ttu-id="5d049-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5d049-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d049-126">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="5d049-126">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="5d049-127">Представляет элемент календаря Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-127">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5d049-128">Контакт</span><span class="sxs-lookup"><span data-stu-id="5d049-128">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="5d049-129">Представляет элемент контакта Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-129">Represents an Exchange contact item.</span></span>  <br/> |
|[<span data-ttu-id="5d049-130">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="5d049-130">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="5d049-131">Представляет одно действие должен применяться к разговора.</span><span class="sxs-lookup"><span data-stu-id="5d049-131">Represents a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="5d049-132">DistributionList</span><span class="sxs-lookup"><span data-stu-id="5d049-132">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="5d049-133">Представляет список рассылки.</span><span class="sxs-lookup"><span data-stu-id="5d049-133">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="5d049-134">Элемент</span><span class="sxs-lookup"><span data-stu-id="5d049-134">Item</span></span>](item.md) <br/> |<span data-ttu-id="5d049-135">Представляет элемент в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-135">Represents an item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-136">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="5d049-136">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="5d049-137">Представляет отмену собрания в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-137">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-138">MeetingMessage</span><span class="sxs-lookup"><span data-stu-id="5d049-138">MeetingMessage</span></span>](meetingmessage.md) <br/> |<span data-ttu-id="5d049-139">Представляет собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-139">Represents a meeting in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-140">MeetingRequest</span><span class="sxs-lookup"><span data-stu-id="5d049-140">MeetingRequest</span></span>](meetingrequest.md) <br/> |<span data-ttu-id="5d049-141">Представляет приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-141">Represents a meeting request in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-142">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="5d049-142">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="5d049-143">Представляет ответ на приглашение на собрание в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-143">Represents a meeting response in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-144">Message</span><span class="sxs-lookup"><span data-stu-id="5d049-144">Message</span></span>](message-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5d049-145">Представляет сообщение электронной почты Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-145">Represents an Exchange e-mail message.</span></span>  <br/> |
|[<span data-ttu-id="5d049-146">PostItem</span><span class="sxs-lookup"><span data-stu-id="5d049-146">PostItem</span></span>](postitem.md) <br/> |<span data-ttu-id="5d049-147">Представляет элемент post в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-147">Represents a post item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-148">RemoveItem</span><span class="sxs-lookup"><span data-stu-id="5d049-148">RemoveItem</span></span>](removeitem.md) <br/> |<span data-ttu-id="5d049-149">Удаляет элемент из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-149">Removes an item from the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-150">Задача</span><span class="sxs-lookup"><span data-stu-id="5d049-150">Task</span></span>](task.md) <br/> |<span data-ttu-id="5d049-151">Представляет задачу в хранилище Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-151">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="5d049-152">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="5d049-152">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="5d049-153">Представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="5d049-153">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d049-154">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="5d049-154">Text value</span></span>

<span data-ttu-id="5d049-155">Нет.</span><span class="sxs-lookup"><span data-stu-id="5d049-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d049-156">Замечания</span><span class="sxs-lookup"><span data-stu-id="5d049-156">Remarks</span></span>

<span data-ttu-id="5d049-157">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="5d049-157">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d049-158">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="5d049-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d049-159">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="5d049-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5d049-160">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="5d049-160">Schema Name</span></span>  <br/> |<span data-ttu-id="5d049-161">Схема Types</span><span class="sxs-lookup"><span data-stu-id="5d049-161">Types schema</span></span>  <br/> |
|<span data-ttu-id="5d049-162">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="5d049-162">Validation File</span></span>  <br/> |<span data-ttu-id="5d049-163">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5d049-163">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5d049-164">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="5d049-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d049-165">False</span><span class="sxs-lookup"><span data-stu-id="5d049-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d049-166">См. также</span><span class="sxs-lookup"><span data-stu-id="5d049-166">See also</span></span>

- [<span data-ttu-id="5d049-167">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="5d049-167">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="5d049-168">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="5d049-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

