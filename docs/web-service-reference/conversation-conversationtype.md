---
title: Беседы (ConversationType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Conversation
api_type:
- schema
ms.assetid: 59d014cd-5886-49ea-8d36-ba5de7e675de
description: Элемент CONVERSATION представляет одну беседу.
ms.openlocfilehash: 9969a6cfe1f977b1c24e03771f231f4eb03d1ac6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458938"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="f6beb-103">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f6beb-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="f6beb-104">Элемент **CONVERSATION** представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="f6beb-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="f6beb-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="f6beb-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="f6beb-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="f6beb-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="f6beb-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="f6beb-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
```XML
<Conversation>
   <ConversationId/>
   <ConversationTopic/>
   <UniqueRecipients/>
   <GlobalUniqueRecipients/>
   <UniqueUnreadSenders/>
   <GlobalUniqueUnreadSenders/>
   <UniqueSenders/>
   <GlobalUniqueSenders/>
   <LastDeliveryTime/>
   <GlobalLastDeliveryTime/>
   <Categories/>
   <GlobalCategories/>
   <FlagStatus/>
   <GlobalFlagStatus/>
   <HasAttachments/>
   <GlobalHasAttachments/>
   <MessageCount/>
   <GlobalMessageCount/>
   <UnreadCount/>
   <GlobalUnreadCount/>
   <Size/>   <GlobalSize/>
   <ItemClasses/>
   <GlobalItemClasses/>
   <Importance/>
   <GlobalImportance/>
   <ItemIds/>
   <GlobalItemIds/>
</Conversation>
```

 <span data-ttu-id="f6beb-108">**конверсатионтипе**</span><span class="sxs-lookup"><span data-stu-id="f6beb-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6beb-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f6beb-109">Attributes and elements</span></span>

<span data-ttu-id="f6beb-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f6beb-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6beb-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f6beb-111">Attributes</span></span>

<span data-ttu-id="f6beb-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f6beb-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f6beb-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f6beb-113">Child elements</span></span>

|<span data-ttu-id="f6beb-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6beb-114">**Element**</span></span>|<span data-ttu-id="f6beb-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6beb-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6beb-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="f6beb-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="f6beb-117">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="f6beb-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="f6beb-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="f6beb-119">Представляет раздел "Беседа".</span><span class="sxs-lookup"><span data-stu-id="f6beb-119">Represents the conversation topic.</span></span> <span data-ttu-id="f6beb-120">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6beb-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-121">уникуереЦипиентс</span><span class="sxs-lookup"><span data-stu-id="f6beb-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="f6beb-122">Содержит список получателей беседы, собранные из определенной папки.</span><span class="sxs-lookup"><span data-stu-id="f6beb-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="f6beb-123">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6beb-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-124">глобалуникуереЦипиентс</span><span class="sxs-lookup"><span data-stu-id="f6beb-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="f6beb-125">Содержит список получателей беседы, собранные по почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="f6beb-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="f6beb-126">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6beb-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-127">уникуеунреадсендерс</span><span class="sxs-lookup"><span data-stu-id="f6beb-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="f6beb-128">Содержит список всех пользователей, которые отправили сообщения, которые в настоящее время не прочитаны в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="f6beb-129">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6beb-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-130">глобалуникуеунреадсендерс</span><span class="sxs-lookup"><span data-stu-id="f6beb-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="f6beb-131">Содержит список всех пользователей, которые отправили сообщение, непрочтенное в этой беседе, во всех папках почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f6beb-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-132">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="f6beb-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="f6beb-133">Содержит список всех отправителей элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="f6beb-134">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="f6beb-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-135">глобалуникуесендерс</span><span class="sxs-lookup"><span data-stu-id="f6beb-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="f6beb-136">Содержит список всех отправителей элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-137">ластделиверитиме</span><span class="sxs-lookup"><span data-stu-id="f6beb-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="f6beb-138">Содержит время доставки сообщения, которое было последний раз получено в этой беседе в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-139">глобалластделиверитиме</span><span class="sxs-lookup"><span data-stu-id="f6beb-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="f6beb-140">Содержит время доставки сообщения, которое было последний раз получено в этой беседе, во всех папках почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f6beb-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-141">Категории</span><span class="sxs-lookup"><span data-stu-id="f6beb-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6beb-142">Содержит коллекцию строк, определяющих категории, которые применяются ко всем элементам бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-143">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="f6beb-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="f6beb-144">Содержит список категорий для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="f6beb-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="f6beb-146">Содержит сводный статус флага для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-147">глобалфлагстатус</span><span class="sxs-lookup"><span data-stu-id="f6beb-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="f6beb-148">Содержит сводный статус флага для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="f6beb-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="f6beb-150">Содержит значение, указывающее, есть ли вложение по крайней мере для одного элемента беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="f6beb-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="f6beb-152">Содержит значение, указывающее, имеет ли хотя бы один элемент в почтовом ящике вложение.</span><span class="sxs-lookup"><span data-stu-id="f6beb-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="f6beb-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="f6beb-154">Содержит общее число элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-155">глобалмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="f6beb-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="f6beb-156">Содержит общее число элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-157">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="f6beb-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="f6beb-158">Содержит число непрочитанных элементов беседы в папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-159">глобалунреадкаунт</span><span class="sxs-lookup"><span data-stu-id="f6beb-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="f6beb-160">Содержит количество всех непрочтенных элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-161">Размер</span><span class="sxs-lookup"><span data-stu-id="f6beb-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="f6beb-162">Содержит размер беседы, рассчитанный на основе размера всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-163">глобалсизе</span><span class="sxs-lookup"><span data-stu-id="f6beb-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="f6beb-164">Содержит размер диалога, рассчитанный на основе размера всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-165">Итемклассес (Аррайофитемкласстипе)</span><span class="sxs-lookup"><span data-stu-id="f6beb-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="f6beb-166">Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-167">глобалитемклассес</span><span class="sxs-lookup"><span data-stu-id="f6beb-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="f6beb-168">Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-169">Importance</span><span class="sxs-lookup"><span data-stu-id="f6beb-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="f6beb-170">Содержит совокупную важность для всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-171">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="f6beb-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="f6beb-172">Содержит совокупную важность для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-173">итемидс</span><span class="sxs-lookup"><span data-stu-id="f6beb-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="f6beb-174">Содержит коллекцию идентификаторов элементов для всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="f6beb-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="f6beb-175">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="f6beb-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="f6beb-176">Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="f6beb-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6beb-177">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f6beb-177">Parent elements</span></span>

|<span data-ttu-id="f6beb-178">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f6beb-178">**Element**</span></span>|<span data-ttu-id="f6beb-179">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f6beb-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6beb-180">Беседы</span><span class="sxs-lookup"><span data-stu-id="f6beb-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="f6beb-181">Содержит массив бесед, возвращаемых в ответе **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="f6beb-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f6beb-182">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f6beb-182">Text value</span></span>

<span data-ttu-id="f6beb-183">Нет.</span><span class="sxs-lookup"><span data-stu-id="f6beb-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6beb-184">Примечания</span><span class="sxs-lookup"><span data-stu-id="f6beb-184">Remarks</span></span>

<span data-ttu-id="f6beb-185">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="f6beb-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6beb-186">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f6beb-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6beb-187">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f6beb-187">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f6beb-188">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f6beb-188">Schema name</span></span>  <br/> |<span data-ttu-id="f6beb-189">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f6beb-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="f6beb-190">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f6beb-190">Validation file</span></span>  <br/> |<span data-ttu-id="f6beb-191">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f6beb-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f6beb-192">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f6beb-192">Can be empty</span></span>  <br/> |<span data-ttu-id="f6beb-193">False</span><span class="sxs-lookup"><span data-stu-id="f6beb-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6beb-194">См. также</span><span class="sxs-lookup"><span data-stu-id="f6beb-194">See also</span></span>



[<span data-ttu-id="f6beb-195">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="f6beb-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="f6beb-196">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="f6beb-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="f6beb-197">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="f6beb-197">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

