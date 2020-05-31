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
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761812"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="674f8-103">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="674f8-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="674f8-104">Элемент **CONVERSATION** представляет одну беседу.</span><span class="sxs-lookup"><span data-stu-id="674f8-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="674f8-105">финдконверсатионреспонсе</span><span class="sxs-lookup"><span data-stu-id="674f8-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="674f8-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="674f8-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="674f8-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="674f8-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
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

 <span data-ttu-id="674f8-108">**конверсатионтипе**</span><span class="sxs-lookup"><span data-stu-id="674f8-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="674f8-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="674f8-109">Attributes and elements</span></span>

<span data-ttu-id="674f8-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="674f8-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="674f8-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="674f8-111">Attributes</span></span>

<span data-ttu-id="674f8-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="674f8-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="674f8-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="674f8-113">Child elements</span></span>

|<span data-ttu-id="674f8-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="674f8-114">**Element**</span></span>|<span data-ttu-id="674f8-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="674f8-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="674f8-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="674f8-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="674f8-117">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="674f8-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="674f8-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="674f8-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="674f8-119">Представляет раздел "Беседа".</span><span class="sxs-lookup"><span data-stu-id="674f8-119">Represents the conversation topic.</span></span> <span data-ttu-id="674f8-120">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="674f8-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="674f8-121">уникуереЦипиентс</span><span class="sxs-lookup"><span data-stu-id="674f8-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="674f8-122">Содержит список получателей беседы, собранные из определенной папки.</span><span class="sxs-lookup"><span data-stu-id="674f8-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="674f8-123">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="674f8-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="674f8-124">глобалуникуереЦипиентс</span><span class="sxs-lookup"><span data-stu-id="674f8-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="674f8-125">Содержит список получателей беседы, собранные по почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="674f8-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="674f8-126">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="674f8-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="674f8-127">уникуеунреадсендерс</span><span class="sxs-lookup"><span data-stu-id="674f8-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="674f8-128">Содержит список всех пользователей, которые отправили сообщения, которые в настоящее время не прочитаны в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="674f8-129">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="674f8-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="674f8-130">глобалуникуеунреадсендерс</span><span class="sxs-lookup"><span data-stu-id="674f8-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="674f8-131">Содержит список всех пользователей, которые отправили сообщение, непрочтенное в этой беседе, во всех папках почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="674f8-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-132">уникуесендерс</span><span class="sxs-lookup"><span data-stu-id="674f8-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="674f8-133">Содержит список всех отправителей элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="674f8-134">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="674f8-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="674f8-135">глобалуникуесендерс</span><span class="sxs-lookup"><span data-stu-id="674f8-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="674f8-136">Содержит список всех отправителей элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-137">ластделиверитиме</span><span class="sxs-lookup"><span data-stu-id="674f8-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="674f8-138">Содержит время доставки сообщения, которое было последний раз получено в этой беседе в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-139">глобалластделиверитиме</span><span class="sxs-lookup"><span data-stu-id="674f8-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="674f8-140">Содержит время доставки сообщения, которое было последний раз получено в этой беседе, во всех папках почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="674f8-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-141">Категории</span><span class="sxs-lookup"><span data-stu-id="674f8-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="674f8-142">Содержит коллекцию строк, определяющих категории, которые применяются ко всем элементам бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-143">глобалкатегориес</span><span class="sxs-lookup"><span data-stu-id="674f8-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="674f8-144">Содержит список категорий для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="674f8-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="674f8-146">Содержит сводный статус флага для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-147">глобалфлагстатус</span><span class="sxs-lookup"><span data-stu-id="674f8-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="674f8-148">Содержит сводный статус флага для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="674f8-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="674f8-150">Содержит значение, указывающее, есть ли вложение по крайней мере для одного элемента беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="674f8-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="674f8-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="674f8-152">Содержит значение, указывающее, имеет ли хотя бы один элемент в почтовом ящике вложение.</span><span class="sxs-lookup"><span data-stu-id="674f8-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="674f8-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="674f8-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="674f8-154">Содержит общее число элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-155">глобалмессажекаунт</span><span class="sxs-lookup"><span data-stu-id="674f8-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="674f8-156">Содержит общее число элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-157">унреадкаунт</span><span class="sxs-lookup"><span data-stu-id="674f8-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="674f8-158">Содержит число непрочитанных элементов беседы в папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-159">глобалунреадкаунт</span><span class="sxs-lookup"><span data-stu-id="674f8-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="674f8-160">Содержит количество всех непрочтенных элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-161">Размер</span><span class="sxs-lookup"><span data-stu-id="674f8-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="674f8-162">Содержит размер беседы, рассчитанный на основе размера всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-163">глобалсизе</span><span class="sxs-lookup"><span data-stu-id="674f8-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="674f8-164">Содержит размер диалога, рассчитанный на основе размера всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-165">Итемклассес (Аррайофитемкласстипе)</span><span class="sxs-lookup"><span data-stu-id="674f8-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="674f8-166">Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-167">глобалитемклассес</span><span class="sxs-lookup"><span data-stu-id="674f8-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="674f8-168">Содержит список классов элементов, которые представляют все классы элементов для элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-169">Importance</span><span class="sxs-lookup"><span data-stu-id="674f8-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="674f8-170">Содержит совокупную важность для всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-171">глобалимпортанце</span><span class="sxs-lookup"><span data-stu-id="674f8-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="674f8-172">Содержит совокупную важность для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="674f8-173">итемидс</span><span class="sxs-lookup"><span data-stu-id="674f8-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="674f8-174">Содержит коллекцию идентификаторов элементов для всех элементов бесед в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="674f8-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="674f8-175">глобалитемидс</span><span class="sxs-lookup"><span data-stu-id="674f8-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="674f8-176">Содержит коллекцию идентификаторов элементов для всех элементов бесед в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="674f8-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="674f8-177">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="674f8-177">Parent elements</span></span>

|<span data-ttu-id="674f8-178">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="674f8-178">**Element**</span></span>|<span data-ttu-id="674f8-179">**Описание**</span><span class="sxs-lookup"><span data-stu-id="674f8-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="674f8-180">Беседы</span><span class="sxs-lookup"><span data-stu-id="674f8-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="674f8-181">Содержит массив бесед, возвращаемых в ответе **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="674f8-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="674f8-182">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="674f8-182">Text value</span></span>

<span data-ttu-id="674f8-183">Нет.</span><span class="sxs-lookup"><span data-stu-id="674f8-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="674f8-184">Примечания</span><span class="sxs-lookup"><span data-stu-id="674f8-184">Remarks</span></span>

<span data-ttu-id="674f8-185">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="674f8-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="674f8-186">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="674f8-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="674f8-187">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="674f8-187">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="674f8-188">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="674f8-188">Schema name</span></span>  <br/> |<span data-ttu-id="674f8-189">Схема Types</span><span class="sxs-lookup"><span data-stu-id="674f8-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="674f8-190">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="674f8-190">Validation file</span></span>  <br/> |<span data-ttu-id="674f8-191">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="674f8-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="674f8-192">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="674f8-192">Can be empty</span></span>  <br/> |<span data-ttu-id="674f8-193">False</span><span class="sxs-lookup"><span data-stu-id="674f8-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="674f8-194">См. также</span><span class="sxs-lookup"><span data-stu-id="674f8-194">See also</span></span>



[<span data-ttu-id="674f8-195">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="674f8-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="674f8-196">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="674f8-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="674f8-197">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="674f8-197">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

