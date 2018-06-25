---
title: Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Узнайте, как перемещение и копирование сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 16f0604a16785c34dd04bdabedeedd331668a479
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761082"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange

Узнайте, как перемещение и копирование сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно использовать управляемый API EWS или веб-служб Exchange для перемещения и копирования сообщений в почтовый ящик электронной почты.
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange на перемещение и копирование сообщений электронной почты**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Перемещение сообщения электронной почты  <br/> |[EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Скопируйте сообщение электронной почты  <br/> |[EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
Важно отметить, что после перемещения или копирования сообщения электронной почты в другую папку, в новую папку с Идентификатором уникального элемента создается новый элемент и исходное сообщение удаляется. Если в случае перемещения или копирования сообщения электронной почты между двумя папок в тот же почтовый ящик, новый элемент, возвращается в ответ, который предоставляет доступ к новый идентификатор элемента. Тем не менее если в случае перемещения или копирования сообщения электронной почты между двумя почтовых ящиков или почтового ящика и общей папки, новый элемент не возвращается в ответе. Для доступа к перемещенной сообщения в этом сценарии, используйте метод управляемый API EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или операции EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [Создание определения расширенных свойств](properties-and-extended-properties-in-ews-in-exchange.md) для свойства [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102), или создать и параметры настраиваемые расширенные свойства и выполните поиск дополнительное пользовательское свойство в новую папку. 
  
Удаление сообщения электронной почты, отличается от Перемещение элемента в папку «Удаленные». При использовании метода управляемый API EWS [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) или операции EWS [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) элемента, указанного в запросе удаляется из исходной папки, а копия помещается в папку «Удаленные» с новый идентификатор элемента. В отличие от при переместить или скопировать любой элемент новый элемент не возвращается в метод **Delete** или ответа **DeleteItem** операции. Шаги при [удалении сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) или [веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) такие же, как для удаления любого универсального элемента из хранилища Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Перемещение сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_moveewsma"> </a>

В следующем примере кода показано, как использовать метод [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) для перемещения существующего сообщения электронной почты из одной папки в другую. 
  
В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и этот **идентификатор элемента** — это [идентификатор](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) для сообщения электронной почты для перемещения или копирования. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage beforeMessage = EmailMessage.Bind(service, ItemId, propSet);
// Move the specified mail to the JunkEmail folder and store the returned item.
Item item = beforeMessage.Move(WellKnownFolderName.JunkEmail);
// Check that the item was moved by binding to the moved email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage movedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + beforeMessage.Subject + "' has been moved from the '" + beforeMessage.ParentFolderId + "' folder to the '" + movedMessage.ParentFolderId + "' folder.");
```

## <a name="move-an-email-message-by-using-ews"></a>Перемещение сообщения электронной почты с помощью веб-служб Exchange
<a name="bk_moveews"> </a>

В следующем примере кода показано, как использовать операцию [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) для перемещения сообщения электронной почты в папку нежелательной почты. 
  
Это также запроса XML, отправляемого управляемый API EWS при вызове метода [перемещения](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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
    <m:MoveItem>
      <m:ToFolderId>
        <t:DistinguishedFolderId Id="junkemail" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="AfwDoAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF25sM1" />
      </m:ItemIds>
    </m:MoveItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **MoveItem** [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно перемещен. Ответ также включает **ItemId** для сообщения электронной почты в новых папка, в которой необходимо хранить из-за **ItemId** в новую папку. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Скопируйте сообщение электронной почты с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_copyewsma"> </a>

В следующем примере кода показано, как использовать метод [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) , чтобы скопировать существующее сообщение электронной почты из одной папки. 
  
В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и этот **идентификатор элемента** — это [идентификатор](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) для сообщения электронной почты для копирования. Значения некоторых параметров URL-были сокращены для удобства чтения. 
  
```cs
// As a best practice, limit the properties returned by the Bind method to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, EmailMessageSchema.Subject, EmailMessageSchema.ParentFolderId);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
EmailMessage originalMessage = EmailMessage.Bind(service, ItemId, propSet);
// Copy the orignal message into another folder in the mailbox and store the returned item.
Item item = originalMessage.Copy("epQ/3AAA=");
// Check that the item was copied by binding to the copied email message 
// and retrieving the new ParentFolderId.
// This method call results in a GetItem call to EWS.
EmailMessage copiedMessage = EmailMessage.Bind(service, item.Id, propSet);
Console.WriteLine("An email message with the subject '" + originalMessage.Subject + "' has been copied from the '" + originalMessage.ParentFolderId + "' folder to the '" + copiedMessage.ParentFolderId + "' folder.");
```

## <a name="copy-an-email-message-by-using-ews"></a>Скопируйте сообщение электронной почты с помощью веб-служб Exchange
<a name="bk_copyews"> </a>

В следующем примере кода показано, как использовать операцию [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) для копирования сообщения электронной почты в другую папку в тот же почтовый ящик, отправив [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) сообщения электронной почты для перемещения и указания папки назначения в [ToFolderId ](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)элемент. 
  
Это также запроса XML, отправляемого управляемый API EWS при вызове метода [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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
    <m:CopyItem>
      <m:ToFolderId>
        <t:FolderId Id="pQ/3AAA=" />
      </m:ToFolderId>
      <m:ItemIds>
        <t:ItemId Id="2TSeSAAA="
                  ChangeKey="CQAAABYAAAApjGm7TnMWQ5TzjbhziLL0AAF2d+3+" />
      </m:ItemIds>
    </m:CopyItem>
  </soap:Body>
</soap:Envelope>
```

Сервер отвечает на запрос **CopyItem** [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты копирование было выполнено успешно. Ответ также включает **ItemId** для сообщения электронной почты в новых папка, в которой необходимо хранить из-за **ItemId** в новую папку. 
  
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

