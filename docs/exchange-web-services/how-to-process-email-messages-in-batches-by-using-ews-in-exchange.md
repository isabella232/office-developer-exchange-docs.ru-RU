---
title: Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Узнайте, как создавать, получать, обновлять и удалять пакеты сообщений электронной почты в едином вызове с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 2592076c9c5b57356d96872f006dd7b0abfc328a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527777"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a><span data-ttu-id="808b9-103">Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="808b9-103">Process email messages in batches by using EWS in Exchange</span></span>

<span data-ttu-id="808b9-104">Узнайте, как создавать, получать, обновлять и удалять пакеты сообщений электронной почты в едином вызове с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="808b9-104">Learn how to create, get, update, and delete batches of email messages in a single call by using the EWS Managed API or EWS in Exchange.</span></span>

<span data-ttu-id="808b9-105">Вы можете использовать управляемый API EWS или EWS для работы с пакетами сообщений электронной почты, чтобы уменьшить количество звонков, которые клиент делает на сервер Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="808b9-105">You can use the EWS Managed API or EWS to work with batches of email messages to reduce the number of calls a client makes to an Exchange server.</span></span> <span data-ttu-id="808b9-106">При использовании управляемого API EWS для создания, получения, обновления, удаления и отправки сообщений в пакетах используются методы объекта [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а при работе с отдельными сообщениями электронной почты используются методы объекта [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="808b9-106">When you use the EWS Managed API to create, get, update, delete, and send messages in batches, you use [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object methods, whereas when you work with single email messages, you use [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object methods.</span></span> <span data-ttu-id="808b9-107">Если вы используете EWS, вы можете использовать те же операции для работы с одним и пакетными сообщениями электронной почты.</span><span class="sxs-lookup"><span data-stu-id="808b9-107">If you are using EWS, you use the same operations to work with both single and batches of email messages.</span></span>

<span data-ttu-id="808b9-108">**Таблица 1. Методы управляемого API EWS и операции EWS для работы с пакетами сообщений электронной почты**</span><span class="sxs-lookup"><span data-stu-id="808b9-108">**Table 1. EWS Managed API methods and EWS operations for working with batches of email messages**</span></span>

|<span data-ttu-id="808b9-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="808b9-109">**In order to…**</span></span>|<span data-ttu-id="808b9-110">**Используйте этот метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="808b9-110">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="808b9-111">**Используйте эту операцию EWS**</span><span class="sxs-lookup"><span data-stu-id="808b9-111">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="808b9-112">Создание сообщений электронной почты в пакетах</span><span class="sxs-lookup"><span data-stu-id="808b9-112">Create email messages in batches</span></span>  <br/> |[<span data-ttu-id="808b9-113">ExchangeService. CreateItems</span><span class="sxs-lookup"><span data-stu-id="808b9-113">ExchangeService.CreateItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="808b9-114">CreateItem</span><span class="sxs-lookup"><span data-stu-id="808b9-114">CreateItem</span></span>](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="808b9-115">Получение сообщений электронной почты в пакетах</span><span class="sxs-lookup"><span data-stu-id="808b9-115">Get email messages in batches</span></span>  <br/> |[<span data-ttu-id="808b9-116">ExchangeService. Биндтоитемс</span><span class="sxs-lookup"><span data-stu-id="808b9-116">ExchangeService.BindToItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="808b9-117">GetItem</span><span class="sxs-lookup"><span data-stu-id="808b9-117">GetItem</span></span>](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="808b9-118">Обновление сообщений электронной почты в пакетах</span><span class="sxs-lookup"><span data-stu-id="808b9-118">Update email messages in batches</span></span>  <br/> |[<span data-ttu-id="808b9-119">ExchangeService. Упдатеитемс</span><span class="sxs-lookup"><span data-stu-id="808b9-119">ExchangeService.UpdateItems</span></span>](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="808b9-120">UpdateItem</span><span class="sxs-lookup"><span data-stu-id="808b9-120">UpdateItem</span></span>](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="808b9-121">Удаление сообщений электронной почты в пакетах</span><span class="sxs-lookup"><span data-stu-id="808b9-121">Delete email messages in batches</span></span>  <br/> |[<span data-ttu-id="808b9-122">ExchangeService. Делетеитемс</span><span class="sxs-lookup"><span data-stu-id="808b9-122">ExchangeService.DeleteItems</span></span>](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="808b9-123">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="808b9-123">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |

<span data-ttu-id="808b9-124">В этой статье рассказывается, как выполнить основные задачи для пакетов сообщений электронной почты с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="808b9-124">In this article, you'll learn how to complete basic tasks for batches of email messages by using the EWS Managed API or EWS.</span></span>

## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="808b9-125">Создание сообщений электронной почты в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-125">Create email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="808b9-126"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-126"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="808b9-127">Вы можете создавать сообщения в пакетах с помощью метода **CreateItems** управляемого API EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-127">You can create messages in batches by using the EWS Managed API **CreateItems** method, as shown in the following example.</span></span> <span data-ttu-id="808b9-128">В этом примере создаются три объекта [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) локально, каждое сообщение добавляется в коллекцию, после чего вызывается метод **CreateItems** для коллекции сообщений.</span><span class="sxs-lookup"><span data-stu-id="808b9-128">This example creates three [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) objects locally, adds each message to a collection, then calls the **CreateItems** method on the collection of messages.</span></span>

<span data-ttu-id="808b9-129">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="808b9-129">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

```cs
public static Collection<ItemId> CreateDraftEmailInBatch(ExchangeService service)
{
    // These are unsaved local instances of an EmailMessage object.
    // Despite the required parameter of an ExchangeService object (service), no call
    // to an Exchange server is made when the objects are instantiated.
    // A call to the Exchange server is made when the service.CreateItems() method is called.
    EmailMessage message1 = new EmailMessage(service);
    EmailMessage message2 = new EmailMessage(service);
    EmailMessage message3 = new EmailMessage(service);
    // Set the properties on the first message.
    message1.Subject = "Project priorities";
    message1.Body = "(1) Buy pizza, (2) Eat pizza";
    message1.ToRecipients.Add("sadie@contoso.com");
    // Set the properties on the second message.
    message2.Subject = "Company Soccer Team";
    message2.Body = "Are you interested in joining?";
    message2.ToRecipients.Add("magdalena@contoso.com");
    // Set the properties on the third message.
    message3.Subject = "Code Blast";
    message3.Body = "Are you interested in getting together to finish the methods for the ContosoLive project?";
    message3.ToRecipients.Add("mack@contoso.com");
    // Add the EmailMessage objects to a collection.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>() { message1, message2, message3 };
    // Create the batch of email messages on the server.
    // This method call results in an CreateItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.Drafts, MessageDisposition.SaveOnly, null);
    // Instantiate a collection of item IDs to populate from the values that are returned by the Exchange server.
    Collection<ItemId> itemIds = new Collection<ItemId>();
    // Collect the item IDs from the created email messages.
    foreach (EmailMessage message in messageItems)
    {
        try
        {
            itemIds.Add(message.Id);
            Console.WriteLine("Email message '{0}' created successfully.", message.Subject);
        }
        catch (Exception ex)
        {
            // Print out the exception and the last eight characters of the item ID.
            Console.WriteLine("Exception while creating message {0}: {1}", message.Id.ToString().Substring(144), ex.Message);
        }
    }
    // Check for success of the CreateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
            Console.WriteLine("All locally created messages were successfully saved to the Drafts folder.");
            Console.WriteLine("\r\n");
    }

    // If the method did not return success, print the result message for each email.
    else
    {
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            // Print out the result and the last eight characters of the item ID.
            Console.WriteLine("Result (message {0}), id {1}: {2}", counter, itemIds[counter - 1].ToString().Substring(144), resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            Console.WriteLine("\r\n");
            counter++;
        }
    }
    return itemIds;
}
```

<span data-ttu-id="808b9-130">Обратите внимание, что в этом примере сообщения сохраняются только в папке "Черновики"; сообщения не отправляются.</span><span class="sxs-lookup"><span data-stu-id="808b9-130">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="808b9-131">Дополнительные сведения о том, как отправлять сообщения, [можно узнать в статье отправка сообщений электронной почты в пакетах с помощью управляемого API EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-131">For more about how to send the messages, see [Send email messages in batches by using the EWS Managed API](#bk_sendewsma).</span></span>

## <a name="create-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="808b9-132">Создание сообщений электронной почты в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-132">Create email messages in batches by using EWS</span></span>
<span data-ttu-id="808b9-133"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-133"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="808b9-134">Вы можете создавать сообщения электронной почты в пакетах с помощью операции [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="808b9-134">You can create email messages in batches by using the [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="808b9-135">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [создания сообщений электронной почты в пакетах](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-135">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [create email messages in batches](#bk_createewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>magdalena@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
        <t:Message>
          <t:Subject>Code Blast</t:Subject>
          <t:Body BodyType="HTML">Are you interested in getting together to finish the methods for the ContosoLive project?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="808b9-136">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для каждого** из новых сообщений, что означает, что каждое сообщение было создано и сохранено успешно.</span><span class="sxs-lookup"><span data-stu-id="808b9-136">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and saved successfully.</span></span>

<span data-ttu-id="808b9-137">Обратите внимание, что в этом примере сообщения сохраняются только в папке "Черновики"; сообщения не отправляются.</span><span class="sxs-lookup"><span data-stu-id="808b9-137">Note that the example only saves the messages in the Drafts folder; it does not send the messages.</span></span> <span data-ttu-id="808b9-138">Дополнительные сведения о том, как отправлять сообщения, [можно узнать в статье отправка сообщений электронной почты пакетами с помощью EWS](#bk_sendews).</span><span class="sxs-lookup"><span data-stu-id="808b9-138">For more about how to send the messages, see [Send email messages in batches by using EWS](#bk_sendews).</span></span>

## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="808b9-139">Отправка сообщений электронной почты в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-139">Send email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="808b9-140"><a name="bk_sendewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-140"><a name="bk_sendewsma"> </a></span></span>

<span data-ttu-id="808b9-141">Один и тот же код используется для отправки сообщений электронной почты в пакетах, которые используются для создания сообщений электронной почты в пакетах, за исключением того, что некоторые параметры метода [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) меняются.</span><span class="sxs-lookup"><span data-stu-id="808b9-141">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the [CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) method parameters change.</span></span> <span data-ttu-id="808b9-142">Таким образом, чтобы отправлять сообщения электронной почты с помощью управляемого API EWS, используйте код, используемый для [создания сообщений электронной почты в пакетах](#bk_createewsma), и замените вызов метода **CreateItems** на вызов в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-142">So, to send email messages by using the EWS Managed API, use the code you use to [create email messages in batches](#bk_createewsma), and replace the call to the **CreateItems** method with the call in the following example.</span></span> <span data-ttu-id="808b9-143">В этом примере сообщения создаются в папке "Отправленные", а расположение сообщения изменяется на [мессажедиспоситион. SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), поэтому сообщение отправляется, а не просто сохраняется локально.</span><span class="sxs-lookup"><span data-stu-id="808b9-143">In this example, the messages are created in the Sent Items folder, and the message disposition is changed to [MessageDisposition.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), so that the message is sent, and not just saved locally.</span></span>

```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="808b9-144">Отправка сообщений электронной почты пакетами с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-144">Send email messages in batches by using EWS</span></span>
<span data-ttu-id="808b9-145"><a name="bk_sendews"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-145"><a name="bk_sendews"> </a></span></span>

<span data-ttu-id="808b9-146">Один и тот же код используется для отправки сообщений электронной почты в пакетах, которые используются для создания сообщений электронной почты в пакетах, за исключением того, что некоторые значения атрибутов изменяются для операции **CreateItem** .</span><span class="sxs-lookup"><span data-stu-id="808b9-146">You use the same code to send email messages in batches that you use to create email messages in batches, except that a few of the attribute values change for the **CreateItem** operation.</span></span> <span data-ttu-id="808b9-147">Таким образом, чтобы отправлять сообщения электронной почты с помощью EWS, используйте код, используемый для [создания сообщений электронной почты в пакетах](#bk_createews), и измените значение **Мессажедиспоситион** на "SendAndSaveCopy" и измените [дистингуишедфолдерид](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) на "sentitems", как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="808b9-147">So, to send email messages by using EWS, use the code you use to [create email message in batches](#bk_createews), and change the **MessageDisposition** value to "SendAndSaveCopy", and change the [DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) to "sentitems", as shown in the following code example.</span></span>

```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

<span data-ttu-id="808b9-148">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) для каждого из новых сообщений, что **указывает на то** , что каждое сообщение было создано и отправлено успешно.</span><span class="sxs-lookup"><span data-stu-id="808b9-148">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each of the new messages, which indicates that each email was created and sent successfully.</span></span>

## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="808b9-149">Получение сообщений электронной почты в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-149">Get email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="808b9-150"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-150"><a name="bk_getewsma"> </a></span></span>

<span data-ttu-id="808b9-151">Вы можете получать сообщения электронной почты в пакетах с помощью метода [Биндтоитемс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-151">You can get email messages in batches by using the EWS Managed API [BindToItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="808b9-152">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="808b9-152">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

```cs
public static Collection<EmailMessage> BatchGetEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Create a property set that limits the properties returned by the Bind method to only those that are required.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ToRecipients);
    // Get the items from the server.
    // This method call results in a GetItem call to EWS.
    ServiceResponseCollection<GetItemResponse> response = service.BindToItems(itemIds, propSet);

    // Instantiate a collection of EmailMessage objects to populate from the values that are returned by the Exchange server.
    Collection<EmailMessage> messageItems = new Collection<EmailMessage>();
    foreach (GetItemResponse getItemResponse in response)
    {
        try
        {
            Item item = getItemResponse.Item;
            EmailMessage message = (EmailMessage)item;
            messageItems.Add(message);
            // Print out confirmation and the last eight characters of the item ID.
            Console.WriteLine("Found item {0}.", message.Id.ToString().Substring(144));
        }
        catch (Exception ex)
        {
           Console.WriteLine("Exception while getting a message: {0}", ex.Message);
        }
    }
    // Check for success of the BindToItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages retrieved successfully.");
        Console.WriteLine("\r\n");
    }
        return messageItems;
}
```

## <a name="get-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="808b9-153">Получение сообщений электронной почты в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-153">Get email messages in batches by using EWS</span></span>
<span data-ttu-id="808b9-154"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-154"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="808b9-155">Вы можете получать сообщения электронной почты в пакетах с помощью операции [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) и кода в приведенном ниже примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-155">You can get email messages in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation and the code in the following example.</span></span> <span data-ttu-id="808b9-156">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [получения сообщений электронной почты в пакетах](#bk_getewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-156">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get email messages in batches](#bk_getewsma).</span></span>

<span data-ttu-id="808b9-157">Атрибуты **ItemId** и **чанжекэй** были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="808b9-157">The **ItemId** and **ChangeKey** attributes have been shortened for readability.</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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
        <t:ItemId Id="m4NxAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB0" />
        <t:ItemId Id="m4NyAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB1" />
        <t:ItemId Id="m4NzAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKB2" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="808b9-158">Сервер отвечает на запрос **GetItem** с сообщением [жетитемреспонсе](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) , которое включает [свойства первого класса](email-properties-and-elements-in-ews-in-exchange.md) для каждого из запрошенных сообщений.</span><span class="sxs-lookup"><span data-stu-id="808b9-158">The server responds to the **GetItem** request with a [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes the [first class properties](email-properties-and-elements-in-ews-in-exchange.md) for each of the requested messages.</span></span>

## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="808b9-159">Обновление сообщений электронной почты в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-159">Update email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="808b9-160"><a name="bk_updateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-160"><a name="bk_updateewsma"> </a></span></span>

<span data-ttu-id="808b9-161">Вы можете получать сообщения электронной почты в пакетах с помощью метода [Упдатеитемс](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-161">You can get email messages in batches by using the EWS Managed API [UpdateItems](https://msdn.microsoft.com/library/dd634705%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="808b9-162">Список свойств сообщений электронной почты, доступных для записи, приведен [в статье свойства и элементы электронной почты в EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="808b9-162">For a list of writable email message properties, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>

<span data-ttu-id="808b9-163">Сведения о том, как отправить черновик сообщения после его обновления, можно узнать в статье [Отправка сообщений электронной почты с помощью управляемого API EWS](#bk_sendewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-163">For details about how to send a draft message after it's been updated, see [Sending email messages by using the EWS Managed API](#bk_sendewsma).</span></span>

<span data-ttu-id="808b9-164">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="808b9-164">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

```cs
public static Collection<EmailMessage> BatchUpdateEmailItems(ExchangeService service, Collection<EmailMessage> messageItems)
{
    // Update the subject of each message locally.
    foreach (EmailMessage message in messageItems)
    {
        // Update the Subject of the email.
        message.Subject = "Updated subject at " + DateTime.Now;
        // Print out confirmation with the last eight characters of the item ID and the email subject.
        Console.WriteLine("Updated local email message {0} with the subject '{1}'.", message.Id.ToString().Substring(144), message.Subject);
    }
    // Send the item updates to the server.
    // This method call results in an UpdateItem call to EWS.
    ServiceResponseCollection<UpdateItemResponse> response = service.UpdateItems(messageItems, WellKnownFolderName.Drafts, ConflictResolutionMode.AutoResolve, MessageDisposition.SaveOnly, null);
    // Check for success of the UpdateItems method call.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("All email messages updated successfully.\r\n");
    }
    // If the method did not return success, print the result message for each email.
    else
    {
        Console.WriteLine("All emails were not successfully saved on the server.\r\n");
        int counter = 1;
        foreach (ServiceResponse resp in response)
        {
            Console.WriteLine("Result for (message {0}): {1}", counter, resp.Result);
            Console.WriteLine("Error Code: {0}", resp.ErrorCode);
            Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
            counter++;
        }
    }
    return messageItems;
}
```

## <a name="update-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="808b9-165">Обновление сообщений электронной почты в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-165">Update email messages in batches by using EWS</span></span>
<span data-ttu-id="808b9-166"><a name="bk_updateews"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-166"><a name="bk_updateews"> </a></span></span>

<span data-ttu-id="808b9-167">Вы можете обновлять сообщения электронной почты в пакетах с помощью операции [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="808b9-167">You can update email messages in batches by using the [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS operation, as shown in following code example.</span></span> <span data-ttu-id="808b9-168">Это также запрос XML, который отправляет управляемый API EWS при использовании управляемого API EWS для [обновления сообщений электронной почты в пакетах](#bk_updateewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-168">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [update email messages in batches](#bk_updateewsma).</span></span>

<span data-ttu-id="808b9-169">Список доступных для записи элементов сообщения электронной почты приведен [в статье свойства и элементы электронной почты в веб EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="808b9-169">For a list of writable email message elements, see [Email properties and elements in EWS in Exchange](email-properties-and-elements-in-ews-in-exchange.md).</span></span>

<span data-ttu-id="808b9-170">Сведения о том, как отправить черновик сообщения после его обновления, можно узнать в статье [Отправка черновика сообщения электронной почты с помощью EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span><span class="sxs-lookup"><span data-stu-id="808b9-170">For details about how to send a draft message after it's been updated, see [Send a draft email message by using EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly"
                  ConflictResolution="AutoResolve">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="m4OVAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCy" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OWAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKCz" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
        <t:ItemChange>
          <t:ItemId Id="m4OXAAA="
                    ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKC0" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>Updated subject at 1/17/2014 2:58:09 PM</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="808b9-171">Сервер отвечает на запрос **UpdateItem** с сообщением [упдатеитемреспонсе](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , указывающее на то **, что**все обновления успешно сохранены на сервере.</span><span class="sxs-lookup"><span data-stu-id="808b9-171">The server responds to the **UpdateItem** request with an [UpdateItemResponse](https://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that each of the updates was saved successfully on the server.</span></span> <span data-ttu-id="808b9-172">Все конфликты включаются в элемент [конфликтресулт](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="808b9-172">Any conflicts are reported in the [ConflictResult](https://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) element.</span></span>

## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a><span data-ttu-id="808b9-173">Удаление сообщений электронной почты в пакетах с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-173">Delete email messages in batches by using the EWS Managed API</span></span>
<span data-ttu-id="808b9-174"><a name="bk_deleteewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-174"><a name="bk_deleteewsma"> </a></span></span>

<span data-ttu-id="808b9-175">Вы можете удалять сообщения в пакетах с помощью метода [Делетеитемс](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="808b9-175">You can delete messages in batches by using the EWS Managed API [DeleteItems](https://msdn.microsoft.com/library/dd635460%28v=exchg.80%29.aspx) method, as shown in the following example.</span></span>

<span data-ttu-id="808b9-176">В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server.</span><span class="sxs-lookup"><span data-stu-id="808b9-176">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span>

```cs
public static void BatchDeleteEmailItems(ExchangeService service, Collection<ItemId> itemIds)
{
    // Delete the batch of email message objects.
    // This method call results in an DeleteItem call to EWS.
    ServiceResponseCollection<ServiceResponse> response = service.DeleteItems(itemIds, DeleteMode.SoftDelete, null, AffectedTaskOccurrence.AllOccurrences);

    // Check for success of the DeleteItems method call.
    // DeleteItems returns success even if it does not find all the item IDs.
    if (response.OverallResult == ServiceResult.Success)
    {
        Console.WriteLine("Email messages deleted successfully.\r\n");
    }
    // If the method did not return success, print a message.
    else
    {
        Console.WriteLine("Not all email messages deleted successfully.\r\n");
    }
}
```

## <a name="delete-email-messages-in-batches-by-using-ews"></a><span data-ttu-id="808b9-177">Удаление сообщений электронной почты в пакетах с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-177">Delete email messages in batches by using EWS</span></span>
<span data-ttu-id="808b9-178"><a name="bk_deleteews"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-178"><a name="bk_deleteews"> </a></span></span>

<span data-ttu-id="808b9-179">Вы можете удалять сообщения электронной почты в пакетах с помощью операции [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS, как показано в следующем примере кода.</span><span class="sxs-lookup"><span data-stu-id="808b9-179">You can delete email messages in batches by using the [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS operation, as shown in the following code example.</span></span> <span data-ttu-id="808b9-180">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [удаления сообщений электронной почты в пакетах](#bk_deleteewsma).</span><span class="sxs-lookup"><span data-stu-id="808b9-180">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [delete email messages in batches](#bk_deleteewsma).</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="SoftDelete"
                  AffectedTaskOccurrences="AllOccurrences">
      <m:ItemIds>
        <t:ItemId Id="m4OkAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDE" />
        <t:ItemId Id="m4OlAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDF" />
        <t:ItemId Id="m4OmAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF/yKDG" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="808b9-181">Сервер отвечает на запрос **DeleteItem** с сообщением [делетеитемреспонсе](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для удаления для каждого** удаленного элемента.</span><span class="sxs-lookup"><span data-stu-id="808b9-181">The server responds to the **DeleteItem** request with a [DeleteItemResponse](https://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** for each item that was removed.</span></span> <span data-ttu-id="808b9-182">Обратите внимание, что при выполнении операции также возвращается значение Success, если не удалось найти идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="808b9-182">Note that the operation also returns success if the item ID could not be found.</span></span>

## <a name="verifying-that-a-batch-process-completed-successfully"></a><span data-ttu-id="808b9-183">Проверка успешного завершения пакетной обработки</span><span class="sxs-lookup"><span data-stu-id="808b9-183">Verifying that a batch process completed successfully</span></span>
<span data-ttu-id="808b9-184"><a name="bk_successful"> </a></span><span class="sxs-lookup"><span data-stu-id="808b9-184"><a name="bk_successful"> </a></span></span>

<span data-ttu-id="808b9-185">Если одно или несколько сообщений электронной почты в пакетном запросе не могут быть обработаны как запрошенные, возвращается ошибка для каждого неудачного сообщения электронной почты, а остальные сообщения в пакете обрабатываются должным образом.</span><span class="sxs-lookup"><span data-stu-id="808b9-185">When one or more email messages in a batched request can't be processed as requested, an error is returned for each email message that failed, and the rest of the emails in the batch are processed as expected.</span></span> <span data-ttu-id="808b9-186">Ошибки в пакетной обработке могут возникать, если элемент был удален, поэтому не может быть отправлен, извлечен или обновлен, или если элемент перемещен в другую папку, и поэтому не может быть изменен с помощью идентификатора элемента.</span><span class="sxs-lookup"><span data-stu-id="808b9-186">Failures in batch processing can occur if the item was deleted, and therefore can't be sent, retrieved, or updated, or if the item moved to a different folder, and therefore has a new item ID, and cannot be modified with the item ID sent.</span></span> <span data-ttu-id="808b9-187">В этом разделе показано, как получить сведения об ошибках при пакетной обработке сообщения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="808b9-187">The information in this section shows how to get error details about failures in batch processing of email message.</span></span>

<span data-ttu-id="808b9-188">Чтобы проверить успешность пакетной обработки с помощью управляемого API EWS, можно проверить, что свойство [овераллресулт](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) объекта [сервицереспонсеколлектион](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) равно [сервицересулт. Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="808b9-188">To verify the success of a batch process by using the EWS Managed API, you can check that the [OverallResult](https://msdn.microsoft.com/library/dd634515%28v=exchg.80%29.aspx) property of the [ServiceResponseCollection](https://msdn.microsoft.com/library/dd633715%28v=exchg.80%29.aspx) is equal to [ServiceResult.Success](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx).</span></span> <span data-ttu-id="808b9-189">В таком случае все сообщения электронной почты обрабатывались успешно.</span><span class="sxs-lookup"><span data-stu-id="808b9-189">If so, all the emails were processed successfully.</span></span> <span data-ttu-id="808b9-190">Если **овераллресулт** не равно **сервицересулт. Success**, одно или несколько сообщений электронной почты не были обработаны успешно.</span><span class="sxs-lookup"><span data-stu-id="808b9-190">If the **OverallResult** is not equal to **ServiceResult.Success**, one or more of the emails were not processed successfully.</span></span> <span data-ttu-id="808b9-191">Каждый из объектов, возвращенных в **сервицереспонсеколлектион** , содержит следующие свойства:</span><span class="sxs-lookup"><span data-stu-id="808b9-191">Each of the objects returned in the **ServiceResponseCollection** contains the following properties:</span></span>

- [<span data-ttu-id="808b9-192">ErrorCode</span><span class="sxs-lookup"><span data-stu-id="808b9-192">ErrorCode</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)

- [<span data-ttu-id="808b9-193">еррордетаилс</span><span class="sxs-lookup"><span data-stu-id="808b9-193">ErrorDetails</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)

- [<span data-ttu-id="808b9-194">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="808b9-194">ErrorMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)

- [<span data-ttu-id="808b9-195">еррорпропертиес</span><span class="sxs-lookup"><span data-stu-id="808b9-195">ErrorProperties</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)

- [<span data-ttu-id="808b9-196">Результат</span><span class="sxs-lookup"><span data-stu-id="808b9-196">Result</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)

<span data-ttu-id="808b9-197">Эти свойства содержат сведения о том, почему сообщения электронной почты не могут быть обработаны по запросу.</span><span class="sxs-lookup"><span data-stu-id="808b9-197">These properties contain information about why the email messages could not be processed as requested.</span></span> <span data-ttu-id="808b9-198">В примерах, приведенных в этой статье, распечатываться **результат**, **ErrorCode**и **ErrorMessage** для каждого сообщения, которое не удалось выполнить.</span><span class="sxs-lookup"><span data-stu-id="808b9-198">The examples in this article print out the **Result**, **ErrorCode**, and **ErrorMessage** for each failed message.</span></span> <span data-ttu-id="808b9-199">Вы можете использовать эти результаты для изучения проблемы.</span><span class="sxs-lookup"><span data-stu-id="808b9-199">You can use these results to investigate the issue.</span></span>

<span data-ttu-id="808b9-200">Для проверки успешности пакетного процесса в EWS проверьте атрибут [респонсекласс](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) для каждого обрабатываемого элемента.</span><span class="sxs-lookup"><span data-stu-id="808b9-200">For EWS, to verify the success of a batched process, check the [ResponseClass](https://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) attribute for each item being processed.</span></span> <span data-ttu-id="808b9-201">Ниже приведена базовая структура **респонсемессажетипе**, базовый тип которого является производным от всех ответных сообщений.</span><span class="sxs-lookup"><span data-stu-id="808b9-201">The following is the basic structure of the **ResponseMessageType**, the base type from which all response messages are derived.</span></span>

```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

<span data-ttu-id="808b9-202">Атрибут **респонсекласс** имеет значение **Success** , если сообщение было обработано успешно, или **Ошибка** , если сообщение не было обработано успешно.</span><span class="sxs-lookup"><span data-stu-id="808b9-202">The **ResponseClass** attribute is set to **Success** if the email was processed successfully, or **Error** if the email was not processed successfully.</span></span> <span data-ttu-id="808b9-203">Для сообщений электронной почты не будет появляться **предупреждение** во время пакетной обработки.</span><span class="sxs-lookup"><span data-stu-id="808b9-203">For email messages, you will not encounter a **Warning** during batch processing.</span></span> <span data-ttu-id="808b9-204">Если **Респонсекласс** **успешно**, элемент [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , который следует за ним, также всегда имеет значение " **Ошибка**".</span><span class="sxs-lookup"><span data-stu-id="808b9-204">If the **ResponseClass** is **Success**, the [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element that follows is also always set to **NoError**.</span></span> <span data-ttu-id="808b9-205">Если **респонсекласс** является **ошибкой**, необходимо проверить значения элементов [мессажетекст](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **респонсекоде**и [мессажексмл](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) , чтобы определить, что привело к проблеме.</span><span class="sxs-lookup"><span data-stu-id="808b9-205">If the **ResponseClass** is **Error**, you need to check the values of the [MessageText](https://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**, and [MessageXml](https://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) elements to determine what caused the problem.</span></span> <span data-ttu-id="808b9-206">[Дескриптивелинккэй](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) в настоящее время не используется.</span><span class="sxs-lookup"><span data-stu-id="808b9-206">[DescriptiveLinkKey](https://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) is currently unused.</span></span>

## <a name="see-also"></a><span data-ttu-id="808b9-207">См. также</span><span class="sxs-lookup"><span data-stu-id="808b9-207">See also</span></span>


- [<span data-ttu-id="808b9-208">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="808b9-208">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)

- [<span data-ttu-id="808b9-209">Отправка сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="808b9-209">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="808b9-210">Ответ на сообщения электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="808b9-210">Respond to email messages by using EWS in Exchange</span></span>](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="808b9-211">Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="808b9-211">Move and copy email messages by using EWS in Exchange</span></span>](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)

- [<span data-ttu-id="808b9-212">Влияние регулирования на пакетные запросы EWS</span><span class="sxs-lookup"><span data-stu-id="808b9-212">Throttling implications for EWS batch requests</span></span>](ews-throttling-in-exchange.md#throttling-implications-for-ews-batch-requests)
