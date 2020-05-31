---
title: Отправка сообщений электронной почты с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 5290fafe-8b51-4275-a27e-baf497fc969c
description: Сведения о том, как отправлять новые или черновики сообщений электронной почты, а также отправлять задержанные сообщения электронной почты с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: f09babfcc420d4cbc563ed6605ba555fd9f8c7e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761108"
---
# <a name="send-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="4adc3-103">Отправка сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4adc3-103">Send email messages by using EWS in Exchange</span></span>

<span data-ttu-id="4adc3-104">Сведения о том, как отправлять новые или черновики сообщений электронной почты, а также отправлять задержанные сообщения электронной почты с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="4adc3-104">Learn how to send new or draft email messages, or to send a delayed email message by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="4adc3-105">Независимо от того, используете ли вы управляемый API EWS или EWS, вы можете отправлять сообщения электронной почты двумя способами.</span><span class="sxs-lookup"><span data-stu-id="4adc3-105">Whether you are using the EWS Managed API or EWS, you can send email messages in two ways.</span></span> <span data-ttu-id="4adc3-106">Вы можете отправить существующее сообщение, например сообщение, сохраненное в папке "Черновики", или создать и отправить сообщение на одном шаге.</span><span class="sxs-lookup"><span data-stu-id="4adc3-106">You can either send an existing message, such as a message stored in your Drafts folder, or you can create and send an email in one step.</span></span> <span data-ttu-id="4adc3-107">Методы и операции, используемые для отправки сообщения, одинаковы, если вы отправляете сообщение немедленно или отправляете отложенное сообщение.</span><span class="sxs-lookup"><span data-stu-id="4adc3-107">The methods and operations that you use to send the message are the same whether you're sending a message immediately, or sending a delayed message.</span></span>
  
<span data-ttu-id="4adc3-108">**Таблица 1. Методы управляемого API EWS и операции EWS для отправки сообщений электронной почты**</span><span class="sxs-lookup"><span data-stu-id="4adc3-108">**Table 1. EWS Managed API methods and EWS operations for sending email messages**</span></span>

|<span data-ttu-id="4adc3-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="4adc3-109">**Task**</span></span>|<span data-ttu-id="4adc3-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="4adc3-110">**EWS Managed API method**</span></span>|<span data-ttu-id="4adc3-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="4adc3-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4adc3-112">Отправка нового сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="4adc3-112">Send a new email message</span></span>  <br/> |[<span data-ttu-id="4adc3-113">EmailMessage. SendAndSaveCopy</span><span class="sxs-lookup"><span data-stu-id="4adc3-113">EmailMessage.SendAndSaveCopy</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4adc3-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="4adc3-114">CreateItem</span></span>](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="4adc3-115">Отправка существующего сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="4adc3-115">Send an existing email message</span></span>  <br/> |[<span data-ttu-id="4adc3-116">EmailMessage. Send</span><span class="sxs-lookup"><span data-stu-id="4adc3-116">EmailMessage.Send</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="4adc3-117">SendItem</span><span class="sxs-lookup"><span data-stu-id="4adc3-117">SendItem</span></span>](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> |
   
## <a name="send-a-new-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="4adc3-118">Отправка нового сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-118">Send a new email message by using the EWS Managed API</span></span>
<span data-ttu-id="4adc3-119"><a name="bk_sendnewewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-119"><a name="bk_sendnewewsma"> </a></span></span>

<span data-ttu-id="4adc3-120">В приведенном ниже примере кода показано, как использовать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты и метода [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) для отправки сообщения получателю и сохранения сообщения в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-120">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message and the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send the message to the recipient and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="4adc3-121">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="4adc3-121">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "' and saved in the SendItems folder.");
```

## <a name="send-a-new-email-message-by-using-ews"></a><span data-ttu-id="4adc3-122">Отправка нового сообщения электронной почты с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-122">Send a new email message by using EWS</span></span>
<span data-ttu-id="4adc3-123"><a name="bk_sendnewews"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-123"><a name="bk_sendnewews"> </a></span></span>

<span data-ttu-id="4adc3-124">В следующем примере кода показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) со значением **мессажедиспоситион** , равным **SendAndSaveCopy** , для создания сообщения электронной почты, отправки сообщения получателю и сохранения сообщения в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-124">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, send the message to the recipient, and save the message in the Sent Items folder.</span></span> <span data-ttu-id="4adc3-125">Это также запрос XML, который отправляет управляемый API EWS при [отправке нового сообщения электронной почты](#bk_sendnewewsma).</span><span class="sxs-lookup"><span data-stu-id="4adc3-125">This is also the XML request that the EWS Managed API sends when you [send a new email message](#bk_sendnewewsma).</span></span>
  
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
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4adc3-126">В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="4adc3-126">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="send-a-draft-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="4adc3-127">Отправка черновика электронного сообщения с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-127">Send a draft email message by using the EWS Managed API</span></span>
<span data-ttu-id="4adc3-128"><a name="bk_senddraftewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-128"><a name="bk_senddraftewsma"> </a></span></span>

<span data-ttu-id="4adc3-129">В приведенном ниже примере кода показано, как отправить сообщение, которое было сохранено в папке "Черновики", как показано в разделе [Создание сообщения электронной почты с помощью управляемого API EWS](email-and-ews-in-exchange.md#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="4adc3-129">The following code example shows how to send a message that was stored in the Drafts folder, as shown in [Create an email message by using the EWS Managed API](email-and-ews-in-exchange.md#bk_createewsma).</span></span> <span data-ttu-id="4adc3-130">Сначала используйте метод [BIND](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , чтобы получить сообщение, а затем используйте метод [Send](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) для отправки сообщения электронной почты, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="4adc3-130">First, use the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to retrieve the message, and then use the [Send](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) method to send the email message, as shown in the following code example.</span></span> <span data-ttu-id="4adc3-131">Обратите внимание, что этот метод не сохраняет отправленное сообщение в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-131">Note that this method does not save the sent message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="4adc3-132">В этом случае свойства [емаилмессажесчема. subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) и [емаилмессажесчема. ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) добавляются в [свойство](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы эти значения можно было включить в выходные данные консоли.</span><span class="sxs-lookup"><span data-stu-id="4adc3-132">In this case, the [EmailMessageSchema.Subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) and [EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) properties are added to the [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) so that the values can be included in the console output.</span></span> 
  
<span data-ttu-id="4adc3-133">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="4adc3-133">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// As a best practice, create a property set that limits the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
// This method call results in a GetItem call to EWS.
EmailMessage message = EmailMessage.Bind(service, ItemId, propSet);
// Send the email message.
// This method call results in a SendItem call to EWS.
message.Send();
Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" + message.ToRecipients[0] + "'.");
```

## <a name="send-a-draft-email-message-by-using-ews"></a><span data-ttu-id="4adc3-134">Отправка черновика электронного сообщения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-134">Send a draft email message by using EWS</span></span>
<span data-ttu-id="4adc3-135"><a name="bk_senddraftews"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-135"><a name="bk_senddraftews"> </a></span></span>

<span data-ttu-id="4adc3-136">В приведенных ниже примерах кода показано, как отправить сообщение, которое ранее хранилось в папке "Черновики", как показано в разделе [Создание сообщения электронной почты с помощью EWS](email-and-ews-in-exchange.md#bk_createews).</span><span class="sxs-lookup"><span data-stu-id="4adc3-136">The following code examples show how to send a message that was previously stored in the Drafts folder, as shown in [Create an email message by using EWS](email-and-ews-in-exchange.md#bk_createews).</span></span> <span data-ttu-id="4adc3-137">Сначала используйте операцию [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , чтобы получить сообщение электронной почты для отправки.</span><span class="sxs-lookup"><span data-stu-id="4adc3-137">First use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to retrieve the email message to send.</span></span> <span data-ttu-id="4adc3-138">Затем с помощью операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) отправьте сообщение электронной почты получателям и сохраните его в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-138">Then use the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the email message to recipients and save it in the Sent Items folder.</span></span> 
  
<span data-ttu-id="4adc3-139">Первое сообщение, сообщение с запросом **GetItem** , указывает идентификатор [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) черновика сообщения электронной почты, к которому выполняется привязка, а элементы в элементе [итемшапе](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) ограничивают результаты для включения в ответ **GetItem** .</span><span class="sxs-lookup"><span data-stu-id="4adc3-139">The first message, the **GetItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the draft email message to bind to, and elements in the [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) element limit the results to include in the **GetItem** response.</span></span> <span data-ttu-id="4adc3-140">Элемент **итемшапе** имеет [басешапе](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) из **идонли**, а элемент [аддитионалпропертиес](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) содержит значения [Фиелдури](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) для свойства **subject** из схемы элемента и свойства **ToRecipients** из схемы сообщения, что означает, что клиенту в ответе будут возвращены только элементы **ItemId**, [subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)и [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4adc3-140">The **ItemShape** element has a [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) of **IdOnly**, and the [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) element includes the [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) values for the **Subject** property from the Item schema and the **ToRecipients** property from the Message schema, which means that only the **ItemId**, [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx), and [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) elements will be returned to the client in the response.</span></span> <span data-ttu-id="4adc3-141">Дополнительные сведения об ограничении значений, возвращаемых в вызовах и значении элемента **басешапе** , приведены в статье [наборы свойств и формы ответа в EWS в Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="4adc3-141">For more information about limiting the values returned in calls and the meaning of the **BaseShape** element, see [Property sets and response shapes in EWS in Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="4adc3-142">Это также XML-запрос, который отправляется управляемым API EWS при вызове метода [BIND](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="4adc3-142">This is also the XML request that is sent by the EWS Managed API when calling the [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="4adc3-143">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="4adc3-143">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="message:ToRecipients" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="AAMkADE4=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

В приведенном ниже примере показан XML-ответ, возвращаемый сервером после обработки операции **GetItem**. Ответ указывает на то, что сообщение электронной почты было успешно получено и включает элементы **subject** и **тореЦипиент** по запросу. <span data-ttu-id="4adc3-146">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="4adc3-146">The values of some attributes and elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="842"
                         MinorBuildNumber="10"
                         Version="V2_8"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="AAMkADE4="
                        ChangeKey="CQAAABYA" />
              <t:Subject>Project priorities</t:Subject>
              <t:ToRecipients>
                <t:Mailbox>
                  <t:Name>sadie@contoso.com</t:Name>
                  <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                  <t:MailboxType>OneOff</t:MailboxType>
                </t:Mailbox>
              </t:ToRecipients>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="4adc3-147">Второе сообщение, сообщение запроса **SendItem** , указывает идентификатор [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) отправляемого сообщения электронной почты, а также [саведитемфолдерид](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), указывающий папку, в которой нужно сохранить отправленный элемент.</span><span class="sxs-lookup"><span data-stu-id="4adc3-147">The second message, the **SendItem** request message, specifies the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to send, as well as the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), which specifies the folder in which to save the sent item.</span></span>
  
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
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADE4="
                  ChangeKey="CQAAABYA" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4adc3-148">Сервер отвечает на запрос **SendItem** с сообщением [сендитемреспонсе](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение было отправлено успешно.</span><span class="sxs-lookup"><span data-stu-id="4adc3-148">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was sent successfully.</span></span>
  
## <a name="send-a-delayed-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="4adc3-149">Отправка задержанного сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-149">Send a delayed email message by using the EWS Managed API</span></span>
<span data-ttu-id="4adc3-150"><a name="bk_senddelayedewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-150"><a name="bk_senddelayedewsma"> </a></span></span>

<span data-ttu-id="4adc3-151">В приведенном ниже примере кода показано, как использовать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты, класса [екстендедпропертидефинитион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) , чтобы создать определение свойства для свойства [PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) (0x3FEF0040), а метод [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) — для отправки задержанного сообщения и сохранения сообщения в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-151">The following code example shows how to use the [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object to create an email message, the [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) class to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) (0x3FEF0040) property, and the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) method to send a delayed message and save the message in the Sent Items folder.</span></span> 
  
<span data-ttu-id="4adc3-152">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="4adc3-152">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Create a new email message. 
EmailMessage message = new EmailMessage(service);
// Specify the email recipient and subject. 
message.ToRecipients.Add("sadie@contoso.com");
message.Subject = "Delayed email";
// Identify the extended property that can be used to specify when to send the email. 
ExtendedPropertyDefinition PidTagDeferredSendTime = new ExtendedPropertyDefinition(16367, MapiPropertyType.SystemTime);
// Set the time that will be used to specify when the email is sent. 
// In this example, the email will be sent one minute after the next line executes, 
// provided that the message.SendAndSaveCopy request is processed by the server within one minute. 
string sendTime = DateTime.Now.AddMinutes(1).ToUniversalTime().ToString();
// Specify when to send the email by setting the value of the extended property. 
message.SetExtendedProperty(PidTagDeferredSendTime, sendTime);
// Specify the email body. 
StringBuilder str = new StringBuilder();
str.AppendLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
str.AppendLine("The email message will be sent at: " + sendTime + ".");
message.Body = str.ToString();
Console.WriteLine("");
Console.WriteLine("The client submitted the SendAndSaveCopy request at: " + DateTime.Now.ToUniversalTime().ToString() + ".");
Console.WriteLine("The email message will be sent at: " + sendTime + ".");
// Submit the request to send the email message. 
message.SendAndSaveCopy();
```

## <a name="send-a-delayed-email-message-by-using-ews"></a><span data-ttu-id="4adc3-153">Отправка задержанного сообщения электронной почты с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="4adc3-153">Send a delayed email message by using EWS</span></span>
<span data-ttu-id="4adc3-154"><a name="bk_senddelayedews"> </a></span><span class="sxs-lookup"><span data-stu-id="4adc3-154"><a name="bk_senddelayedews"> </a></span></span>

<span data-ttu-id="4adc3-155">В следующем примере кода показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) со значением **мессажедиспоситион** , равным **SendAndSaveCopy** , чтобы создать сообщение электронной почты, элемент [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) для создания определения свойства для свойства [PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) (0X3FEF0040), чтобы задать время отправки сообщения и элемент [саведитемфолдерид](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) для сохранения отправленного сообщения в папке "Отправленные".</span><span class="sxs-lookup"><span data-stu-id="4adc3-155">The following code example shows how to use the [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) operation with a **MessageDisposition** value of **SendAndSaveCopy** to create an email message, the [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) element to create a property definition for the [PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) (0x3FEF0040) property to set a time to send the message, and the [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) element to save the sent message in the Sent Items folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Delayed email</t:Subject>
          <t:Body BodyType="HTML">
            The client submitted the SendAndSaveCopy request at: 1/2/2014 9:08:52 PM.
            The email message will be sent at: 1/2/2014 9:09:52 PM.
          </t:Body>
          <t:ExtendedProperty>
            <t:ExtendedFieldURI PropertyTag="16367"
                                PropertyType="SystemTime" />
            <t:Value>2014-01-02T21:09:52.000</t:Value>
          </t:ExtendedProperty>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4adc3-156">В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения.</span><span class="sxs-lookup"><span data-stu-id="4adc3-156">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email was created successfully, and the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the newly created message.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="4adc3-157">См. также</span><span class="sxs-lookup"><span data-stu-id="4adc3-157">See also</span></span>


- [<span data-ttu-id="4adc3-158">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="4adc3-158">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="4adc3-159">Ответ на сообщения электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4adc3-159">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    

