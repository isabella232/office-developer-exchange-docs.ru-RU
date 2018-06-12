---
title: GetConversationItems operation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: Найдите сведения о GetConversationItems операции.
ms.openlocfilehash: 9d9fb9cc04bcbb5846162c77c852defa51dff98b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762730"
---
# <a name="getconversationitems-operation"></a><span data-ttu-id="e36ef-103">GetConversationItems operation</span><span class="sxs-lookup"><span data-stu-id="e36ef-103">GetConversationItems operation</span></span>

<span data-ttu-id="e36ef-104">Найдите сведения о **GetConversationItems** операции.</span><span class="sxs-lookup"><span data-stu-id="e36ef-104">Find information about the **GetConversationItems** operation.</span></span> 
  
<span data-ttu-id="e36ef-105">Операция **GetConversationItems** получает один или несколько наборов элементов, упорядоченных в узлы в беседе.</span><span class="sxs-lookup"><span data-stu-id="e36ef-105">The **GetConversationItems** operation gets one or more sets of items that are organized in to nodes in a conversation.</span></span> 
  
<span data-ttu-id="e36ef-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="e36ef-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getconversationitems-operation"></a><span data-ttu-id="e36ef-107">С помощью операции GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="e36ef-107">Using the GetConversationItems operation</span></span>

<span data-ttu-id="e36ef-108">Получение элементов беседы, как основной и архивные почтовые ящики, можно использовать операцию **GetConversationItems** .</span><span class="sxs-lookup"><span data-stu-id="e36ef-108">You can use the **GetConversationItems** operation to get items in conversations for both primary and archive mailboxes.</span></span> 
  
### <a name="getconversationitems-operation-soap-headers"></a><span data-ttu-id="e36ef-109">Заголовки SOAP GetConversationItems операции</span><span class="sxs-lookup"><span data-stu-id="e36ef-109">GetConversationItems operation SOAP headers</span></span>

<span data-ttu-id="e36ef-110">Операция **GetConversationItems** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="e36ef-110">The **GetConversationItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e36ef-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="e36ef-111">**Header name**</span></span>|<span data-ttu-id="e36ef-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e36ef-112">**Element**</span></span>|<span data-ttu-id="e36ef-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e36ef-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e36ef-114">**Олицетворение**</span><span class="sxs-lookup"><span data-stu-id="e36ef-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="e36ef-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e36ef-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e36ef-116">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="e36ef-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="e36ef-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="e36ef-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e36ef-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e36ef-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e36ef-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e36ef-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e36ef-120">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="e36ef-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e36ef-121">Минимальное значение для этого элемента — **Exchange2013**.</span><span class="sxs-lookup"><span data-stu-id="e36ef-121">The minimum value for this element is **Exchange2013**.</span></span> <span data-ttu-id="e36ef-122">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="e36ef-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e36ef-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e36ef-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e36ef-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e36ef-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e36ef-125">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="e36ef-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e36ef-126">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="e36ef-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a><span data-ttu-id="e36ef-127">Пример запроса GetConversationItems операции: получение элементов разговора</span><span class="sxs-lookup"><span data-stu-id="e36ef-127">GetConversationItems operation request example: Get items in a single conversation</span></span>

<span data-ttu-id="e36ef-128">Приведенный ниже запрос операции **GetConversationItems** показано, как получить все элементы беседы разговора, за исключением элементы, расположенные в удаленных элементов и папок «черновики».</span><span class="sxs-lookup"><span data-stu-id="e36ef-128">The following example of a **GetConversationItems** operation request shows how to get all conversation items in a single conversation, with the exception of items located in the Deleted Items and Drafts folders.</span></span> <span data-ttu-id="e36ef-129">Каждого элемента, возвращаемого в ответе будет содержать идентификатор элемента, тему и время получения элемента в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="e36ef-129">Each item returned in the response will contain an item identifier, a subject, and the time that the item was received in the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e36ef-130">Все идентификаторы элементов и ключей изменения в этой статье URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="e36ef-130">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e36ef-131">В этом примере запрос **GetConversationItems** не включает следующие параметры:</span><span class="sxs-lookup"><span data-stu-id="e36ef-131">This example of a **GetConversationItems** request does not include the following options:</span></span> 
  
- <span data-ttu-id="e36ef-132">Элемент [MaxItemsToReturn](maxitemstoreturn.md) , который задает максимальное число элементов, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="e36ef-132">The [MaxItemsToReturn](maxitemstoreturn.md) element, which sets the maximum number of items to return in the response.</span></span> 
    
- <span data-ttu-id="e36ef-133">Элемент [MailboxScope](mailboxscope.md) , который задает область почтовых ящиков с, указывающее, является ли операция **GetConversationItems** выполняется на основной почтовый ящик, архивного почтового ящика или обеих почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="e36ef-133">The [MailboxScope](mailboxscope.md) element, which sets the mailbox scope by indicating whether the **GetConversationItems** operation is to be performed on the primary mailbox, the archive mailbox, or both mailboxes.</span></span> 
    
- <span data-ttu-id="e36ef-134">Элемент [состояние (base64Binary)](syncstate-base64binary.md) , который задает состояние синхронизации только получение элементов беседы, которые являются новыми или обновленными в окне беседы.</span><span class="sxs-lookup"><span data-stu-id="e36ef-134">The [SyncState (base64Binary)](syncstate-base64binary.md) element, which sets the synchronization state to only get conversation items that are new or updated in the conversation.</span></span> <span data-ttu-id="e36ef-135">Этот элемент имеет значение для каждого беседы.</span><span class="sxs-lookup"><span data-stu-id="e36ef-135">This element is set for each conversation.</span></span> 
    
<span data-ttu-id="e36ef-136">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e36ef-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e36ef-137">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="e36ef-137">GetConversationItems</span></span>](getconversationitems.md)
    
- [<span data-ttu-id="e36ef-138">ItemShape</span><span class="sxs-lookup"><span data-stu-id="e36ef-138">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="e36ef-139">BaseShape</span><span class="sxs-lookup"><span data-stu-id="e36ef-139">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="e36ef-140">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="e36ef-140">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="e36ef-141">FieldURI</span><span class="sxs-lookup"><span data-stu-id="e36ef-141">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="e36ef-142">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="e36ef-142">FoldersToIgnore</span></span>](folderstoignore.md)
    
- [<span data-ttu-id="e36ef-143">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="e36ef-143">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="e36ef-144">SortOrder (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="e36ef-144">SortOrder (ConversationNodeSortOrder)</span></span>](sortorder-conversationnodesortorder.md)
    
- [<span data-ttu-id="e36ef-145">Conversations</span><span class="sxs-lookup"><span data-stu-id="e36ef-145">Conversations</span></span>](conversations-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e36ef-146">Беседы (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="e36ef-146">Conversation (ConversationRequestType)</span></span>](conversation-conversationrequesttype.md)
    
- [<span data-ttu-id="e36ef-147">ConversationId</span><span class="sxs-lookup"><span data-stu-id="e36ef-147">ConversationId</span></span>](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a><span data-ttu-id="e36ef-148">Успешные операции ответа GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="e36ef-148">Successful GetConversationItems operation response</span></span>

<span data-ttu-id="e36ef-149">В следующем примере показано успешного ответа на запрос операции **GetConversationItems** для получения элементов разговора.</span><span class="sxs-lookup"><span data-stu-id="e36ef-149">The following example shows a successful response to a **GetConversationItems** operation request to get items in a single conversation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e36ef-150">Рекомендуется сохранять состояние для последующих запросов **GetConversationItems** операции.</span><span class="sxs-lookup"><span data-stu-id="e36ef-150">We recommend that you save the SyncState for subsequent **GetConversationItems** operation requests.</span></span> 
  
<span data-ttu-id="e36ef-151">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="e36ef-151">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e36ef-152">GetConversationItemsResponse</span><span class="sxs-lookup"><span data-stu-id="e36ef-152">GetConversationItemsResponse</span></span>](getconversationitemsresponse.md)
    
- [<span data-ttu-id="e36ef-153">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e36ef-153">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e36ef-154">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e36ef-154">GetConversationItemsResponseMessage</span></span>](getconversationitemsresponsemessage.md)
    
- [<span data-ttu-id="e36ef-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e36ef-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e36ef-156">Беседы (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="e36ef-156">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md)
    
- [<span data-ttu-id="e36ef-157">ConversationId</span><span class="sxs-lookup"><span data-stu-id="e36ef-157">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="e36ef-158">Состояние (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="e36ef-158">SyncState (base64Binary)</span></span>](syncstate-base64binary.md)
    
- [<span data-ttu-id="e36ef-159">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="e36ef-159">ConversationNodes</span></span>](conversationnodes.md)
    
- [<span data-ttu-id="e36ef-160">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="e36ef-160">ConversationNode</span></span>](conversationnode.md)
    
- [<span data-ttu-id="e36ef-161">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="e36ef-161">InternetMessageId</span></span>](internetmessageid.md)
    
- [<span data-ttu-id="e36ef-162">Элементы (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="e36ef-162">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="e36ef-163">Message</span><span class="sxs-lookup"><span data-stu-id="e36ef-163">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="e36ef-164">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="e36ef-164">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="e36ef-165">Subject</span><span class="sxs-lookup"><span data-stu-id="e36ef-165">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="e36ef-166">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="e36ef-166">DateTimeReceived</span></span>](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a><span data-ttu-id="e36ef-167">Ошибка операции GetConversationItems ответа</span><span class="sxs-lookup"><span data-stu-id="e36ef-167">GetConversationItems operation error response</span></span>

<span data-ttu-id="e36ef-168">В следующем примере показано возврату ошибки на запрос операции **GetConversationItems** для получения элементов в беседе, либо больше не существует в почтовом ящике, или для которого всех элементов беседы, находятся в папках, которые игнорируются.</span><span class="sxs-lookup"><span data-stu-id="e36ef-168">The following example shows an error response to a **GetConversationItems** operation request to get items in a conversation that either no longer exists in the mailbox, or for which all the conversation items are located in folders that are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="e36ef-169">См. также</span><span class="sxs-lookup"><span data-stu-id="e36ef-169">See also</span></span>

- [<span data-ttu-id="e36ef-170">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e36ef-170">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="e36ef-171">Операция ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="e36ef-171">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
    
- [<span data-ttu-id="e36ef-172">FindConversation Operation</span><span class="sxs-lookup"><span data-stu-id="e36ef-172">FindConversation operation</span></span>](findconversation-operation.md)
    
