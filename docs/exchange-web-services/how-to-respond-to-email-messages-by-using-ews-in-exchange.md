---
title: Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9d584991-4d67-4d36-ae2f-99970af8488f
description: Узнайте, как отвечать на сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 2f1428251084a7f2bf8d589a788c143f34b64d5c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761110"
---
# <a name="respond-to-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="8279c-103">Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-103">Respond to email messages by using EWS in Exchange</span></span>

<span data-ttu-id="8279c-104">Узнайте, как отвечать на сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-104">Learn how to respond to email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="8279c-105">Чтобы ответить на сообщения, отвечая на них или пересылать их получателей можно использовать управляемый API EWS или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-105">You can use the EWS Managed API or EWS to respond to messages by replying to them or forwarding them to recipients.</span></span>
  
<span data-ttu-id="8279c-106">**В таблице 1. Управляемый API EWS методы и операции EWS для ответа на сообщения электронной почты**</span><span class="sxs-lookup"><span data-stu-id="8279c-106">**Table 1. EWS Managed API methods and EWS operations for responding to email messages**</span></span>

|<span data-ttu-id="8279c-107">**Задача**</span><span class="sxs-lookup"><span data-stu-id="8279c-107">**Task**</span></span>|<span data-ttu-id="8279c-108">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="8279c-108">**EWS Managed API method**</span></span>|<span data-ttu-id="8279c-109">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="8279c-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="8279c-110">Ответ на сообщение электронной почты</span><span class="sxs-lookup"><span data-stu-id="8279c-110">Reply to an email message</span></span>  <br/> |[<span data-ttu-id="8279c-111">EmailMessage.Reply</span><span class="sxs-lookup"><span data-stu-id="8279c-111">EmailMessage.Reply</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8279c-112">EmailMessage.CreateReply</span><span class="sxs-lookup"><span data-stu-id="8279c-112">EmailMessage.CreateReply</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8279c-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), где элемент [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) имеет дочерний элемент [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) или [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8279c-113">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of either [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) or [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).</span></span>  <br/> |
|<span data-ttu-id="8279c-114">Пересылать сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="8279c-114">Forward an email message</span></span>  <br/> |[<span data-ttu-id="8279c-115">EmailMessage.Forward</span><span class="sxs-lookup"><span data-stu-id="8279c-115">EmailMessage.Forward</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="8279c-116">EmailMessage.CreateForward</span><span class="sxs-lookup"><span data-stu-id="8279c-116">EmailMessage.CreateForward</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) <br/> |<span data-ttu-id="8279c-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), где элемент [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) имеет дочерний элемент [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8279c-117">[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), where the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element has a child element of [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).</span></span>  <br/> |
   
## <a name="reply-to-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="8279c-118">Ответ на сообщение электронной почты с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-118">Reply to an email message by using the EWS Managed API</span></span>
<span data-ttu-id="8279c-119"><a name="bk_replyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8279c-119"></span></span>

<span data-ttu-id="8279c-120">Управляемый API веб-служб Exchange предоставляет два метода, которые можно использовать для ответа на сообщения: [ответ](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) и [CreateReply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8279c-120">The EWS Managed API provides two methods that you can use to respond to messages: [Reply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) and [CreateReply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="8279c-121">Метод **ответа** только используются два входных параметра: ответное сообщение в начале существующий текст и **логическое** значение, указывающее, является ли ответ должен приходить для всех получателей (true) или просто отправителя (false).</span><span class="sxs-lookup"><span data-stu-id="8279c-121">The **Reply** method only takes two parameters: the response message to prepend to the existing body, and a **Boolean** value that indicates whether the response should go to all recipients (true) or just the sender (false).</span></span> <span data-ttu-id="8279c-122">Если требуется добавить дополнительных получателей на сообщение задавать дополнительные свойства в ответ, или добавить вложение, используйте метод **CreateReply** , который позволяет задать все [первого класса свойства](email-properties-and-elements-in-ews-in-exchange.md) , доступные на [EmailMessage ](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)объект.</span><span class="sxs-lookup"><span data-stu-id="8279c-122">If you need to add additional recipients to a message, set additional properties on a response, or add an attachment, use the **CreateReply** method, which enables you to set all the [first-class properties](email-properties-and-elements-in-ews-in-exchange.md) that are available on an [EmailMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="8279c-123">В следующем примере кода показано, как использовать метод **ответ** в ответ на сообщение электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8279c-123">The following code example shows how to use the **Reply** method to respond to an email message.</span></span> 
  
<span data-ttu-id="8279c-124">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-124">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="8279c-125">Локальной переменной *ItemId* — это [идентификатор](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента реагировать на.</span><span class="sxs-lookup"><span data-stu-id="8279c-125">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to respond to.</span></span> <span data-ttu-id="8279c-126">В примере вызывается [метод FindRecentlySent](#bk_findlast) , чтобы убедиться, что сообщение помечено как ответ.</span><span class="sxs-lookup"><span data-stu-id="8279c-126">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as replied to.</span></span> 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.LastModifiedTime);
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
string myReply = "This is the message body of the email reply.";
bool replyToAll = false;
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Reply(myReply, replyToAll);
// Verify that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="8279c-127">В следующем примере кода показано, как использовать метод **CreateReply** отвечать на сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="8279c-127">The following code example shows how to use the **CreateReply** method to respond to an email message.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
bool replyToAll = true;
ResponseMessage responseMessage = message.CreateReply(replyToAll);
// Prepend the reply to the message body. 
string myReply = "This is the message body of the email reply.";
responseMessage.BodyPrefix = myReply;
// Send the response message.
// This method call results in a CreateItem call to EWS.
responseMessage.SendAndSaveCopy();
// Check that the response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="8279c-128">Если необходимо добавить вложения в сообщении ответа, замените вызов метода **SendAndSaveCopy** следующий код.</span><span class="sxs-lookup"><span data-stu-id="8279c-128">If you need to add an attachment to the response message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage reply = responseMessage.Save();
reply.Attachments.AddFileAttachment("attachmentname.txt");
reply.Update(ConflictResolutionMode.AutoResolve);
reply.SendAndSaveCopy();
```

## <a name="reply-to-an-email-message-by-using-ews"></a><span data-ttu-id="8279c-129">Ответ на сообщение электронной почты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-129">Reply to an email message by using EWS</span></span>
<span data-ttu-id="8279c-130"><a name="bk_replyews"> </a></span><span class="sxs-lookup"><span data-stu-id="8279c-130"></span></span>

<span data-ttu-id="8279c-131">В следующем примере кода показано, как отвечать на сообщения с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-131">The following code example shows how to reply to a message by using EWS.</span></span> <span data-ttu-id="8279c-132">С помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с атрибутом **MessageDisposition** , равным **SendAndSaveCopy** отправлять сообщения и сохранения ответа в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="8279c-132">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="8279c-133">Включить элемент [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) в качестве дочерних [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) элемента ответить всем на сообщение потока или включить элемент [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) отвечать только для отправителя.</span><span class="sxs-lookup"><span data-stu-id="8279c-133">Include either the [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) element as a child of the [Items](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) element to reply to everyone on the message thread, or include the [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) element to reply only to the sender.</span></span> 
  
<span data-ttu-id="8279c-134">Это также XML-запрос, который отправляет управляемый API EWS при вызове [ответ](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) или метод [CreateReply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8279c-134">This is also the XML request that the EWS Managed API sends when calling either the [Reply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) or the [CreateReply](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ReplyAllToItem>
          <t:ReferenceItemId Id="AAMkADE4="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the email reply.</t:NewBodyContent>
        </t:ReplyAllToItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8279c-135">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что ответ был создан и отправлен успешно.</span><span class="sxs-lookup"><span data-stu-id="8279c-135">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the reply was created and sent successfully.</span></span>
  
<span data-ttu-id="8279c-136">Если необходимо добавить вложения в ответное сообщение вызова операции **CreateItem** , как указано выше, но измените **MessageDisposition** на **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="8279c-136">If you need to add an attachment to your response message, call the **CreateItem** operation as specified above, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="8279c-137">Затем вызовите операцию [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , а затем операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8279c-137">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="forward-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="8279c-138">Пересылать сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-138">Forward an email message by using the EWS Managed API</span></span>
<span data-ttu-id="8279c-139"><a name="bk_forwardewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="8279c-139"></span></span>

<span data-ttu-id="8279c-140">Управляемый API веб-служб Exchange предоставляет два метода, которые можно использовать для пересылки сообщений: [вперед](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) и [CreateForward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="8279c-140">The EWS Managed API provides two methods that you can use to forward messages: [Forward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) and [CreateForward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="8279c-141">Метод **переадресовывать** только используются два входных параметра: сообщение, чтобы в начале существующий текст и массив или коллекцию получателей, в зависимости от того, используется перегруженный метод.</span><span class="sxs-lookup"><span data-stu-id="8279c-141">The **Forward** method only takes two parameters: the message to prepend to the existing body, and an array or collection of recipients, depending on the overload you choose to use.</span></span> <span data-ttu-id="8279c-142">Если необходимо добавить вложения в сообщение в случае переадресации или задавать дополнительные свойства для нового сообщения, используйте метод **CreateForward** , который позволяет задать все свойства, доступные в объект [EmailMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8279c-142">If you need to add an attachment to the message you're forwarding, or set additional properties on the new message, use the **CreateForward** method, which enables you to set all the properties that are available on an [EmailMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object.</span></span> 
  
<span data-ttu-id="8279c-143">В следующем примере кода показано, как использовать метод **переадресовывать** пересылать сообщения электронной почты для одного получателя.</span><span class="sxs-lookup"><span data-stu-id="8279c-143">The following code example shows how to use the **Forward** method to forward an email message to one recipient.</span></span> 
  
<span data-ttu-id="8279c-144">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-144">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> <span data-ttu-id="8279c-145">Локальной переменной *ItemId* — это [идентификатор](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для пересылки.</span><span class="sxs-lookup"><span data-stu-id="8279c-145">The local variable  *ItemId*  is the [Id](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the item to forward.</span></span> <span data-ttu-id="8279c-146">В примере вызывается [метод FindRecentlySent](#bk_findlast) , убедитесь, что сообщение помечено как пересылку.</span><span class="sxs-lookup"><span data-stu-id="8279c-146">The example calls the [FindRecentlySent method](#bk_findlast) to verify that the message was marked as forwarded.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
string myForward = "This is the message body of the forwarded email.";
// Send the response message.
// This method call results in a CreateItem call to EWS.
message.Forward(myForward, "sadie@contoso.com");
// Verify that the forwarded response was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="8279c-147">В следующем примере кода показано, как использовать метод **CreateForward** пересылать сообщения электронной почты для одного получателя.</span><span class="sxs-lookup"><span data-stu-id="8279c-147">The following code example shows how to use the **CreateForward** method to forward an email message to one recipient.</span></span> 
  
```cs
// Bind to the email message to reply to by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, BasePropertySet.IdOnly);
// Create the reply response message from the original email message.
// Indicate whether the message is a reply or reply all type of reply.
ResponseMessage forwardMessage = message.CreateForward();
// Set properties on the email message.
forwardMessage.ToRecipients.Add("sadie@contoso.com");
forwardMessage.Body = "Sadie,<br><br>I thought you'd be interested in this thread.<br><br>-Mack";
// Send and save a copy of the replied email message in the default Sent Items folder. 
forwardMessage.SendAndSaveCopy();
// Verify that the forwarded message was sent by calling FindRecentlySent.
FindRecentlySent(message);
```

<span data-ttu-id="8279c-148">Если требуется добавить вложение в переадресованных сообщений, замените вызов метода **SendAndSaveCopy** следующий код.</span><span class="sxs-lookup"><span data-stu-id="8279c-148">If you need to add an attachment to the forwarded message, replace the call to the **SendAndSaveCopy** method with the following code.</span></span> 
  
```cs
EmailMessage forward = forwardMessage.Save();
forward.Attachments.AddFileAttachment("attachmentname.txt");
forward.Update(ConflictResolutionMode.AutoResolve);
forward.SendAndSaveCopy();
```

## <a name="forward-an-email-message-by-using-ews"></a><span data-ttu-id="8279c-149">Пересылать сообщения электронной почты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-149">Forward an email message by using EWS</span></span>
<span data-ttu-id="8279c-150"><a name="bk_forwardews"> </a></span><span class="sxs-lookup"><span data-stu-id="8279c-150"></span></span>

<span data-ttu-id="8279c-151">В следующем примере кода показано, как пересылать сообщение с помощью веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="8279c-151">The following code example shows how to forward a message by using EWS.</span></span> <span data-ttu-id="8279c-152">С помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с атрибутом **MessageDisposition** , равным **SendAndSaveCopy** отправлять сообщения и сохранения ответа в папке «Отправленные».</span><span class="sxs-lookup"><span data-stu-id="8279c-152">Use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with the **MessageDisposition** attribute set to **SendAndSaveCopy** to send the message and save the response in the Sent Items folder.</span></span> <span data-ttu-id="8279c-153">Элемент [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) указывает, что элемент переадресованных сообщений.</span><span class="sxs-lookup"><span data-stu-id="8279c-153">The [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) element indicates that the item is a forwarded message.</span></span> 
  
<span data-ttu-id="8279c-154">Это также XML-запрос, который отправляет управляемый API EWS при вызове [вперед](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) или метод [CreateForward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8279c-154">This is also the XML request that the EWS Managed API sends when calling either the [Forward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) or the [CreateForward](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) method.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:ForwardItem>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
          <t:ReferenceItemId Id="AAAMkADE="
                             ChangeKey="CQAAABYA" />
          <t:NewBodyContent BodyType="HTML">This is the message body of the forwarded email.</t:NewBodyContent>
        </t:ForwardItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="8279c-155">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что переадресованных сообщений был создан и отправлен успешно.</span><span class="sxs-lookup"><span data-stu-id="8279c-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the forwarded message was created and sent successfully.</span></span>
  
<span data-ttu-id="8279c-156">Если необходимо добавить вложения в ответное сообщение вызова операции **CreateItem** , но измените **MessageDisposition** на **SaveOnly**.</span><span class="sxs-lookup"><span data-stu-id="8279c-156">If you need to add an attachment to your response message, call the **CreateItem** operation, but change the **MessageDisposition** to **SaveOnly**.</span></span> <span data-ttu-id="8279c-157">Затем вызовите операцию [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , а затем операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8279c-157">Then call the [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) operation, followed by the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation.</span></span> 
  
## <a name="find-the-message-last-replied-to-or-forwarded-by-using-the-ews-managed-api"></a><span data-ttu-id="8279c-158">Найдите сообщение последнего или задачи с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-158">Find the message last replied to or forwarded by using the EWS Managed API</span></span>
<span data-ttu-id="8279c-159"><a name="bk_findlast"> </a></span><span class="sxs-lookup"><span data-stu-id="8279c-159"></span></span>

<span data-ttu-id="8279c-160">В следующем примере кода показано, как найти последнего выполнения команды и время последнего глаголов выполнен на указанный элемент.</span><span class="sxs-lookup"><span data-stu-id="8279c-160">The following code example shows how to find the last verb executed and the time the last verb was executed on the item specified.</span></span> <span data-ttu-id="8279c-161">Этот метод вызывается из других примеров кода, управляемый API EWS в этом разделе, чтобы подтвердить, что элементы вы или задачи были помечается как ответ или перенаправлять в папку "Входящие".</span><span class="sxs-lookup"><span data-stu-id="8279c-161">This method is called from other EWS Managed API code examples in this topic to verify that the items you replied to or forwarded were marked as replied to or forwarded in your Inbox.</span></span> 
  
<span data-ttu-id="8279c-162">В примере используется свойство [PidTagLastVerbExecuted](http://msdn.microsoft.com/ru-ru/library/cc841968.aspx) (0x10820003) расширенные для определения необходимости сообщение было ответ, ответить всем или прямого и [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/ru-ru/library/cc839918.aspx) (0x10820040) расширенные свойства, чтобы определить, когда ответить или переслать было отправлено.</span><span class="sxs-lookup"><span data-stu-id="8279c-162">The example uses the [PidTagLastVerbExecuted](http://msdn.microsoft.com/ru-ru/library/cc841968.aspx) (0x10820003) extended property to determine whether the message was a reply, a reply all, or a forward, and the [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/ru-ru/library/cc839918.aspx) (0x10820040) extended property to determine when the reply or forward was sent.</span></span> 
  
```cs
public static void FindRecentlySent(EmailMessage messageToCheck)
{
    // Create extended property definitions for PidTagLastVerbExecuted and PidTagLastVerbExecutionTime.
    ExtendedPropertyDefinition PidTagLastVerbExecuted = new ExtendedPropertyDefinition(0x1081, MapiPropertyType.Integer);
    ExtendedPropertyDefinition PidTagLastVerbExecutionTime = new ExtendedPropertyDefinition(0x1082, MapiPropertyType.SystemTime);
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, PidTagLastVerbExecutionTime, PidTagLastVerbExecuted);
    messageToCheck = EmailMessage.Bind(service, messageToCheck.Id, propSet);
    // Determine the last verb executed on the message and display output.
    object responseType;
    if (messageToCheck.TryGetProperty(PidTagLastVerbExecuted, out responseType))
    {
        object ReplyTime = null;
        switch (((Int32)responseType))
        {
            case 102: Console.WriteLine("A reply was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 103: Console.WriteLine("A reply all was sent to the '" + messageToCheck.Subject.ToString() + "' email message at");
                break;
            case 104: Console.WriteLine("The '" + messageToCheck.Subject.ToString() + "' email message was forwarded at");
                break;
        }
        if (messageToCheck.TryGetProperty(PidTagLastVerbExecutionTime, out ReplyTime))
        {
            Console.WriteLine(((DateTime)ReplyTime).ToString() + ".");
        }
    }
    else
    {
        Console.WriteLine("No changes were made to  '" + messageToCheck.Subject.ToString() + "'.");
    }
}
```

## <a name="see-also"></a><span data-ttu-id="8279c-163">См. также</span><span class="sxs-lookup"><span data-stu-id="8279c-163">See also</span></span>


- [<span data-ttu-id="8279c-164">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-164">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="8279c-165">Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="8279c-165">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

