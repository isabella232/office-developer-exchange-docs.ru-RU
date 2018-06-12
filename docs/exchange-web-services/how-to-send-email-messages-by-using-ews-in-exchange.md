---
title: Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 5290fafe-8b51-4275-a27e-baf497fc969c
description: Узнайте, как отправлять сообщения электронной почты нового или черновой или отправить сообщение отложенный электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: f09babfcc420d4cbc563ed6605ba555fd9f8c7e9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761108"
---
# <a name="send-email-messages-by-using-ews-in-exchange"></a>Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange

Узнайте, как отправлять сообщения электронной почты нового или черновой или отправить сообщение отложенный электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Будет ли вы используете управляемый API EWS или веб-служб Exchange, могут отправлять сообщения электронной почты двумя способами. Можно либо отправить существующее сообщение, такие как сообщения, хранящиеся в папке «Черновики», или можно создать и отправить сообщение электронной почты в один шаг. Методы и операции, которые можно использовать для отправки сообщения одинаковы ли вы сразу же отправки сообщения, отправка отложенные сообщения.
  
**В таблице 1. Управляемый API EWS методы и операций веб-служб Exchange для отправки сообщений электронной почты**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Отправьте новое сообщение электронной почты  <br/> |[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|Отправьте сообщение электронной почты существующего  <br/> |[EmailMessage.Send](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) <br/> |[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) <br/> |
   
## <a name="send-a-new-email-message-by-using-the-ews-managed-api"></a>Отправьте новое сообщение электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_sendnewewsma"> </a>

В следующем примере кода показано, как использовать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты и метод [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) , чтобы отправить сообщение получателю и сохраните сообщение в папке «Отправленные». 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="send-a-new-email-message-by-using-ews"></a>Отправьте новое сообщение электронной почты с помощью веб-служб Exchange
<a name="bk_sendnewews"> </a>

В следующем примере кода показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) со значением **MessageDisposition** **SendAndSaveCopy** создавать сообщения электронной почты, отправить сообщение получателю, и сохранять сообщения в папке «Отправленные». Это также запроса XML, что управляемый API EWS отправляет при [Отправьте новое сообщение электронной почты](#bk_sendnewewsma).
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно создан, и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из вновь сообщение о создании. 
  
## <a name="send-a-draft-email-message-by-using-the-ews-managed-api"></a>Отправлять черновики по электронной почте с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_senddraftewsma"> </a>

В следующем примере кода показано, как отправить сообщение, в котором была сохранена в папке «Черновики», как показано в разделе [Создание сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange](email-and-ews-in-exchange.md#bk_createewsma). Во-первых используйте метод [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) для получения сообщений и используйте метод [Send](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.send%28v=exchg.80%29.aspx) для отправки сообщений электронной почты, как показано в следующем примере кода. Обратите внимание, что этот метод не сохраняет отправленное сообщение в папку «Отправленные». 
  
В этом случае свойства [EmailMessageSchema.Subject](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema.subject%28v=exchg.80%29.aspx) и [EmailMessageSchema.ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.torecipients%28v=exchg.80%29.aspx) добавляются [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) , чтобы значения, которые могут быть включены в выходные данные консоли. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="send-a-draft-email-message-by-using-ews"></a>Отправлять черновики по электронной почте с помощью веб-служб Exchange
<a name="bk_senddraftews"> </a>

В следующих примерах кода показано, как отправить сообщение, которое ранее было сохранено в папке «Черновики», как показано в разделе [Создание сообщения электронной почты с помощью веб-служб Exchange](email-and-ews-in-exchange.md#bk_createews). Сначала с помощью операции [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения сообщений электронной почты для отправки. Затем с помощью операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) отправить сообщение электронной почты для получателей и сохранение его в папку «Отправленные». 
  
Первое сообщение сообщении с запросом **GetItem** , указывает [идентификатор элемента](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) черновика сообщения электронной почты для привязки к и элементы в элементе [ItemShape](http://msdn.microsoft.com/library/c5604161-bbc0-40bc-ad75-ff7e837d745f%28Office.15%29.aspx) ограничить результаты для включения в **GetItem** ответа. Элемент **ItemShape** имеет [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx) из **IdOnly**, после чего элемент [AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx) включает в себя [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) значения для свойства **темы** из схемы элемента и **ToRecipients** свойство из схемы сообщений, которая означает, что только **ItemId**, [теме](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx)и [ToRecipients](http://msdn.microsoft.com/library/72dc3be8-30bb-4ae1-acf4-fb94ff490631%28Office.15%29.aspx) элементы будут возвращены клиенту в ответе. Дополнительные сведения об ограничении значений, возвращенных в вызовах и значение элемента, **BaseShape** видеть [наборы свойств и ответ с фигурами в веб-служб Exchange в Exchange](property-sets-and-response-shapes-in-ews-in-exchange.md).
  
Это также запроса XML, отправляемого управляемый API EWS при вызове метода [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) . Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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

В следующем примере показано XML-ответ, что сервер возвращает после обработки операции **GetItem** . Ответ указывает, что сообщение электронной почты был успешно извлечен и содержит **тему** и **ToRecipient** элементы по запросу. Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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

Второе сообщение сообщения запроса **SendItem** указывает [идентификатор элемента](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) для сообщения электронной почты для отправки, а также [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx), который определяет папку, в которой требуется сохранить отправленное сообщение.
  
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

Сервер отвечает на запрос **SendItem** [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты было успешно отправлено.
  
## <a name="send-a-delayed-email-message-by-using-the-ews-managed-api"></a>Отправка сообщения электронной почты отложенный с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_senddelayedewsma"> </a>

В следующем примере кода показано, как использовать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) для создания сообщения электронной почты, класс [ExtendedPropertyDefinition](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.extendedpropertydefinition%28v=exchg.80%29.aspx) для создания определения свойства для свойства [PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) (0x3FEF0040) и Метод [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) отправьте отложенные сообщения и сохраните сообщение в папке «Отправленные». 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. 
  
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

## <a name="send-a-delayed-email-message-by-using-ews"></a>Отправка сообщения электронной почты отложенный с помощью веб-служб Exchange
<a name="bk_senddelayedews"> </a>

В следующем примере кода показано, как создавать сообщения электронной почты, элемент [ExtendedProperty](http://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) для создания определения свойства для [с помощью операции [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) со значением **MessageDisposition** **SendAndSaveCopy** PidTagDeferredSendTime](http://msdn.microsoft.com/en-us/library/cc840017.aspx) свойство (0x3FEF0040), чтобы задать время для отправки сообщения и элемент [SavedItemFolderId](http://msdn.microsoft.com/library/4b8b475c-9ca5-48c9-acb0-8848b53be1ce%28Office.15%29.aspx) Сохранить отправленное сообщение в папку «Отправленные». 
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно создан, и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из вновь сообщение о создании. 
  
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Ответ на сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    

