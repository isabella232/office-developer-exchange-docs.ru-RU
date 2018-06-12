---
title: Работа с беседы с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7750528c-acb2-43e5-a1e1-ee201c0e1730
description: Сведения о том, как найти бесед, применить действие к бесед и получение элементов в беседах с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 71ef7674086607e1544111071928f3dd74073a77
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761143"
---
# <a name="work-with-conversations-by-using-ews-in-exchange"></a><span data-ttu-id="83b45-103">Работа с беседы с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-103">Work with conversations by using EWS in Exchange</span></span>

<span data-ttu-id="83b45-104">Сведения о том, как найти бесед, применить действие к бесед и получение элементов в беседах с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-104">Learn about how to find conversations, apply actions to conversations, and get items in conversations by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="83b45-105">В контексте Exchange бесед — это способ группировки и управление связанный набор сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="83b45-105">In the context of Exchange, conversations are a way to group and manage a related set of email messages.</span></span> <span data-ttu-id="83b45-106">Их можно также указать способ просмотра связанных сообщений.</span><span class="sxs-lookup"><span data-stu-id="83b45-106">They can also provide a way to view related messages.</span></span> <span data-ttu-id="83b45-107">Exchange определяется на основе значения **Message-ID** для первого сообщения электронной почты в потоке бесед.</span><span class="sxs-lookup"><span data-stu-id="83b45-107">Exchange defines conversations based on the **Message-ID** value of the first email message in a thread.</span></span> <span data-ttu-id="83b45-108">Все ответы и связанных с ними сообщения ссылаться заголовок исходного сообщения **Идентификатор сообщения** в их **Справочные материалы** и **В-адрес для ответа** заголовков.</span><span class="sxs-lookup"><span data-stu-id="83b45-108">All replies and related messages reference the original message's **Message-ID** header in their **References** and **In-Reply-To** headers.</span></span> 
  
<span data-ttu-id="83b45-109">Кроме того в конверте SOAP для каждого сообщения, полученные в почтовом ящике Exchange задает определенные свойства и элементы.</span><span class="sxs-lookup"><span data-stu-id="83b45-109">Additionally, inside the SOAP envelope, for each message received in a mailbox, Exchange sets specific properties and elements.</span></span>
  
<span data-ttu-id="83b45-110">**В таблице 1. Элементы на все сообщения электронной почты и свойства беседы**</span><span class="sxs-lookup"><span data-stu-id="83b45-110">**Table 1. Conversation properties and elements set on all email messages**</span></span>

|<span data-ttu-id="83b45-111">**Свойство управляемый API EWS**</span><span class="sxs-lookup"><span data-stu-id="83b45-111">**EWS Managed API property**</span></span>|<span data-ttu-id="83b45-112">**Элемент веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="83b45-112">**EWS element**</span></span>|<span data-ttu-id="83b45-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="83b45-113">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="83b45-114">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="83b45-114">ConversationTopic</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-115">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="83b45-115">ConversationTopic</span></span>](http://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |<span data-ttu-id="83b45-116">Содержит нормализованный формы значение темы, заданный для исходного сообщения.</span><span class="sxs-lookup"><span data-stu-id="83b45-116">Contains a normalized form of the subject value that was set on the original message.</span></span> <span data-ttu-id="83b45-117">Это то же, что **Поток раздел** заголовка сообщения.</span><span class="sxs-lookup"><span data-stu-id="83b45-117">This is the same as the **Thread-Topic** message header.</span></span> <span data-ttu-id="83b45-118">Это значение доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83b45-118">This value is read-only.</span></span>  <br/> |
|[<span data-ttu-id="83b45-119">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="83b45-119">ConversationIndex</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-120">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="83b45-120">ConversationIndex</span></span>](http://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |<span data-ttu-id="83b45-121">Представляет положение элемента в окне беседы.</span><span class="sxs-lookup"><span data-stu-id="83b45-121">Represents the position of the item in the conversation.</span></span> <span data-ttu-id="83b45-122">Это то же, что заголовок сообщения **Индекс потока** .</span><span class="sxs-lookup"><span data-stu-id="83b45-122">This is the same as the **Thread-Index** message header.</span></span> <span data-ttu-id="83b45-123">Это значение доступно только для чтения.</span><span class="sxs-lookup"><span data-stu-id="83b45-123">This value is read-only.</span></span>  <br/> |
   
<span data-ttu-id="83b45-124">Exchange применяется такое же значение **ConversationTopic** ответы на первом сообщение, а затем обновляет значение **ConversationIndex** для представления положения сообщения относительно исходного сообщения.</span><span class="sxs-lookup"><span data-stu-id="83b45-124">Exchange applies the same **ConversationTopic** value to replies to the first message and then updates the **ConversationIndex** value to represent the message's position relative to the original message.</span></span> <span data-ttu-id="83b45-125">При изменении темы потока электронной почты Exchange применяется новое значение **ConversationTopic** и новые значения **ConversationIndex** в новую беседу.</span><span class="sxs-lookup"><span data-stu-id="83b45-125">If the subject of the email thread changes, Exchange applies a new **ConversationTopic** value and new **ConversationIndex** values to the new conversation.</span></span> 
  
<span data-ttu-id="83b45-126">**В таблице 2. Управляемый API EWS методы и операции веб-служб Exchange для работы с бесед**</span><span class="sxs-lookup"><span data-stu-id="83b45-126">**Table 2. EWS Managed API methods and EWS operations for working with conversations**</span></span>

|<span data-ttu-id="83b45-127">**Чтобы...**</span><span class="sxs-lookup"><span data-stu-id="83b45-127">**In order to…**</span></span>|<span data-ttu-id="83b45-128">**Используйте этот метод управляемый API EWS или методы**</span><span class="sxs-lookup"><span data-stu-id="83b45-128">**Use this EWS Managed API method or methods**</span></span>|<span data-ttu-id="83b45-129">**Используйте эту операцию EWS**</span><span class="sxs-lookup"><span data-stu-id="83b45-129">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="83b45-130">Поиск бесед</span><span class="sxs-lookup"><span data-stu-id="83b45-130">Find conversations</span></span>  <br/> |[<span data-ttu-id="83b45-131">ExchangeService.FindConversation</span><span class="sxs-lookup"><span data-stu-id="83b45-131">ExchangeService.FindConversation</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-132">FindConversation</span><span class="sxs-lookup"><span data-stu-id="83b45-132">FindConversation</span></span>](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="83b45-133">Применение действия беседы</span><span class="sxs-lookup"><span data-stu-id="83b45-133">Apply conversation actions</span></span>  <br/> |[<span data-ttu-id="83b45-134">Conversation.EnableAlwaysCategorizeItems</span><span class="sxs-lookup"><span data-stu-id="83b45-134">Conversation.EnableAlwaysCategorizeItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwayscategorizeitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-135">Conversation.EnableAlwaysDeleteItems</span><span class="sxs-lookup"><span data-stu-id="83b45-135">Conversation.EnableAlwaysDeleteItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-136">Conversation.EnableAlwaysMoveItems</span><span class="sxs-lookup"><span data-stu-id="83b45-136">Conversation.EnableAlwaysMoveItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversation.enablealwaysmoveitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-137">ExchangeService.CopyItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-137">ExchangeService.CopyItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.copyitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-138">ExchangeService.DeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-138">ExchangeService.DeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.deleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-145">ExchangeService.MoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-145">ExchangeService.MoveItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.moveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-146">ExchangeService.SetFlagStatusForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-146">ExchangeService.SetFlagStatusForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setflagstatusforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-147">ExchangeService.SetReadStateForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-147">ExchangeService.SetReadStateForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.setreadstateforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="83b45-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="83b45-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.setretentionpolicyforitemsinconversations%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-149">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="83b45-149">ApplyConversationAction</span></span>](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="83b45-150">Получение элементов в один или несколько бесед</span><span class="sxs-lookup"><span data-stu-id="83b45-150">Get items in one or more conversations</span></span>  <br/> |[<span data-ttu-id="83b45-151">ExchangeService.GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="83b45-151">ExchangeService.GetConversationItems</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-152">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="83b45-152">GetConversationItems</span></span>](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |

<span data-ttu-id="83b45-153"><a name="bk_findewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-153"></span></span>

## <a name="find-a-conversation-by-using-the-ews-managed-api"></a><span data-ttu-id="83b45-154">Найдите беседы с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-154">Find a conversation by using the EWS Managed API</span></span>

<span data-ttu-id="83b45-155">Беседы можно найти с помощью метода управляемый API EWS [ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="83b45-155">You can find conversations by using the [ExchangeService.FindConversation](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="83b45-156">В этом примере возвращается первые 10 бесед в папке "Входящие", с темой, содержащий слово «новости».</span><span class="sxs-lookup"><span data-stu-id="83b45-156">This example gets the first 10 conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="83b45-157">В примере выводится предметам, время последнего доставки и глобальный уникальный список получателей в окне консоли.</span><span class="sxs-lookup"><span data-stu-id="83b45-157">The example then writes the conversation topic, last delivery time, and global unique recipient list to the console window.</span></span> 
  
<span data-ttu-id="83b45-158">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-158">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void FindConversation(ExchangeService service)
{
    // Create the view of conversations returned in the response. This view will return at most 10 results.
    ConversationIndexedItemView view = new ConversationIndexedItemView(10);
    // Create the query string to search for.
    String queryString = "subject:news";
    // Search the Inbox for conversations and return a results set with the specified view.
    // This method call results in a FindConversation call to EWS. 
    ICollection<Conversation> conversations = service.FindConversation(view, WellKnownFolderName.Inbox, queryString);
    // Examine properties on each conversation returned in the response.
    foreach (Conversation conversation in conversations)
    {
        Console.WriteLine("Conversation Topic: " + conversation.Topic);
        Console.WriteLine("Last Delivered: " + conversation.LastDeliveryTime.ToString());
        ApplyConversationActions(service, conversation);
        foreach (string GlUniqRec in conversation.GlobalUniqueRecipients)
        {
            Console.WriteLine("Global Unique Recipient: " + GlUniqRec);
        }
        Console.WriteLine("");
    }
}
```

<span data-ttu-id="83b45-159"><a name="bk_findews"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-159"></span></span>

## <a name="find-a-conversation-by-using-ews"></a><span data-ttu-id="83b45-160">Найдите беседы с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-160">Find a conversation by using EWS</span></span>

<span data-ttu-id="83b45-161">Беседы можно найти с помощью операции [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="83b45-161">You can find conversations by using the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS operation, as shown in the following example.</span></span> <span data-ttu-id="83b45-162">В этом примере возвращается первых десяти бесед в папке "Входящие", с темой, содержащий слово «новости».</span><span class="sxs-lookup"><span data-stu-id="83b45-162">This example gets the first ten conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="83b45-163">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [поиска беседы](#bk_findewsma).</span><span class="sxs-lookup"><span data-stu-id="83b45-163">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [find a conversation](#bk_findewsma).</span></span>
  
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
    <m:FindConversation>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:QueryString>subject:news</m:QueryString>
    </m:FindConversation>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="83b45-164">Сервер отвечает на запрос **FindConversation** [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** , чтобы указать, что операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="83b45-164">The server responds to the **FindConversation** request with a [FindConversationResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> <span data-ttu-id="83b45-165">Ответ также включает в себя только бесед в почтовый ящик, имеющий темы, которая содержит слово «новости».</span><span class="sxs-lookup"><span data-stu-id="83b45-165">The response also includes the only conversation in the mailbox that has a subject that contains the word "news".</span></span> 
  
<span data-ttu-id="83b45-166">Для удобства чтения элементов **ItemId**, **ChangeKey**и **ConversationId** URL были сокращены.</span><span class="sxs-lookup"><span data-stu-id="83b45-166">The **ItemId**, **ChangeKey**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success"
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <Conversation xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <ConversationId Id="aO2NM+Q=" />
          <ConversationTopic>Today's top news headlines</ConversationTopic>
          <UniqueRecipients>
            <String>Sadie Daniels</String>
          </UniqueRecipients>
          <GlobalUniqueRecipients>
            <String>Sadie Daniels</String>
          </GlobalUniqueRecipients>
          <UniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </UniqueUnreadSenders>
          <GlobalUniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueUnreadSenders>
          <UniqueSenders>
            <String>Ronnie Sturgis</String>
          </UniqueSenders>
          <GlobalUniqueSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueSenders>
          <LastDeliveryTime>2014-02-18T20:42:26Z</LastDeliveryTime>
          <GlobalLastDeliveryTime>2014-02-18T20:42:26Z</GlobalLastDeliveryTime>
          <HasAttachments>false</HasAttachments>
          <GlobalHasAttachments>false</GlobalHasAttachments>
          <MessageCount>1</MessageCount>
          <GlobalMessageCount>1</GlobalMessageCount>
          <UnreadCount>1</UnreadCount>
          <GlobalUnreadCount>1</GlobalUnreadCount>
          <Size>9330</Size>
          <GlobalSize>9330</GlobalSize>
          <ItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </ItemClasses>
          <GlobalItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </GlobalItemClasses>
          <Importance>Normal</Importance>
          <GlobalImportance>Normal</GlobalImportance>
          <ItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </ItemIds>
          <GlobalItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </GlobalItemIds>
          <LastModifiedTime>2014-02-18T20:42:26Z</LastModifiedTime>
          <InstanceKey>AQAAAAAAAQABAAAACbFYggAAAAA=</InstanceKey>
          <HasIrm>false</HasIrm>
          <GlobalHasIrm>false</GlobalHasIrm>
        </Conversation>
      </Conversations>
      <TotalConversationsInView>1</TotalConversationsInView>
      <IndexedOffset>1</IndexedOffset>
    </FindConversationResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="83b45-167"><a name="bk_applyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-167"></span></span>

## <a name="apply-conversation-actions-by-using-the-ews-managed-api"></a><span data-ttu-id="83b45-168">Применение действия беседы с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-168">Apply conversation actions by using the EWS Managed API</span></span>

<span data-ttu-id="83b45-169">Можно применить действия беседы принять участие в беседе с помощью ряд методов управляемый API веб-служб Exchange, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="83b45-169">You can apply conversation actions to a conversation by using a number of EWS Managed API methods, as shown in the following example.</span></span> <span data-ttu-id="83b45-170">В этом примере добавляется категорий для существующих элементов в беседе и применение одной категории для будущих элементов в окне беседы.</span><span class="sxs-lookup"><span data-stu-id="83b45-170">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="83b45-171">Также показано, как включить автоматическое перемещение элементов в окне беседы в папке.</span><span class="sxs-lookup"><span data-stu-id="83b45-171">It also shows how to enable the automatic moving of items in the conversation to a folder.</span></span> <span data-ttu-id="83b45-172">В этом примере элементы перемещаются в папку «Черновики».</span><span class="sxs-lookup"><span data-stu-id="83b45-172">In this example, items are moved to the Drafts folder.</span></span>
  
<span data-ttu-id="83b45-173">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-173">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
<span data-ttu-id="83b45-174">Полный список методов, которые применяются действия беседы см в таблице 2.</span><span class="sxs-lookup"><span data-stu-id="83b45-174">For a complete list of methods that apply conversation actions, see Table 2.</span></span>
  
```cs
static void ApplyConversationActions(ExchangeService service, Conversation conversation)
{
   // Create a list of categories to apply to a conversation.
   List<string> categories = new List<string>();
   categories.Add("Customer");
   categories.Add("System Integrator");
   // Apply categorization to all items in the conversation and process the request
   // synchronously after enabling this rule and after all item categorization has been applied. 
   // This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysCategorizeItems(categories, true);
   // Apply an always move rule to all items in the conversation and move the items
   // to the Drafts folder. Process the request asynchronously and return the response. 
   // immediately. This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysMoveItems(WellKnownFolderName.Drafts, false);
}

```

<span data-ttu-id="83b45-175"><a name="bk_applyews"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-175"></span></span>

## <a name="apply-conversation-actions-by-using-ews"></a><span data-ttu-id="83b45-176">Применение действия беседы с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-176">Apply conversation actions by using EWS</span></span>

<span data-ttu-id="83b45-177">Можно применить действия беседы, таких как распределить по категориям, удаление и перемещение, с помощью операции [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) , как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="83b45-177">You can apply conversation actions, such as categorize, delete, and move, by using the [ApplyConversationAction](http://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) operation, as shown in the following example.</span></span> <span data-ttu-id="83b45-178">В этом примере добавляется категорий для существующих элементов в беседе и применение одной категории для будущих элементов в окне беседы.</span><span class="sxs-lookup"><span data-stu-id="83b45-178">This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation.</span></span> <span data-ttu-id="83b45-179">Также показано, как включить автоматическое перемещение элементов в окне беседы в папке; в этом примере элементы перемещаются в папку «Черновики».</span><span class="sxs-lookup"><span data-stu-id="83b45-179">It also shows how to enable the automatic moving of items in the conversation to a folder; in this example, items are moved to the Drafts folder.</span></span> <span data-ttu-id="83b45-180">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [применения действия беседы](#bk_applyewsma).</span><span class="sxs-lookup"><span data-stu-id="83b45-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [apply conversation actions](#bk_applyewsma).</span></span>
  
<span data-ttu-id="83b45-181">Элемент **ConversationId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="83b45-181">The **ConversationId** element has been shortened for readability.</span></span> 
  
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
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="jG6WVpg=" />
          <t:ProcessRightAway>false</t:ProcessRightAway>
          <t:DestinationFolderId>
            <t:DistinguishedFolderId Id="drafts" />
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="83b45-182">Сервер отвечает на запрос **ApplyConversationAction** [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** , чтобы указать, что операция выполнена успешно.</span><span class="sxs-lookup"><span data-stu-id="83b45-182">The server responds to the **ApplyConversationAction** request with a [ApplyConversationActionResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> 

<span data-ttu-id="83b45-183"><a name="bk_getitemssingleewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-183"></span></span>

## <a name="get-items-in-a-single-conversation-by-using-the-conversation-identifier-in-the-ews-managed-api"></a><span data-ttu-id="83b45-184">Получение элементов разговора с помощью идентификатора сообщений в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-184">Get items in a single conversation by using the conversation identifier in the EWS Managed API</span></span>

<span data-ttu-id="83b45-185">Можно получить элементов в беседе с помощью метода [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-185">You can get items in a conversation by using the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="83b45-186">В этом примере предоставляет набор узлов беседы для первого беседы в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="83b45-186">This example provides the set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="83b45-187">Идентификатор элемента, теме и время получения для каждого элемента возвращаемого в ответе, наряду с беседы индекса и родительский беседы индекс свойства.</span><span class="sxs-lookup"><span data-stu-id="83b45-187">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="83b45-188">Можно использовать свойства index беседы для восстановления иерархии узла.</span><span class="sxs-lookup"><span data-stu-id="83b45-188">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="83b45-189">В этом примере все элементы беседы в удаленных элементов и Черновики папок по умолчанию игнорируются.</span><span class="sxs-lookup"><span data-stu-id="83b45-189">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="83b45-190">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-190">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsSingleConversation(ExchangeService service)
{
   try
   {
      // Find the first item in the mailbox.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox,
                                                         new ItemView(1));
      // Get the conversation identifier of the item. 
      ConversationId convId = results.Items[0].ConversationId;
      // Specify the properties that will be 
      // returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ConversationResponse response = service.GetConversationItems(convId,
                                                   properties,
                                                  null,
                                                  foldersToIgnore,
                                                  ConversationSortOrder.TreeOrderDescending);
      // Get the synchronization state of the conversation.
      Console.WriteLine("SyncState: " + response.SyncState);
      Collection<Item> items = new Collection<Item>();
      // Process each node of conversation items.
      foreach (ConversationNode node in response.ConversationNodes)
      {
         Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
         Console.WriteLine("Conversation index: " + node.ConversationIndex);
         Console.WriteLine("Conversation node items:");
         // Process each item in the conversation node.
         foreach (Item item in node.Items)
         {
            Console.WriteLine("   Item ID: " + item.Id.UniqueId);
            Console.WriteLine("   Subject: " + item.Subject);
            Console.WriteLine("   Received: " + item.DateTimeReceived);
            items.Add(item);
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   {
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="83b45-191">Мы рекомендуем кэшировании свойство **состояние** для последующих запросов для получения элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="83b45-191">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="83b45-192"><a name="bk_getitemsmanyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-192"></span></span>

## <a name="get-items-in-many-conversations-by-using-the-conversationrequest-object-in-the-ews-managed-api"></a><span data-ttu-id="83b45-193">Получение элементов в много беседы с помощью объекта ConversationRequest в управляемый API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-193">Get items in many conversations by using the ConversationRequest object in the EWS Managed API</span></span>

<span data-ttu-id="83b45-194">Объект [ConversationRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) и метод управляемый API EWS [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) можно использовать для получения элементов из двух или более бесед.</span><span class="sxs-lookup"><span data-stu-id="83b45-194">You can use the [ConversationRequest](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) object and the [ExchangeService.GetConversationItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method to get items from two or more conversations.</span></span> <span data-ttu-id="83b45-195">В этом примере набор узлов беседы для первых двух беседы в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="83b45-195">This example provides a set of conversation nodes for the first two conversations in the Inbox.</span></span> <span data-ttu-id="83b45-196">Идентификатор элемента, темы и время получения для каждого элемента будут возвращены в ответ, наряду с беседы индекса и родительский беседы индекс свойства.</span><span class="sxs-lookup"><span data-stu-id="83b45-196">The item identifier, subject, and the received time for each item will be returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="83b45-197">Можно использовать свойства index беседы для восстановления иерархии узла.</span><span class="sxs-lookup"><span data-stu-id="83b45-197">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> <span data-ttu-id="83b45-198">В этом примере предполагается, что первых двух элементов в папке "Входящие", из различных бесед.</span><span class="sxs-lookup"><span data-stu-id="83b45-198">This example assumes that the first two items in the Inbox are from different conversations.</span></span> 
  
<span data-ttu-id="83b45-199">В этом примере все элементы беседы в удаленных элементов и Черновики папок по умолчанию игнорируются.</span><span class="sxs-lookup"><span data-stu-id="83b45-199">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="83b45-200">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-200">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsManyConversations(ExchangeService service)
{
   try
   {
      // Find the first two items in the Inbox. This item will be used to call the GetConversationItems operation.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox, new ItemView(2));
      // Get the conversation identifier of the first two items in the Inbox. 
      ConversationId convId1 = results.Items[0].ConversationId;
      ConversationId convId2 = results.Items[1].ConversationId;
      
      // Identify two conversation requests. 
      ConversationRequest convR1 = new ConversationRequest();
      convR1.ConversationId = convId1;
      ConversationRequest convR2 = new ConversationRequest();
      convR2.ConversationId = convId2;
      // Create a collection of conversations to fetch. 
      Collection<ConversationRequest> conversations = new Collection<ConversationRequest>();
      conversations.Add(convR1);
      conversations.Add(convR2);
      // Specify the properties that will be returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ServiceResponseCollection<GetConversationItemsResponse> responses = 
          service.GetConversationItems(conversations, properties, foldersToIgnore, 
          ConversationSortOrder.TreeOrderDescending);
      // Process each conversation.
      foreach (GetConversationItemsResponse resp in responses)
      {
         // Identify the synchronization state of the conversation.
         Console.WriteLine("Sync State: " + resp.Conversation.SyncState);
         // Process each node in the conversation.
         foreach (ConversationNode node in resp.Conversation.ConversationNodes)
         {
            Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
            Console.WriteLine("Conversation index: " + node.ConversationIndex);
            Console.WriteLine("Conversation node items:");
            // Process each item in the conversation node.
            foreach (Item item in node.Items)
            {
               Console.WriteLine("   Item ID: " + item.Id.UniqueId);
               Console.WriteLine("   Subject: " + item.Subject);
               Console.WriteLine("   Received: " + item.DateTimeReceived);
            }
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   { 
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="83b45-201">Рекомендуется мы рекомендуем возвращения только свойства, которые требуется клиентского приложения, а не с помощью параметра **FirstClassProperties** для класса **BasePropertySet** .</span><span class="sxs-lookup"><span data-stu-id="83b45-201">As a best practice, we recommend that you return only the properties that the client application requires, rather than using the **FirstClassProperties** option for the **BasePropertySet** class.</span></span> <span data-ttu-id="83b45-202">Мы рекомендуем кэшировании свойство **состояние** для последующих запросов для получения элементов в беседе.</span><span class="sxs-lookup"><span data-stu-id="83b45-202">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="83b45-203"><a name="bk_getitemsews"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-203"></span></span>

## <a name="get-items-in-conversations-by-using-the-conversation-identifier-in-ews"></a><span data-ttu-id="83b45-204">Получение элементов в беседах с помощью идентификатора сообщений в веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-204">Get items in conversations by using the conversation identifier in EWS</span></span>

<span data-ttu-id="83b45-205">Можно получить элементов в беседе с помощью операции [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="83b45-205">You can get items in a conversation by using the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="83b45-206">В этом примере набор узлов беседы для первого беседы в папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="83b45-206">This example provides a set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="83b45-207">Идентификатор элемента, теме и время получения для каждого элемента возвращаемого в ответе, наряду с беседы индекса и родительский беседы индекс свойства.</span><span class="sxs-lookup"><span data-stu-id="83b45-207">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="83b45-208">Можно использовать свойства index беседы для восстановления иерархии узла.</span><span class="sxs-lookup"><span data-stu-id="83b45-208">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="83b45-209">В этом примере все элементы беседы в удаленных элементов и Черновики папок по умолчанию игнорируются.</span><span class="sxs-lookup"><span data-stu-id="83b45-209">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="83b45-210">Элемент **ConversationId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="83b45-210">The **ConversationId** element has been shortened for readability.</span></span> 
  
<span data-ttu-id="83b45-211">Получение элементов из нескольких беседы, включите дополнительные элементы **беседы** .</span><span class="sxs-lookup"><span data-stu-id="83b45-211">To get items from more than one conversation, include additional **Conversation** elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m=http://schemas.microsoft.com/exchange/services/2006/messages
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
          <t:ConversationId Id="LUQFH6Q=" />
        </t:Conversation>
      </m:Conversations>
    </m:GetConversationItems>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **GetConversationItems** [GetConversationItemsResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** , чтобы указать, что операция выполнена успешно. <span data-ttu-id="83b45-213">Ответ также включает в себя [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) в окне беседы.</span><span class="sxs-lookup"><span data-stu-id="83b45-213">The response also includes the [ConversationNodes](http://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) in the conversation.</span></span> 
  
<span data-ttu-id="83b45-214">Для удобства чтения элементов **ItemId**, **состояние**и **ConversationId** URL были сокращены.</span><span class="sxs-lookup"><span data-stu-id="83b45-214">The **ItemId**, **SyncState**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="873"
                         MinorBuildNumber="9"
                         Version="V2_9"
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
            <t:ConversationId Id="LUQFH6Q=" />
            <t:SyncState>AAAAYAm1</t:SyncState>
            <t:ConversationNodes>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;994051d7c1a346efbfce8dec2cbad509
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AYB1NAAA="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYCHq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T13:15:00Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;6a8e7658524b41cda7cdc3f23c1074a5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="lQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAu8" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T10:02:08Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96
                    @SN2SR01MB005.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="igAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuj" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T16:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="iwAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAul" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T15:30:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="jQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T14:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="kAAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAux" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T12:52:09Z</t:DateTimeReceived>
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

<span data-ttu-id="83b45-215"><a name="bk_versiondiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="83b45-215"></span></span>

## <a name="version-differences"></a><span data-ttu-id="83b45-216">Различия версий</span><span class="sxs-lookup"><span data-stu-id="83b45-216">Version differences</span></span>

<span data-ttu-id="83b45-217">При использовании Exchange Server 2010 с пакетом обновления 1 (SP1), метод [FindConversation](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) имеет меньшее количество параметров и операции [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) имеет меньшего числа элементов в запросе.</span><span class="sxs-lookup"><span data-stu-id="83b45-217">When you are using Exchange Server 2010 Service Pack 1 (SP1), the [FindConversation](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) method has fewer options available, and the [FindConversation](http://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) operation has fewer elements in the request.</span></span> 
  
<span data-ttu-id="83b45-218">**В таблице 3. Поддержка FindConversation версия Exchange 2010 с пакетом обновления 1**</span><span class="sxs-lookup"><span data-stu-id="83b45-218">**Table 3. Exchange 2010 SP1 version support for FindConversation**</span></span>

|<span data-ttu-id="83b45-219">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="83b45-219">**EWS Managed API method**</span></span>|<span data-ttu-id="83b45-220">**Элементы веб-служб Exchange**</span><span class="sxs-lookup"><span data-stu-id="83b45-220">**EWS elements**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="83b45-221">FindConversation (ViewBase, FolderId)</span><span class="sxs-lookup"><span data-stu-id="83b45-221">FindConversation (ViewBase, FolderId)</span></span>](http://msdn.microsoft.com/en-us/library/office/jj220668%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="83b45-222">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="83b45-222">IndexedPageItemView</span></span>](http://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) <br/> [<span data-ttu-id="83b45-223">SortOrder</span><span class="sxs-lookup"><span data-stu-id="83b45-223">SortOrder</span></span>](http://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) <br/> [<span data-ttu-id="83b45-224">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="83b45-224">ParentFolderId</span></span>](http://msdn.microsoft.com/library/0e3e6e5f-06d0-499b-8ca4-d36036521658%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="83b45-225">Метод управляемый API EWS [GetConversationItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) и операции EWS [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) были представлены в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="83b45-225">The [GetConversationItems](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method and the [GetConversationItems](http://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation were introduced in Exchange Server 2013.</span></span> <span data-ttu-id="83b45-226">Приложения, предназначенные для более ранних версий Exchange может применяться только действия беседы беседы, как показано в таблице 2.</span><span class="sxs-lookup"><span data-stu-id="83b45-226">Applications that target earlier versions of Exchange can only apply conversation actions to conversations, as listed in Table 2.</span></span> 
  
<span data-ttu-id="83b45-227">Управляемый API EWS **FindConversation** метод и метод веб-служб Exchange **FindConversation** не доступна в первоначальной версии Exchange 2010 или в Exchange 2007.</span><span class="sxs-lookup"><span data-stu-id="83b45-227">The **FindConversation** EWS Managed API method and the **FindConversation** EWS method are not available in the initial release version of Exchange 2010 or in Exchange 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="83b45-228">См. также</span><span class="sxs-lookup"><span data-stu-id="83b45-228">See also</span></span>

- [<span data-ttu-id="83b45-229">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-229">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="83b45-230">Используйте фильтры поиска с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="83b45-230">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)   
- [<span data-ttu-id="83b45-231">Exchange 2013: Поиск бесед в почтовых ящиках программными средствами</span><span class="sxs-lookup"><span data-stu-id="83b45-231">Exchange 2013: Find conversations in mailboxes programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Find-d4b6b3af)    
- [<span data-ttu-id="83b45-232">Exchange 2013: Применение действий по управлению бесед в почтовый ящик</span><span class="sxs-lookup"><span data-stu-id="83b45-232">Exchange 2013: Apply actions to manage conversations in a mailbox</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Apply-accde0b5)
    

