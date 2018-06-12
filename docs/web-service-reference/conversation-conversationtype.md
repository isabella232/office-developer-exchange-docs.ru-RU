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
description: Элемент Conversation представляет разговора.
ms.openlocfilehash: e1ae055d6a77fc5a9b483341830b978e0c1a5b5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761812"
---
# <a name="conversation-conversationtype"></a><span data-ttu-id="ebe3c-103">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ebe3c-103">Conversation (ConversationType)</span></span>

<span data-ttu-id="ebe3c-104">Элемент **Conversation** представляет разговора.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-104">The **Conversation** element represents a single conversation.</span></span> 
  
[<span data-ttu-id="ebe3c-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="ebe3c-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="ebe3c-106">Conversations</span><span class="sxs-lookup"><span data-stu-id="ebe3c-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="ebe3c-107">Беседы (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="ebe3c-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
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

 <span data-ttu-id="ebe3c-108">**ConversationType**</span><span class="sxs-lookup"><span data-stu-id="ebe3c-108">**ConversationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebe3c-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ebe3c-109">Attributes and elements</span></span>

<span data-ttu-id="ebe3c-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebe3c-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ebe3c-111">Attributes</span></span>

<span data-ttu-id="ebe3c-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebe3c-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ebe3c-113">Child elements</span></span>

|<span data-ttu-id="ebe3c-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ebe3c-114">**Element**</span></span>|<span data-ttu-id="ebe3c-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ebe3c-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebe3c-116">ConversationId</span><span class="sxs-lookup"><span data-stu-id="ebe3c-116">ConversationId</span></span>](conversationid.md) <br/> |<span data-ttu-id="ebe3c-117">Представляет идентификатор беседы.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-117">Represents the identifier of a conversation.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-118">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="ebe3c-118">ConversationTopic</span></span>](conversationtopic.md) <br/> |<span data-ttu-id="ebe3c-119">Представляет раздел беседы.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-119">Represents the conversation topic.</span></span> <span data-ttu-id="ebe3c-120">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-120">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-121">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="ebe3c-121">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="ebe3c-122">Содержит список получателей беседы, собранные из определенной папки.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-122">Contains the recipient list of a conversation aggregated from a particular folder.</span></span> <span data-ttu-id="ebe3c-123">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-123">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-124">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="ebe3c-124">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="ebe3c-125">Содержит список получателей беседы сводный в почтовый ящик.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-125">Contains the recipient list of a conversation aggregated across a mailbox.</span></span> <span data-ttu-id="ebe3c-126">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-126">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-127">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ebe3c-127">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="ebe3c-128">Содержит список всех людей, отправленные сообщения, которые в настоящее время непрочитанные сообщения в эту беседу в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-128">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span> <span data-ttu-id="ebe3c-129">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-129">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-130">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="ebe3c-130">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="ebe3c-131">Содержит список всех людей, отправленные сообщения, в настоящее время непрочитанные сообщения в беседе для всех папок в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-131">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-132">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="ebe3c-132">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="ebe3c-133">Содержит список всех отправителей элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-133">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="ebe3c-134">Этот элемент доступен только для чтения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-134">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-135">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="ebe3c-135">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="ebe3c-136">Содержит список всех отправителей беседы элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-136">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-137">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="ebe3c-137">LastDeliveryTime</span></span>](lastdeliverytime.md) <br/> |<span data-ttu-id="ebe3c-138">Содержит время доставки сообщений, который был получен последний в эту беседу в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-138">Contains the delivery time of the message that was last received in this conversation in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-139">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="ebe3c-139">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md) <br/> |<span data-ttu-id="ebe3c-140">Содержит время доставки сообщений, который был получен последний беседы во всех папках в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-140">Contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-141">Категории</span><span class="sxs-lookup"><span data-stu-id="ebe3c-141">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ebe3c-142">Содержит коллекцию строк, которые определяют категории, которые применяются ко всем элементам беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-142">Contains a collection of strings that identify the categories that are applied to all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-143">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="ebe3c-143">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="ebe3c-144">Содержит список категорий для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-144">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-145">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="ebe3c-145">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="ebe3c-146">Содержит объединенные флаг состояния для элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-146">Contains the aggregated flag status for conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-147">GlobalFlagStatus</span><span class="sxs-lookup"><span data-stu-id="ebe3c-147">GlobalFlagStatus</span></span>](globalflagstatus.md) <br/> |<span data-ttu-id="ebe3c-148">Содержит объединенные флаг состояния всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-148">Contains the aggregated flag status for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-149">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="ebe3c-149">HasAttachments</span></span>](hasattachments.md) <br/> |<span data-ttu-id="ebe3c-150">Содержит значение, указывающее, имеет ли беседы по крайней мере один элемент в текущей папке вложения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-150">Contains a value that indicates whether at least one conversation item in the current folder has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-151">GlobalHasAttachments</span><span class="sxs-lookup"><span data-stu-id="ebe3c-151">GlobalHasAttachments</span></span>](globalhasattachments.md) <br/> |<span data-ttu-id="ebe3c-152">Содержит значение, указывающее на наличие по крайней мере один беседы элемента в почтовом ящике вложения.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-152">Contains a value that indicates whether at least one conversation item in a mailbox has an attachment.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-153">MessageCount</span><span class="sxs-lookup"><span data-stu-id="ebe3c-153">MessageCount</span></span>](messagecount.md) <br/> |<span data-ttu-id="ebe3c-154">Содержит общее число элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-154">Contains the total number of conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-155">GlobalMessageCount</span><span class="sxs-lookup"><span data-stu-id="ebe3c-155">GlobalMessageCount</span></span>](globalmessagecount.md) <br/> |<span data-ttu-id="ebe3c-156">Содержит общее число элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-156">Contains the total number of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-157">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="ebe3c-157">UnreadCount</span></span>](unreadcount.md) <br/> |<span data-ttu-id="ebe3c-158">Содержит число элементов непрочитанных сообщений в папке.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-158">Contains the count of unread conversation items within a folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-159">GlobalUnreadCount</span><span class="sxs-lookup"><span data-stu-id="ebe3c-159">GlobalUnreadCount</span></span>](globalunreadcount.md) <br/> |<span data-ttu-id="ebe3c-160">Содержит все непрочитанные сообщения беседы элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-160">Contains a count of all the unread conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-161">Размер</span><span class="sxs-lookup"><span data-stu-id="ebe3c-161">Size</span></span>](size.md) <br/> |<span data-ttu-id="ebe3c-162">Содержит размер беседы, вычисляемых из размер всех элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-162">Contains the conversation size calculated from the size of all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-163">GlobalSize</span><span class="sxs-lookup"><span data-stu-id="ebe3c-163">GlobalSize</span></span>](globalsize.md) <br/> |<span data-ttu-id="ebe3c-164">Содержит размер беседы, вычисляемых из размер всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-164">Contains the size of the conversation calculated from the size of all conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-165">ItemClasses (ArrayOfItemClassType)</span><span class="sxs-lookup"><span data-stu-id="ebe3c-165">ItemClasses (ArrayOfItemClassType)</span></span>](itemclasses-arrayofitemclasstype.md) <br/> |<span data-ttu-id="ebe3c-166">Содержит список классов элементов, представляющий все классы элементов из элементов беседы в текущей папке.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-166">Contains a list of item classes that represents all the item classes of the conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-167">GlobalItemClasses</span><span class="sxs-lookup"><span data-stu-id="ebe3c-167">GlobalItemClasses</span></span>](globalitemclasses.md) <br/> |<span data-ttu-id="ebe3c-168">Содержит список классов элементов, представляющий все классы элементов беседы элементов в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-168">Contains a list of item classes that represents all the item classes of the conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-169">Важность</span><span class="sxs-lookup"><span data-stu-id="ebe3c-169">Importance</span></span>](importance.md) <br/> |<span data-ttu-id="ebe3c-170">Содержит объединенные важности для всех элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-170">Contains the aggregated importance for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-171">GlobalImportance</span><span class="sxs-lookup"><span data-stu-id="ebe3c-171">GlobalImportance</span></span>](globalimportance.md) <br/> |<span data-ttu-id="ebe3c-172">Содержит объединенные важности для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-172">Contains the aggregated importance for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-173">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="ebe3c-173">ItemIds</span></span>](itemids.md) <br/> |<span data-ttu-id="ebe3c-174">Содержит коллекцию идентификаторов элементов для всех элементов беседы в текущую папку.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-174">Contains the collection of item identifiers for all conversation items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="ebe3c-175">GlobalItemIds</span><span class="sxs-lookup"><span data-stu-id="ebe3c-175">GlobalItemIds</span></span>](globalitemids.md) <br/> |<span data-ttu-id="ebe3c-176">Содержит коллекцию идентификаторов элементов для всех элементов беседы в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-176">Contains the collection of item identifiers for all conversation items in a mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ebe3c-177">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ebe3c-177">Parent elements</span></span>

|<span data-ttu-id="ebe3c-178">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ebe3c-178">**Element**</span></span>|<span data-ttu-id="ebe3c-179">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ebe3c-179">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebe3c-180">Conversations</span><span class="sxs-lookup"><span data-stu-id="ebe3c-180">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ebe3c-181">Содержит массив диалогов, возвращаемого в ответе **FindConversation** .</span><span class="sxs-lookup"><span data-stu-id="ebe3c-181">Contains an array of conversations that are returned in the **FindConversation** response.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ebe3c-182">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ebe3c-182">Text value</span></span>

<span data-ttu-id="ebe3c-183">Нет.</span><span class="sxs-lookup"><span data-stu-id="ebe3c-183">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebe3c-184">Замечания</span><span class="sxs-lookup"><span data-stu-id="ebe3c-184">Remarks</span></span>

<span data-ttu-id="ebe3c-185">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.Этот элемент появился в Exchange Server 2010 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="ebe3c-185">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebe3c-186">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ebe3c-186">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebe3c-187">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ebe3c-187">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebe3c-188">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ebe3c-188">Schema name</span></span>  <br/> |<span data-ttu-id="ebe3c-189">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ebe3c-189">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebe3c-190">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ebe3c-190">Validation file</span></span>  <br/> |<span data-ttu-id="ebe3c-191">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="ebe3c-191">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ebe3c-192">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ebe3c-192">Can be empty</span></span>  <br/> |<span data-ttu-id="ebe3c-193">False</span><span class="sxs-lookup"><span data-stu-id="ebe3c-193">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebe3c-194">См. также</span><span class="sxs-lookup"><span data-stu-id="ebe3c-194">See also</span></span>



[<span data-ttu-id="ebe3c-195">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="ebe3c-195">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="ebe3c-196">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="ebe3c-196">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="ebe3c-197">Conversations in EWS</span><span class="sxs-lookup"><span data-stu-id="ebe3c-197">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

