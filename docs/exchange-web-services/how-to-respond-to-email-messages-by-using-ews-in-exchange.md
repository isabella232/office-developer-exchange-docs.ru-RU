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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761110"
---
# <a name="respond-to-email-messages-by-using-ews-in-exchange"></a>Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange

Узнайте, как отвечать на сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Чтобы ответить на сообщения, отвечая на них или пересылать их получателей можно использовать управляемый API EWS или веб-служб Exchange.
  
**В таблице 1. Управляемый API EWS методы и операции EWS для ответа на сообщения электронной почты**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Ответ на сообщение электронной почты  <br/> |[EmailMessage.Reply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> [EmailMessage.CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), где элемент [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) имеет дочерний элемент [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) или [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx).  <br/> |
|Пересылать сообщения электронной почты  <br/> |[EmailMessage.Forward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) <br/> [EmailMessage.CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx), где элемент [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) имеет дочерний элемент [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx).  <br/> |
   
## <a name="reply-to-an-email-message-by-using-the-ews-managed-api"></a>Ответ на сообщение электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_replyewsma"> </a>

Управляемый API веб-служб Exchange предоставляет два метода, которые можно использовать для ответа на сообщения: [ответ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) и [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx). Метод **ответа** только используются два входных параметра: ответное сообщение в начале существующий текст и **логическое** значение, указывающее, является ли ответ должен приходить для всех получателей (true) или просто отправителя (false). Если требуется добавить дополнительных получателей на сообщение задавать дополнительные свойства в ответ, или добавить вложение, используйте метод **CreateReply** , который позволяет задать все [первого класса свойства](email-properties-and-elements-in-ews-in-exchange.md) , доступные на [EmailMessage ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)объект. 
  
В следующем примере кода показано, как использовать метод **ответ** в ответ на сообщение электронной почты. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *ItemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента реагировать на. В примере вызывается [метод FindRecentlySent](#bk_findlast) , чтобы убедиться, что сообщение помечено как ответ. 
  
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

В следующем примере кода показано, как использовать метод **CreateReply** отвечать на сообщения электронной почты. 
  
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

Если необходимо добавить вложения в сообщении ответа, замените вызов метода **SendAndSaveCopy** следующий код. 
  
```cs
EmailMessage reply = responseMessage.Save();
reply.Attachments.AddFileAttachment("attachmentname.txt");
reply.Update(ConflictResolutionMode.AutoResolve);
reply.SendAndSaveCopy();
```

## <a name="reply-to-an-email-message-by-using-ews"></a>Ответ на сообщение электронной почты с помощью веб-служб Exchange
<a name="bk_replyews"> </a>

В следующем примере кода показано, как отвечать на сообщения с помощью веб-служб Exchange. С помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с атрибутом **MessageDisposition** , равным **SendAndSaveCopy** отправлять сообщения и сохранения ответа в папке «Отправленные». Включить элемент [ReplyAllToItem](http://msdn.microsoft.com/library/8ca970ca-ca73-40db-9233-7b271cc5f44f%28Office.15%29.aspx) в качестве дочерних [элементов](http://msdn.microsoft.com/library/d61ef1cc-ddfc-480a-9625-7b436cb33ae0%28Office.15%29.aspx) элемента ответить всем на сообщение потока или включить элемент [ReplyToItem](http://msdn.microsoft.com/library/35ee751a-41c0-4216-ad8b-78f7ada43a2f%28Office.15%29.aspx) отвечать только для отправителя. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове [ответ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) или метод [CreateReply](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createreply%28v=exchg.80%29.aspx) . 
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что ответ был создан и отправлен успешно.
  
Если необходимо добавить вложения в ответное сообщение вызова операции **CreateItem** , как указано выше, но измените **MessageDisposition** на **SaveOnly**. Затем вызовите операцию [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , а затем операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) . 
  
## <a name="forward-an-email-message-by-using-the-ews-managed-api"></a>Пересылать сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_forwardewsma"> </a>

Управляемый API веб-служб Exchange предоставляет два метода, которые можно использовать для пересылки сообщений: [вперед](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) и [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx). Метод **переадресовывать** только используются два входных параметра: сообщение, чтобы в начале существующий текст и массив или коллекцию получателей, в зависимости от того, используется перегруженный метод. Если необходимо добавить вложения в сообщение в случае переадресации или задавать дополнительные свойства для нового сообщения, используйте метод **CreateForward** , который позволяет задать все свойства, доступные в объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) . 
  
В следующем примере кода показано, как использовать метод **переадресовывать** пересылать сообщения электронной почты для одного получателя. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *ItemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для пересылки. В примере вызывается [метод FindRecentlySent](#bk_findlast) , убедитесь, что сообщение помечено как пересылку. 
  
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

В следующем примере кода показано, как использовать метод **CreateForward** пересылать сообщения электронной почты для одного получателя. 
  
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

Если требуется добавить вложение в переадресованных сообщений, замените вызов метода **SendAndSaveCopy** следующий код. 
  
```cs
EmailMessage forward = forwardMessage.Save();
forward.Attachments.AddFileAttachment("attachmentname.txt");
forward.Update(ConflictResolutionMode.AutoResolve);
forward.SendAndSaveCopy();
```

## <a name="forward-an-email-message-by-using-ews"></a>Пересылать сообщения электронной почты с помощью веб-служб Exchange
<a name="bk_forwardews"> </a>

В следующем примере кода показано, как пересылать сообщение с помощью веб-служб Exchange. С помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) с атрибутом **MessageDisposition** , равным **SendAndSaveCopy** отправлять сообщения и сохранения ответа в папке «Отправленные». Элемент [ForwardItem](http://msdn.microsoft.com/library/97786086-8b91-4471-8af8-d21e8d66de87%28Office.15%29.aspx) указывает, что элемент переадресованных сообщений. 
  
Это также XML-запрос, который отправляет управляемый API EWS при вызове [вперед](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.forward%28v=exchg.80%29.aspx) или метод [CreateForward](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.createforward%28v=exchg.80%29.aspx) . 
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что переадресованных сообщений был создан и отправлен успешно.
  
Если необходимо добавить вложения в ответное сообщение вызова операции **CreateItem** , но измените **MessageDisposition** на **SaveOnly**. Затем вызовите операцию [CreateAttachment](http://msdn.microsoft.com/library/e066db95-6963-4507-a8d0-8efad287f550%28Office.15%29.aspx) , а затем операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) . 
  
## <a name="find-the-message-last-replied-to-or-forwarded-by-using-the-ews-managed-api"></a>Найдите сообщение последнего или задачи с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_findlast"> </a>

В следующем примере кода показано, как найти последнего выполнения команды и время последнего глаголов выполнен на указанный элемент. Этот метод вызывается из других примеров кода, управляемый API EWS в этом разделе, чтобы подтвердить, что элементы вы или задачи были помечается как ответ или перенаправлять в папку "Входящие". 
  
В примере используется свойство [PidTagLastVerbExecuted](http://msdn.microsoft.com/en-us/library/cc841968.aspx) (0x10820003) расширенные для определения необходимости сообщение было ответ, ответить всем или прямого и [PidTagLastVerbExecutionTime](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x10820040) расширенные свойства, чтобы определить, когда ответить или переслать было отправлено. 
  
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

## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

