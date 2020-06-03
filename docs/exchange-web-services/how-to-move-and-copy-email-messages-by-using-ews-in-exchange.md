---
title: Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Сведения о том, как перемещать и копировать сообщения электронной почты с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: d13e84648f194dd4f431cf128396daf016addb22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527938"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a>Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange

Сведения о том, как перемещать и копировать сообщения электронной почты с помощью управляемого API EWS или EWS в Exchange.
  
Для перемещения и копирования сообщений электронной почты в почтовый ящик можно использовать управляемый API EWS или EWS.
  
**Таблица 1. Методы управляемого API EWS и операции EWS для перемещения и копирования сообщений электронной почты**

|**Задача**|**Метод управляемого API EWS**|**Операция EWS**|
|:-----|:-----|:-----|
|Перемещение сообщения электронной почты  <br/> |[EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|Копирование сообщения электронной почты  <br/> |[EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
Важно отметить, что при перемещении или копировании сообщения электронной почты в другую папку в новой папке создается новый элемент с уникальным ИДЕНТИФИКАТОРом элемента, а исходное сообщение удаляется. Если вы перемещаете или копируете сообщение электронной почты между двумя папками в одном почтовом ящике, в ответе возвращается новый элемент, который предоставляет доступ к новому ИДЕНТИФИКАТОРу элемента. Однако если вы перемещаете или копируете сообщение электронной почты между двумя почтовыми ящиками, а также между почтовым ящиком и общедоступной папкой, новый элемент не возвращается в ответе. Чтобы получить доступ к перемещенному сообщению в этом сценарии, используйте метод [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) управляемого API EWS или операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [Создайте определение расширенного свойства](properties-and-extended-properties-in-ews-in-exchange.md) для свойства [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) или создайте и задайте пользовательское расширенное свойство, а затем выполните поиск настраиваемого расширенного свойства в новой папке. 
  
Удаление сообщения электронной почты отличается от перемещения элемента в папку "Удаленные". Если вы используете метод [Item. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) управляемого API EWS или EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) , элемент, указанный в запросе, удаляется из исходной папки, а копия помещается в папку "Удаленные" с новым идентификатором элемента. В отличие от того, что вы перемещаете или копируете какой-либо элемент, новый элемент не возвращается в методе **Delete** или ответе операции **DeleteItem** . Действия, выполняемые при [удалении электронной почты с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) или [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) , такие же, как и для удаления любого универсального элемента из хранилища Exchange. 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a>Перемещение сообщения электронной почты с помощью управляемого API EWS
<a name="bk_moveewsma"> </a>

В приведенном ниже примере кода показано, как с помощью метода [EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) переместить существующее сообщение электронной почты из одной папки в другую. 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а идентификатор **ItemId** — [идентификатором](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) сообщения электронной почты, которое необходимо переместить или скопировать. 
  
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

## <a name="move-an-email-message-by-using-ews"></a>Перемещение сообщения электронной почты с помощью EWS
<a name="bk_moveews"> </a>

В приведенном ниже примере кода показано, как с помощью операции [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) переместить сообщение электронной почты в папку нежелательной почты. 
  
Это также XML-запрос, который отправляется управляемым API EWS при вызове метода [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) . Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **MoveItem** с сообщением [мовеитемреспонсе](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение электронной почты было перемещено успешно. Ответ также включает идентификатор **ItemId** для сообщения электронной почты в новой папке, который важен для хранения, так как идентификатор элемента ( **ItemId** ) отличается в новой папке. 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a>Копирование сообщения электронной почты с помощью управляемого API EWS
<a name="bk_copyewsma"> </a>

В приведенном ниже примере кода показано, как с помощью метода [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) скопировать существующее сообщение электронной почты из одной папки в другую. 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а идентификатор **ItemId** — [идентификатором](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) сообщения электронной почты, которое необходимо скопировать. Значения некоторых параметров были сокращены для удобочитаемости. 
  
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

## <a name="copy-an-email-message-by-using-ews"></a>Копирование электронного сообщения с помощью EWS
<a name="bk_copyews"> </a>

В следующем примере кода показано, как с помощью операции [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) скопировать сообщение электронной почты в другую папку в том же почтовом ящике, отправив идентификатор [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) сообщения электронной почты для перемещения и указав папку назначения в элементе [тофолдерид](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) . 
  
Это также XML-запрос, который отправляется управляемым API EWS при вызове метода [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) . Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **CopyItem** с сообщением [копитемреспонсе](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение электронной почты было успешно скопировано. Ответ также включает идентификатор **ItemId** для сообщения электронной почты в новой папке, который важен для хранения, так как идентификатор элемента ( **ItemId** ) отличается в новой папке. 
  
## <a name="see-also"></a>См. также


- [Электронная почта и веб-службах Exchange](email-and-ews-in-exchange.md)
    
- [Отправка сообщений электронной почты с помощью EWS в Exchange](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

