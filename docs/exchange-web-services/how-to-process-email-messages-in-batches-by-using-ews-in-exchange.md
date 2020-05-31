---
title: Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 96390f92-cab1-4de6-9ec2-a55678fc20af
description: Узнайте, как создавать, получать, обновлять и удалять пакеты сообщений электронной почты в едином вызове с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: b7dcc8f0961a34061b0476e2136193bf21731d99
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354045"
---
# <a name="process-email-messages-in-batches-by-using-ews-in-exchange"></a>Обработка сообщений электронной почты в пакетах с помощью EWS в Exchange

Узнайте, как создавать, получать, обновлять и удалять пакеты сообщений электронной почты в едином вызове с помощью управляемого API EWS или EWS в Exchange.
  
Вы можете использовать управляемый API EWS или EWS для работы с пакетами сообщений электронной почты, чтобы уменьшить количество звонков, которые клиент делает на сервер Exchange Server. При использовании управляемого API EWS для создания, получения, обновления, удаления и отправки сообщений в пакетах используются методы объекта [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а при работе с отдельными сообщениями электронной почты используются методы объекта [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . Если вы используете EWS, вы можете использовать те же операции для работы с одним и пакетными сообщениями электронной почты. 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для работы с пакетами сообщений электронной почты**

|**Задача**|**Используйте этот метод управляемого API EWS**|**Используйте эту операцию EWS**|
|:-----|:-----|:-----|
|Создание сообщений электронной почты в пакетах  <br/> |[ExchangeService. CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Получение сообщений электронной почты в пакетах  <br/> |[ExchangeService. Биндтоитемс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|Обновление сообщений электронной почты в пакетах  <br/> |[ExchangeService. Упдатеитемс](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление сообщений электронной почты в пакетах  <br/> |[ExchangeService. Делетеитемс](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
В этой статье рассказывается, как выполнить основные задачи для пакетов сообщений электронной почты с помощью управляемого API EWS или EWS.
  
## <a name="create-email-messages-in-batches-by-using-the-ews-managed-api"></a>Создание сообщений электронной почты в пакетах с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

Вы можете создавать сообщения в пакетах с помощью метода **CreateItems** управляемого API EWS, как показано в следующем примере. В этом примере создаются три объекта [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) локально, каждое сообщение добавляется в коллекцию, после чего вызывается метод **CreateItems** для коллекции сообщений. 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

Обратите внимание, что в этом примере сообщения сохраняются только в папке "Черновики"; сообщения не отправляются. Дополнительные сведения о том, как отправлять сообщения, [можно узнать в статье отправка сообщений электронной почты в пакетах с помощью управляемого API EWS](#bk_sendewsma).
  
## <a name="create-email-messages-in-batches-by-using-ews"></a>Создание сообщений электронной почты в пакетах с помощью EWS
<a name="bk_createews"> </a>

Вы можете создавать сообщения электронной почты в пакетах с помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) EWS, как показано в следующем примере кода. Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [создания сообщений электронной почты в пакетах](#bk_createewsma). 
  
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

Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для каждого** из новых сообщений, что означает, что каждое сообщение было создано и сохранено успешно. 
  
Обратите внимание, что в этом примере сообщения сохраняются только в папке "Черновики"; сообщения не отправляются. Дополнительные сведения о том, как отправлять сообщения, [можно узнать в статье отправка сообщений электронной почты пакетами с помощью EWS](#bk_sendews).
  
## <a name="send-email-messages-in-batches-by-using-the-ews-managed-api"></a>Отправка сообщений электронной почты в пакетах с помощью управляемого API EWS
<a name="bk_sendewsma"> </a>

Один и тот же код используется для отправки сообщений электронной почты в пакетах, которые используются для создания сообщений электронной почты в пакетах, за исключением того, что некоторые параметры метода [CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) меняются. Таким образом, чтобы отправлять сообщения электронной почты с помощью управляемого API EWS, используйте код, используемый для [создания сообщений электронной почты в пакетах](#bk_createewsma), и замените вызов метода **CreateItems** на вызов в приведенном ниже примере. В этом примере сообщения создаются в папке "Отправленные", а расположение сообщения изменяется на [мессажедиспоситион. SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.messagedisposition%28v=exchg.80%29.aspx), поэтому сообщение отправляется, а не просто сохраняется локально.
  
```cs
// Create and send the batch of email messages on the server.
// This method call results in an CreateItem call to EWS.
ServiceResponseCollection<ServiceResponse> response = service.CreateItems(messageItems, WellKnownFolderName.SentItems, MessageDisposition.SendAndSaveCopy, null);
```

## <a name="send-email-messages-in-batches-by-using-ews"></a>Отправка сообщений электронной почты пакетами с помощью EWS
<a name="bk_sendews"> </a>

Один и тот же код используется для отправки сообщений электронной почты в пакетах, которые используются для создания сообщений электронной почты в пакетах, за исключением того, что некоторые значения атрибутов изменяются для операции **CreateItem** . Таким образом, чтобы отправлять сообщения электронной почты с помощью EWS, используйте код, используемый для [создания сообщений электронной почты в пакетах](#bk_createews), и измените значение **Мессажедиспоситион** на "SendAndSaveCopy" и измените [дистингуишедфолдерид](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) на "sentitems", как показано в следующем примере кода. 
  
```XML
<m:CreateItem MessageDisposition="SendAndSaveCopy">
  <m:SavedItemFolderId>
    <t:DistinguishedFolderId Id="sentitems" />
  </m:SavedItemFolderId>
```

Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) для каждого из новых сообщений, что **указывает на то** , что каждое сообщение было создано и отправлено успешно. 
  
## <a name="get-email-messages-in-batches-by-using-the-ews-managed-api"></a>Получение сообщений электронной почты в пакетах с помощью управляемого API EWS
<a name="bk_getewsma"> </a>

Вы можете получать сообщения электронной почты в пакетах с помощью метода [Биндтоитемс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.bindtoitems%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере. 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

## <a name="get-email-messages-in-batches-by-using-ews"></a>Получение сообщений электронной почты в пакетах с помощью EWS
<a name="bk_getews"> </a>

Вы можете получать сообщения электронной почты в пакетах с помощью операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) и кода в приведенном ниже примере. Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [получения сообщений электронной почты в пакетах](#bk_getewsma). 
  
Атрибуты **ItemId** и **чанжекэй** были сокращены для удобочитаемости. 
  
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

Сервер отвечает на запрос **GetItem** с сообщением [жетитемреспонсе](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) , которое включает [свойства первого класса](email-properties-and-elements-in-ews-in-exchange.md) для каждого из запрошенных сообщений. 
  
## <a name="update-email-messages-in-batches-by-using-the-ews-managed-api"></a>Обновление сообщений электронной почты в пакетах с помощью управляемого API EWS
<a name="bk_updateewsma"> </a>

Вы можете получать сообщения электронной почты в пакетах с помощью метода [Упдатеитемс](http://msdn.microsoft.com/en-us/library/dd634705%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере. 
  
Список свойств сообщений электронной почты, доступных для записи, приведен [в статье свойства и элементы электронной почты в EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Сведения о том, как отправить черновик сообщения после его обновления, можно узнать в статье [Отправка сообщений электронной почты с помощью управляемого API EWS](#bk_sendewsma).
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

## <a name="update-email-messages-in-batches-by-using-ews"></a>Обновление сообщений электронной почты в пакетах с помощью EWS
<a name="bk_updateews"> </a>

Вы можете обновлять сообщения электронной почты в пакетах с помощью операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) EWS, как показано в следующем примере кода. Это также запрос XML, который отправляет управляемый API EWS при использовании управляемого API EWS для [обновления сообщений электронной почты в пакетах](#bk_updateewsma).
  
Список доступных для записи элементов сообщения электронной почты приведен [в статье свойства и элементы электронной почты в веб EWS в Exchange](email-properties-and-elements-in-ews-in-exchange.md).
  
Сведения о том, как отправить черновик сообщения после его обновления, можно узнать в статье [Отправка черновика сообщения электронной почты с помощью EWS](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews).
  
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

Сервер отвечает на запрос **UpdateItem** с сообщением [упдатеитемреспонсе](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , указывающее на то **, что**все обновления успешно сохранены на сервере. Все конфликты включаются в элемент [конфликтресулт](http://msdn.microsoft.com/library/08cdd547-4de7-4c7a-b60f-e618dc217d20%28Office.15%29.aspx) . 
  
## <a name="delete-email-messages-in-batches-by-using-the-ews-managed-api"></a>Удаление сообщений электронной почты в пакетах с помощью управляемого API EWS
<a name="bk_deleteewsma"> </a>

Вы можете удалять сообщения в пакетах с помощью метода [Делетеитемс](http://msdn.microsoft.com/en-us/library/dd635460%28v=exchg.80%29.aspx) управляемого API EWS, как показано в следующем примере. 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. 
  
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

## <a name="delete-email-messages-in-batches-by-using-ews"></a>Удаление сообщений электронной почты в пакетах с помощью EWS
<a name="bk_deleteews"> </a>

Вы можете удалять сообщения электронной почты в пакетах с помощью операции [DeleteItem](../web-service-reference/deleteitem-operation.md) EWS, как показано в следующем примере кода. Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [удаления сообщений электронной почты в пакетах](#bk_deleteewsma).
  
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

Сервер отвечает на запрос **DeleteItem** с сообщением [делетеитемреспонсе](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) , которое содержит значение [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **для удаления для каждого** удаленного элемента. Обратите внимание, что при выполнении операции также возвращается значение Success, если не удалось найти идентификатор элемента. 
  
## <a name="verifying-that-a-batch-process-completed-successfully"></a>Проверка успешного завершения пакетной обработки
<a name="bk_successful"> </a>

Если одно или несколько сообщений электронной почты в пакетном запросе не могут быть обработаны как запрошенные, возвращается ошибка для каждого неудачного сообщения электронной почты, а остальные сообщения в пакете обрабатываются должным образом. Ошибки в пакетной обработке могут возникать, если элемент был удален, поэтому не может быть отправлен, извлечен или обновлен, или если элемент перемещен в другую папку, и поэтому не может быть изменен с помощью идентификатора элемента. В этом разделе показано, как получить сведения об ошибках при пакетной обработке сообщения электронной почты.
  
Чтобы проверить успешность пакетной обработки с помощью управляемого API EWS, можно проверить, что свойство [овераллресулт](http://msdn.microsoft.com/en-us/library/dd634515%28v=exchg.80%29.aspx) объекта [сервицереспонсеколлектион](http://msdn.microsoft.com/en-us/library/dd633715%28v=exchg.80%29.aspx) равно [сервицересулт. Success](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresult%28v=exchg.80%29.aspx). В таком случае все сообщения электронной почты обрабатывались успешно. Если **овераллресулт** не равно **сервицересулт. Success**, одно или несколько сообщений электронной почты не были обработаны успешно. Каждый из объектов, возвращенных в **сервицереспонсеколлектион** , содержит следующие свойства: 
  
- [ErrorCode](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorcode%28v=exchg.80%29.aspx)
    
- [еррордетаилс](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errordetails%28v=exchg.80%29.aspx)
    
- [ErrorMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errormessage%28v=exchg.80%29.aspx)
    
- [еррорпропертиес](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.serviceresponse.errorproperties%28v=exchg.80%29.aspx)
    
- [Результат](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.serviceresponse.result%28v=exchg.80%29.aspx)
    
Эти свойства содержат сведения о том, почему сообщения электронной почты не могут быть обработаны по запросу. В примерах, приведенных в этой статье, распечатываться **результат**, **ErrorCode**и **ErrorMessage** для каждого сообщения, которое не удалось выполнить. Вы можете использовать эти результаты для изучения проблемы. 
  
Для проверки успешности пакетного процесса в EWS проверьте атрибут [респонсекласс](http://msdn.microsoft.com/library/bf57265a-d354-4cd7-bbfc-d93e19cbede6%28Office.15%29.aspx) для каждого обрабатываемого элемента. Ниже приведена базовая структура **респонсемессажетипе**, базовый тип которого является производным от всех ответных сообщений. 
  
```XML
<ResponseMessage ResponseClass="Success | Warning | Error">
            <MessageText/>
            <ResponseCode/>
            <DescriptiveLinkKey/>
            <MessageXml/>
</ResponseMessage>
```

Атрибут **респонсекласс** имеет значение **Success** , если сообщение было обработано успешно, или **Ошибка** , если сообщение не было обработано успешно. Для сообщений электронной почты не будет появляться **предупреждение** во время пакетной обработки. Если **Респонсекласс** **успешно**, элемент [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , который следует за ним, также всегда имеет значение " **Ошибка**". Если **респонсекласс** является **ошибкой**, необходимо проверить значения элементов [мессажетекст](http://msdn.microsoft.com/library/59a23bdc-0d9a-4942-8b3c-9cdb11db1ab1%28Office.15%29.aspx), **респонсекоде**и [мессажексмл](http://msdn.microsoft.com/library/bcaf9e35-d351-48f3-baad-f90c633cba8a%28Office.15%29.aspx) , чтобы определить, что привело к проблеме. [Дескриптивелинккэй](http://msdn.microsoft.com/library/f7f36749-00f3-4915-b17c-e3caa0af6e67%28Office.15%29.aspx) в настоящее время не используется. 
  
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Отправка сообщений электронной почты с помощью EWS в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Ответ на сообщения электронной почты с помощью EWS в Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Влияние регулирования на пакетные запросы EWS](ews-throttling-in-exchange.md#bk_ThrottlingBatch)
    

