---
title: Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Узнайте, как создание, получение, обновление и удаление пакетов сообщений электронной почты в одном вызове с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 30ebbdf4c92111df629c7662987e301d167336e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761121"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Обрабатывать сообщения электронной почты в пакетах с помощью веб-служб Exchange в Exchange

Узнайте, как создание, получение, обновление и удаление пакетов сообщений электронной почты в одном вызове с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно использовать управляемый API EWS или делает веб-служб Exchange для работы с пакетами сообщений электронной почты, чтобы сократить количество вызовов клиента к серверу Exchange. При использовании управляемого интерфейса API веб-служб Exchange для создания, получение, обновление, удаление и отправлять сообщения в пакетах используйте методы объекта [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , то время как при работе с сообщениями одного адреса электронной почты, можно использовать методы объекта [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . При использовании веб-служб Exchange для работы с одним и пакетов сообщений электронной почты использовать такие же операции. 
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для работы с пакетов сообщений электронной почты**

|**Чтобы...**|**Используйте этот метод управляемый API EWS**|**Используйте эту операцию EWS**|
|:-----|:-----|:-----|
|Создание сообщения электронной почты в пакетах  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Получение сообщений электронной почты в пакетах  <br/> |[ExchangeService.BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Обновление сообщений электронной почты в пакетах  <br/> |[ExchangeService.UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление сообщений электронной почты в пакетах  <br/> |[ExchangeService.DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
В этой статье вы узнаете, как для выполнения основных задач для пакетов сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>Создание сообщения электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_createewsma"> </a>

Сообщения в пакетах можно создать с помощью метода управляемый API EWS **CreateItems** , как показано в следующем примере. В этом примере создается три объекта [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) локально, добавляет в коллекцию каждого сообщения, а затем вызывается метод **CreateItems** набор сообщений. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

Обратите внимание на то, что в примере сохраняется только сообщения в папке "Черновики"; не отправляет сообщения. Для получения дополнительных сведений об отправке сообщений см [отправлять сообщения электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange](#bk_sendewsma).
  
## <a name="create-email-messages-in-batches-by-using-ews"></a>Создание сообщения электронной почты в пакетах с помощью веб-служб Exchange
<a name="bk_createews"> </a>

Сообщения электронной почты в пакетах можно создать с помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, как показано в следующем примере кода. Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [создания сообщений электронной почты в пакетах](#bk_createewsma). 
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** для каждого нового сообщения, которые указывает, что каждое сообщение электронной почты был создан успешно сохранены . 
  
Обратите внимание на то, что в примере сохраняется только сообщения в папке "Черновики"; не отправляет сообщения. Для получения дополнительных сведений об отправке сообщений см [отправлять сообщения электронной почты в пакетах с помощью веб-служб Exchange](#bk_sendews).
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>Отправлять сообщения электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_sendewsma"> </a>

Используйте тот же код для отправки сообщений электронной почты в пакетах, используемые для создания сообщений электронной почты в пакетах, за исключением того, что некоторые параметры метода [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) изменить. Таким образом для отправки сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange, используйте код, который используется для [создания сообщений электронной почты в пакетах](#bk_createewsma)и замените вызов метода **CreateItems** звонок в следующем примере. В этом примере сообщений создаются в папке «Отправленные» и ликвидации сообщения изменяется на [MessageDisposition.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), чтобы отправлено сообщение, а не только локального сохранения.
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>Отправлять сообщения электронной почты в пакетах с помощью веб-служб Exchange
<a name="bk_sendews"> </a>

Используйте тот же код для отправки сообщений электронной почты в пакетах, что используется для создания сообщений электронной почты в пакетах, за исключением того, что для операции **CreateItem** изменить несколько значений атрибутов. Таким образом, для отправки сообщений электронной почты с помощью веб-служб Exchange, используйте код используется для [создания сообщения электронной почты в пакетах](#bk_createews)и **MessageDisposition** значение изменяется на «SendAndSaveCopy» и измените [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) для папки "Отправленные «"», как показано в Следующий пример кода. 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** для каждого нового сообщения, которые указывает, что каждое сообщение электронной почты был создан и отправлен успешно. 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>Получение сообщений электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_getewsma"> </a>

Сообщения электронной почты в пакетах можно получить с помощью метода управляемый API EWS [BindToItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) , как показано в следующем примере. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="get-email-messages-in-batches-by-using-ews"></a>Получение сообщений электронной почты в пакетах с помощью веб-служб Exchange
<a name="bk_getews"> </a>

Сообщения электронной почты в пакетах можно получить с помощью операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) веб-служб Exchange и код в следующем примере. Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API EWS для [получения сообщений электронной почты в пакетах](#bk_getewsma). 
  
Атрибуты **ItemId** и **ChangeKey** URL-были сокращены для удобства чтения. 
  
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

Сервер отвечает на запрос **GetItem** [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) сообщение, содержащее [первого класса свойства](email-properties-and-elements-in-ews-in-exchange.md) для каждого из запрошенного сообщения. 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>Обновление сообщений электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_updateewsma"> </a>

Сообщения электронной почты в пакетах можно получить с помощью метода управляемый API EWS [UpdateItems](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) , как показано в следующем примере. 
  
Список свойств сообщения электронной почты для записи в разделе [электронной почты свойства и элементы в веб-служб Exchange в Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Для получения дополнительных сведений о том, как отправить черновик сообщения после его обновляется видеть [Отправка сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange](#bk_sendewsma).
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="update-email-messages-in-batches-by-using-ews"></a>Обновление сообщений электронной почты в пакетах с помощью веб-служб Exchange
<a name="bk_updateews"> </a>

Сообщения электронной почты в пакетах можно обновить с помощью операции [Getitem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) , как показано в следующем примере кода. Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API EWS для [сообщений электронной почты в пакетах обновления](#bk_updateewsma).
  
Список элементов сообщения электронной почты для записи в разделе [электронной почты свойства и элементы в веб-служб Exchange в Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Для получения дополнительных сведений о том, как отправить черновик сообщения после его обновляется видеть [отправлять черновики по электронной почте с помощью веб-служб Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
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

Сервер отвечает на запрос **UpdateItem** с [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) сообщения, которое содержит значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что каждый из обновления успешно сохранен на сервере. В элементе [ConflictResult](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) выводятся все конфликты. 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>Удаление сообщений электронной почты в пакетах с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_deleteewsma"> </a>

Сообщения в пакетах можно удалить с помощью метода управляемый API EWS [DeleteItems](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) , как показано в следующем примере. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="delete-email-messages-in-batches-by-using-ews"></a>Удаление сообщений электронной почты в пакетах с помощью веб-служб Exchange
<a name="bk_deleteews"> </a>

Сообщения электронной почты в пакетах можно удалить с помощью операции [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) EWS, как показано в следующем примере кода. Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API веб-служб Exchange для [удаления сообщений электронной почты в пакетах](#bk_deleteewsma).
  
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

Сервер отвечает на запрос **DeleteItem** [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError** для каждого элемента, который был удален. Обратите внимание, что операция также возвращает успех, если не удалось найти идентификатор элемента. 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a>Проверка успешного завершения процесса пакетной обработки
<a name="bk_successful"> </a>

Когда один или несколько сообщений электронной почты в пакетной запросов не может обработать по запросу, возвращается сообщение об ошибке для каждого сообщения электронной почты, который не удалось и остальную часть сообщения электронной почты в пакете обрабатываются как ожидалось. В пакетной обработке могут возникнуть ошибки при элемент был удален и таким образом не может быть отправлено, получить или обновлены, а также если элемент перемещен в другую папку и поэтому имеет новый идентификатор элемента и не могут быть изменены с Идентификатором элемента отправлено. Сведения, приведенные в этом разделе показано, как получить дополнительные сведения об ошибке о сбоях в пакетной обработке сообщения электронной почты.
  
Чтобы проверить успешность пакетной обработки с помощью управляемого интерфейса API веб-служб Exchange, можно проверить, что свойство [OverallResult](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) [ServiceResponseCollection](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) равен [ServiceResult.Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). Если это так, все сообщения электронной почты обработаны успешно. Если **OverallResult** не равно **ServiceResult.Success**, один или несколько сообщений не были успешно обработаны. Каждый из объектов, возвращаемых **ServiceResponseCollection** содержит следующие свойства: 
  
- [Код ошибки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [ErrorDetails](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [Сообщение об ошибке](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [ErrorProperties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [Результат](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
Эти свойства содержат сведения о почему сообщения электронной почты не удается обработать по запросу. Примеры в этой статье распечатать **результатов**, **код ошибки**и **сообщение об ошибке** для каждого сообщение об ошибке. Эти результаты можно использовать для изучения проблемы. 
  
Для веб-служб Exchange Чтобы убедиться в успешности процесса пакетной, проверьте атрибут [ResponseClass](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) для каждого элемента, обрабатываемых. Ниже приведен базовая структура **ResponseMessageType**, базового типа, из которых все ответа полученных сообщений. 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

Если сообщение электронной почты не был успешно обработан атрибут **ResponseClass** , значение **Success** Если сообщение электронной почты было обработано успешно или **ошибки** . Для сообщений электронной почты не возникает **Предупреждение** во время пакетной обработки. Если **ResponseClass** **Успех**, элемент [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , исходя из также всегда имеет значение **NoError**. Если **ResponseClass** **ошибки**, необходимо проверить значения [MessageText](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **ResponseCode**и [MessageXml](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) элементы, чтобы определить причину ошибки. [DescriptiveLinkKey](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) не в настоящее время используется. 
  
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Регулирование последствия для запросов пакетов веб-служб Exchange](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

