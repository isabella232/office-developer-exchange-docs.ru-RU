---
title: Получение вложений с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: 12ce3cc0-a201-42e4-93e1-1f57961ff711
description: Узнайте, как получить вложения из элементов EWS с помощью управляемого API EWS или протокола EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: de3e3ebfbcb16935130203dfed50f255bd59be7b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528085"
---
# <a name="get-attachments-by-using-ews-in-exchange"></a>Получение вложений с помощью EWS в Exchange

Узнайте, как получить вложения из элементов EWS с помощью управляемого API EWS или протокола EWS в Exchange.
  
Получить вложения из элемента можно с помощью управляемого API EWS или веб-служб EWS. Извлечение вложений всегда проходит в два этапа, поскольку исходный вызов для получения элемента содержит только метаданные о коллекции вложений элемента. Сперва необходимо извлечь объект, а затем — вложение.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для добавления вложений**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Получение вложений элемента  <br/> |[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и [ItemAttachment.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemattachment.load%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) и [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
|Получение файловых вложений  <br/> |[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) и [FileAttachment.Load](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.fileattachment.load%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) и [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) <br/> |
   
## <a name="get-attachments-from-an-email-by-using-the-ews-managed-api"></a>Извлечение вложений из электронного письма с помощью управляемого API EWS
<a name="bk_getattachewsma"> </a>

The following code example shows how to get an [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) object by using the **Bind** method, then iterate through the attachment collection and call the **FileAttachment.Load** or **ItemAttachment.Load** method on each attachment as appropriate. Each file attachment is saved to the C:\temp\ folder, and each item attachment is loaded into memory. For information about how to save an item attachment, see [Save an attached email by using the EWS Managed API](#bk_saveitemattach).
  
В этом примере предполагается, что **service** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), что **itemId** является классом [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого будут извлекаться вложения, а также что пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
public static void GetAttachmentsFromEmail(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and load each attachment.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is FileAttachment)
        {
            FileAttachment fileAttachment = attachment as FileAttachment;
            // Load the attachment into a file.
            // This call results in a GetAttachment call to EWS.
            fileAttachment.Load("C:\\temp\\" + fileAttachment.Name);
           
            Console.WriteLine("File attachment name: " + fileAttachment.Name);
        }
        else // Attachment is an item attachment.
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            // Load attachment into memory and write out the subject.
            // This does not save the file like it does with a file attachment.
            // This call results in a GetAttachment call to EWS.
            itemAttachment.Load();
            Console.WriteLine("Item attachment name: " + itemAttachment.Name);
        }
    }
}
```

## <a name="get-an-attachment-from-an-email-by-using-ews"></a>Извлечение вложения из электронного письма с помощью EWS
<a name="bk_getattachewsma"> </a>

Для извлечения вложения с помощью EWS сперва нужно извлечь сообщение и коллекцию вложений, чтобы получить элемент [Идентификатора вложения AttachmentId (GetAttachment и DeleteAttachment)](https://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) вложения, которое необходимо извлечь. Получив одно или несколько значений **AttachmentId** для извлечения, вызовите операцию [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx), чтобы загрузить все свойства вложения. 
  
В следующем примере кода показано, как использовать операцию [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения сообщения электронной почты и коллекции вложений сообщения. Кроме того, этот код представляет собой первый XML-запрос, посылаемый управляемым API EWS, если с его помощью [получаете вложения из письма](#bk_getattachewsma). Значения некоторых атрибутов укорочены для удобства чтения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange207_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Attachments" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="ERu/AAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

В ответ на запрос **GetItem** сервер отправляет сообщение [GetItemResponse](https://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx), содержащее элемент [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении письма) и значения [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) существующих вложений. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="ERu/AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAYEMnd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="5zTzlqU=" />
                  <t:Name>FileAttachment.txt</t:Name>
                  <t:Size>212</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                  <t:IsContactPhoto>false</t:IsContactPhoto>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="Ktum21o=" />
                  <t:Name>Attached Message Item</t:Name>
                  <t:Size>3063</t:Size>
                  <t:LastModifiedTime>2014-05-14T17:59:30</t:LastModifiedTime>
                  <t:IsInline>false</t:IsInline>
                </t:ItemAttachment>
              </t:Attachments>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>

```

Теперь, когда у вас есть значения [AttachmentId](https://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx), вызовите операцию [GetAttachment](https://msdn.microsoft.com/library/24d10a15-b942-415e-9024-a6375708f326%28Office.15%29.aspx) для всех вложений, которые необходимо извлечь. 
  
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
    <m:GetAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="5zTzlqU=" />
      </m:AttachmentIds>
    </m:GetAttachment>
  </soap:Body>
</soap:Envelope>
```

При извлечении только элемента вложения в ответ на запрос **GetAttachment** сервер отправляет сообщение [GetAttachmentResponse](https://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx), содержащее элемент [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении вложения) и все элементы элемента вложения, т. е. сообщения электронной почты.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="Ktum21o=" />
              <t:Name>Attached Message Item</t:Name>
              <t:Message>
                <t:ItemClass>IPM.Note</t:ItemClass>
                <t:Subject>Message Item Subject</t:Subject>
                <t:Body BodyType="HTML">&amp;lt;meta http-equiv="Content-Type" 
                    content="text/html; charset=utf-8"&amp;gt;Message Item Body</t:Body>
                <t:Size>2859</t:Size>
                <t:IsSubmitted>false</t:IsSubmitted>
                <t:IsDraft>true</t:IsDraft>
                <t:IsFromMe>false</t:IsFromMe>
                <t:IsResend>false</t:IsResend>
                <t:IsUnmodified>false</t:IsUnmodified>
                <t:DateTimeCreated>2014-05-14T17:59:37Z</t:DateTimeCreated>
                <t:ResponseObjects>
                  <t:ForwardItem />
                </t:ResponseObjects>
                <t:DisplayCc />
                <t:DisplayTo>primary; emaildelegate</t:DisplayTo>
                <t:HasAttachments>false</t:HasAttachments>
                <t:Culture>en</t:Culture>
                <t:EffectiveRights>
                  <t:CreateAssociated>false</t:CreateAssociated>
                  <t:CreateContents>false</t:CreateContents>
                  <t:CreateHierarchy>false</t:CreateHierarchy>
                  <t:Delete>true</t:Delete>
                  <t:Modify>true</t:Modify>
                  <t:Read>true</t:Read>
                </t:EffectiveRights>
                <t:LastModifiedName>primary</t:LastModifiedName>
                <t:LastModifiedTime>2014-05-14T17:59:30Z</t:LastModifiedTime>
                <t:IsAssociated>false</t:IsAssociated>
                <t:WebClientReadFormQueryString>?ItemID=AAMk3D&amp;amp;exvsurl=1&amp;amp;viewmodel=
                    ReadMessageItem</t:WebClientReadFormQueryString>
                <t:ConversationId Id="AAQkADIwM2ZlM2ZlLWMwYjctNDg2N/Rc+d0=" />
                <t:ToRecipients>
                  <t:Mailbox>
                    <t:Name>primary</t:Name>
                    <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                  <t:Mailbox>
                    <t:Name>emaildelegate</t:Name>
                    <t:EmailAddress>ronnie@contoso.com</t:EmailAddress>
                    <t:RoutingType>SMTP</t:RoutingType>
                    <t:MailboxType>Mailbox</t:MailboxType>
                  </t:Mailbox>
                </t:ToRecipients>
                <t:IsReadReceiptRequested>false</t:IsReadReceiptRequested>
                <t:ConversationIndex>AQHPb55BxR5Fm0Arx0yY4xbL9Fz53Q==</t:ConversationIndex>
                <t:ConversationTopic>Message Item Subject</t:ConversationTopic>
                <t:IsRead>true</t:IsRead>
              </t:Message>
            </t:ItemAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

При извлечении вложенного файла в ответ на запрос **GetAttachment** сервер отправляет сообщение [GetAttachmentResponse](https://msdn.microsoft.com/library/cb65f449-309b-4b6e-8d22-d1967135490c%28Office.15%29.aspx), содержащее элемент [ResponseCode](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении вложения) и все элементы вложенного файла.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="5zTzlqU=" />
              <t:Name>FileAttachment.txt</t:Name>
              <t:Content>VGhpcyBpcyBhIGZpbGUgYXR0YWNobWVudC4=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:GetAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="save-an-attached-email-by-using-the-ews-managed-api"></a>Сохранение вложенного сообщения электронной почты с помощью управляемого API EWS
<a name="bk_saveitemattach"> </a>

In order to save the contents of an email attachment using the EWS Managed API, you need to save the [MimeContent](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.mimecontent%28v=exchg.80%29.aspx) to a file. In doing so, you will lose any extended properties set on the item, such as follow-up flags and categories. This example saves the email attachment to the to the C:\temp\ folder. 
  
Обратите внимание, что вам не удастся переместить или скопировать вложение в другую папку, так как элемент вложения не является строго типизированным. Поэтому если нужно переместить вложение в другую папку, используйте приведенный ниже пример кода, а затем [импортируйте файл](how-to-import-items-by-using-ews-in-exchange.md) в другую папку. 
  
```cs
public static void SaveEmailAttachment(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message item and retrieve the attachments collection.
    // This method results in an GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment is ItemAttachment)
        {
            ItemAttachment itemAttachment = attachment as ItemAttachment;
            itemAttachment.Load(ItemSchema.MimeContent);
            string fileName = "C:\\Temp\\" + itemAttachment.Item.Subject + ".eml";
            // Write the bytes of the attachment into a file.
            File.WriteAllBytes(fileName, itemAttachment.Item.MimeContent.Content);
            Console.WriteLine("Email attachment name: "+ itemAttachment.Item.Subject + ".eml");
        }
    }
}
```

## <a name="see-also"></a>См. также


- [Вложение и EWS в Exchange](attachments-and-ews-in-exchange.md)
    
- [Добавление вложений с помощью EWS в Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Удаление вложений с помощью EWS в Exchange](how-to-delete-attachments-by-using-ews-in-exchange.md)
    

