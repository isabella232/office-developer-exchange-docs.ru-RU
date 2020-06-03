---
title: Удаление вложений с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Узнайте, как удалять вложения из элементов с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 854f723e9c7452b955d0e7d7a38da7f6224dc8b1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455893"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a>Удаление вложений с помощью EWS в Exchange

Узнайте, как удалять вложения из элементов с помощью управляемого API EWS или EWS в Exchange.
  
Существует несколько вариантов удаления вложенных файлов и элементов из элементов с помощью управляемого API EWS. Вы можете удалить все вложения из сообщения, удалить его по имени или удалить по позиции в коллекции. Для каждого из этих параметров существует метод [аттачментколлектион](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) . 
  
С другой стороны, у вас независимо от того, вы удаляете все вложения из элемента или только из одной, последовательность операций одинакова. В отличие от управляемого API EWS, EWS не включает отдельные операции для удаления в зависимости от имени или положения в массиве вложений.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для удаления вложений**

|**Задача**|**Метод управляемого API EWS**|**Операция EWS**|
|:-----|:-----|:-----|
|Удаление всех вложений из элемента.  <br/> |[Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [аттачментколлектион. Clear](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
|Удаление вложения из элемента по имени.  <br/> |[Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [Аттачментколлектион. Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
|Удаление вложения из элемента по позиции в коллекции.  <br/> |[Item. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [аттачментколлектион. RemoveAt](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](https://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx) <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a>Удаление всех вложений из электронной почты с помощью управляемого API EWS
<a name="bk_deleteattachewsma"> </a>

В приведенном ниже примере кода показано, как удалить все вложения из сообщения электронной почты, выполнив следующие действия:
  
1. С помощью метода [EmailMessage. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).
    
2. Использование метода [аттачментколлектион. Clear](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) для удаления всех вложений из электронной почты. 
    
3. Использование метода [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений. 
    
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , идентификатором **ItemId** является идентификатором [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляются вложения, и что пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
public static void DeleteAllAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Delete all attachments from the message.
    message.Attachments.Clear();
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a>Удаление вложения по имени из сообщения электронной почты с помощью управляемого API EWS
<a name="bk_deleteattachewsma"> </a>

В приведенном ниже примере кода показано, как удалить вложение по имени, выполнив следующие действия:
  
1. С помощью метода [EmailMessage. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).
    
2. Использование метода [аттачментколлектион. Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) для удаления вложения с именем FileAttachment. txt. 
    
3. Использование метода [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений. 
    
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **ItemId** — [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляется вложение, и что пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
public static void DeleteNamedAttachments(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting its attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(ItemSchema.Attachments));
    // Iterate through the attachments collection and delete the attachment named "FileAttachment.txt," if it exists.
    foreach (Attachment attachment in message.Attachments)
    {
        if (attachment.Name == "FileAttachment.txt")
        {
            message.Attachments.Remove(attachment);
            break;
        }
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a>Удаление вложений по положению с помощью управляемого API EWS
<a name="bk_deleteattachewsma"> </a>

В приведенном ниже примере кода показано, как удалить вложение по позиции, выполнив следующие действия:
  
1. С помощью метода [EmailMessage. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) и свойство [EmailMessage. HasAttachments](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) . 
    
2. Использование метода [аттачментколлектион. Remove](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) для удаления первого вложения в коллекции. 
    
3. Использование метода [EmailMessage. Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений. 
    
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **ItemId** — [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляется вложение, и что пользователь прошел проверку подлинности на сервере Exchange. 
  
```cs
public static void DeleteAttachmentByPosition(ExchangeService service, ItemId itemId)
{
    // Bind to an existing message by using its item ID and requesting the HasAttachments property and the attachments collection.
    // This method results in a GetItem call to EWS.
    EmailMessage message = EmailMessage.Bind(service, itemId, new PropertySet(EmailMessageSchema.HasAttachments, ItemSchema.Attachments));
    // Remove attachments using the zero-based index position of the attachment in the attachments collection.
    if (message.HasAttachments)
    {
        message.Attachments.RemoveAt(0);
    }
    // Save the updated message.
    // This method results in an DeleteAttachment call to EWS.
    message.Update(ConflictResolutionMode.AlwaysOverwrite);
}
```

## <a name="delete-attachments-from-an-item-by-using-ews"></a>Удаление вложений из элемента с помощью EWS
<a name="bk_deleteattachewsma"> </a>

Чтобы удалить вложения с помощью EWS, сначала необходимо получить сообщение и коллекцию вложений, чтобы определить [AttachmentId (GetAttachment и DeleteAttachment)](https://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) вложения, которое требуется удалить. После удаления одного или нескольких значений **AttachmentId** вызовите операцию [DeleteAttachment](https://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) , чтобы удалить указанные вложения из сообщения. 
  
В следующем примере кода показано, как использовать операцию [GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения сообщения электронной почты и коллекции вложений сообщения. Кроме того, это первый XML-запрос, который отправляет управляемый API EWS при использовании управляемого API EWS для [удаления всех вложений из электронной почты](#bk_deleteattachewsma). Значения некоторых атрибутов укорочены для удобства чтения.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
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
        <t:ItemId Id="uqE1AAA=" />
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
              <t:ItemId Id="uqE1AAA="
                        ChangeKey="CQAAABYAAAAFI5DJmZv+TLtyLOLIF1S5AAAXulcd" />
              <t:Attachments>
                <t:FileAttachment>
                  <t:AttachmentId Id="IpHLObE=" />
                  <t:Name>FileAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="QuHSSmY=" />
                  <t:Name>SecondAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="qf2KoPo=" />
                  <t:Name>ThirdAttachment.jpg</t:Name>
                </t:FileAttachment>
                <t:FileAttachment>
                  <t:AttachmentId Id="NFQMnMc=" />
                  <t:Name>FourthAttachment.txt</t:Name>
                </t:FileAttachment>
                <t:ItemAttachment>
                  <t:AttachmentId Id="jJvbLXQ=" />
                  <t:Name>Attached Message Item</t:Name>
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

Определив вложение, которое необходимо удалить, вызовите операцию [DeleteAttachment](https://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) и добавьте значения **AttachmentId** для удаляемых вложений. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteAttachment>
      <m:AttachmentIds>
        <t:AttachmentId Id="IpHLObE=" />
        <t:AttachmentId Id="QuHSSmY=" />
        <t:AttachmentId Id="qf2KoPo=" />
        <t:AttachmentId Id="NFQMnMc=" />
        <t:AttachmentId Id="jJvbLXQ=" />
      </m:AttachmentIds>
    </m:DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос DeleteAttachment с сообщением [делетеаттачментреспонсе](https://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx) , которое включает в [себя значение](https://msdn.microsoft.com/library/aa580757%28v=exchg.150%29.aspx) **DeleteAttachment** **для каждого** [делетеаттачментреспонсемессаже](https://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx), что означает, что каждое вложение было удалено успешно. Значения некоторых атрибутов укорочены для удобства чтения.
  
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
    <m:DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
        <m:DeleteAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="uqE1AAA=" RootItemChangeKey="AAAXulck" />
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </m:DeleteAttachmentResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>См. также


- [Вложение и EWS в Exchange](attachments-and-ews-in-exchange.md)
    
- [Добавление вложений с помощью EWS в Exchange](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [Получение вложений с помощью EWS в Exchange](how-to-get-attachments-by-using-ews-in-exchange.md)
    

