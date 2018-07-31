---
title: Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4771668f-5623-4397-a5c0-b75a7ba01698
description: Узнайте, как перемещение и копирование сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 44d5834176b55ad041befbad2230b8b507a12ecc
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353471"
---
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="448de-103">Перемещение и копирование сообщений электронной почты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="448de-104">Узнайте, как перемещение и копирование сообщений электронной почты с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="448de-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="448de-105">Можно использовать управляемый API EWS или веб-служб Exchange для перемещения и копирования сообщений в почтовый ящик электронной почты.</span><span class="sxs-lookup"><span data-stu-id="448de-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="448de-106">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange на перемещение и копирование сообщений электронной почты**</span><span class="sxs-lookup"><span data-stu-id="448de-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="448de-107">**Задача**</span><span class="sxs-lookup"><span data-stu-id="448de-107">**Task**</span></span>|<span data-ttu-id="448de-108">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="448de-108">**EWS Managed API method**</span></span>|<span data-ttu-id="448de-109">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="448de-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="448de-110">Перемещение сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="448de-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="448de-111">EmailMessage.Move</span><span class="sxs-lookup"><span data-stu-id="448de-111">EmailMessage.Move</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="448de-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="448de-112">MoveItem</span></span>](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="448de-113">Скопируйте сообщение электронной почты</span><span class="sxs-lookup"><span data-stu-id="448de-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="448de-114">EmailMessage.Copy</span><span class="sxs-lookup"><span data-stu-id="448de-114">EmailMessage.Copy</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="448de-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="448de-115">CopyItem</span></span>](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="448de-116">Важно отметить, что после перемещения или копирования сообщения электронной почты в другую папку, в новую папку с Идентификатором уникального элемента создается новый элемент и исходное сообщение удаляется.</span><span class="sxs-lookup"><span data-stu-id="448de-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="448de-117">Если в случае перемещения или копирования сообщения электронной почты между двумя папок в тот же почтовый ящик, новый элемент, возвращается в ответ, который предоставляет доступ к новый идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="448de-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="448de-118">Тем не менее если в случае перемещения или копирования сообщения электронной почты между двумя почтовых ящиков или почтового ящика и общей папки, новый элемент не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="448de-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="448de-119">Для доступа к перемещенной сообщения в этом сценарии, используйте метод управляемый API EWS [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или операции EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [Создание определения расширенных свойств](properties-and-extended-properties-in-ews-in-exchange.md) для свойства [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102), или создать и параметры настраиваемые расширенные свойства и выполните поиск дополнительное пользовательское свойство в новую папку.</span><span class="sxs-lookup"><span data-stu-id="448de-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](http://msdn.microsoft.com/en-us/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="448de-120">Удаление сообщения электронной почты, отличается от Перемещение элемента в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="448de-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="448de-121">При использовании метода управляемый API EWS [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) или операции EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) элемента, указанного в запросе удаляется из исходной папки, а копия помещается в папку «Удаленные» с новый идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="448de-121">If you use the EWS Managed API [Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="448de-122">В отличие от при переместить или скопировать любой элемент новый элемент не возвращается в метод **Delete** или ответа **DeleteItem** операции.</span><span class="sxs-lookup"><span data-stu-id="448de-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="448de-123">Шаги при [удалении сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) или [веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) такие же, как для удаления любого универсального элемента из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="448de-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="448de-124">Перемещение сообщения электронной почты с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="448de-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="448de-125"></span></span>

<span data-ttu-id="448de-126">В следующем примере кода показано, как использовать метод [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) для перемещения существующего сообщения электронной почты из одной папки в другую.</span><span class="sxs-lookup"><span data-stu-id="448de-126">The following code example shows how to use the [EmailMessage.Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="448de-127">В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и этот **идентификатор элемента** — это [идентификатор](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) для сообщения электронной почты для перемещения или копирования.</span><span class="sxs-lookup"><span data-stu-id="448de-127">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
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

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="448de-128">Перемещение сообщения электронной почты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-128">Move an email message by using EWS</span></span>
<span data-ttu-id="448de-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="448de-129"></span></span>

<span data-ttu-id="448de-130">В следующем примере кода показано, как использовать операцию [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) для перемещения сообщения электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="448de-130">The following code example shows how to use the [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="448de-131">Это также запроса XML, отправляемого управляемый API EWS при вызове метода [перемещения](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="448de-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="448de-132">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="448de-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="448de-133">Сервер отвечает на запрос **MoveItem** [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно перемещен.</span><span class="sxs-lookup"><span data-stu-id="448de-133">The server responds to the **MoveItem** request with a [MoveItemResponse](http://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="448de-134">Ответ также включает **ItemId** для сообщения электронной почты в новых папка, в которой необходимо хранить из-за **ItemId** в новую папку.</span><span class="sxs-lookup"><span data-stu-id="448de-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="448de-135">Скопируйте сообщение электронной почты с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="448de-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="448de-136"></span></span>

<span data-ttu-id="448de-137">В следующем примере кода показано, как использовать метод [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) , чтобы скопировать существующее сообщение электронной почты из одной папки.</span><span class="sxs-lookup"><span data-stu-id="448de-137">The following code example shows how to use the [EmailMessage.Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="448de-138">В этом примере предполагается, что **службы** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , и этот **идентификатор элемента** — это [идентификатор](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) для сообщения электронной почты для копирования.</span><span class="sxs-lookup"><span data-stu-id="448de-138">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="448de-139">Значения некоторых параметров URL-были сокращены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="448de-139">The values of some parameters have been shortened for readability.</span></span> 
  
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

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="448de-140">Скопируйте сообщение электронной почты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="448de-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="448de-141"></span></span>

<span data-ttu-id="448de-142">В следующем примере кода показано, как использовать операцию [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) для копирования сообщения электронной почты в другую папку в тот же почтовый ящик, отправив [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) сообщения электронной почты для перемещения и указания папки назначения в [ToFolderId ](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx)элемент.</span><span class="sxs-lookup"><span data-stu-id="448de-142">The following code example shows how to use the [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](http://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="448de-143">Это также запроса XML, отправляемого управляемый API EWS при вызове метода [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="448de-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="448de-144">Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.</span><span class="sxs-lookup"><span data-stu-id="448de-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="448de-145">Сервер отвечает на запрос **CopyItem** [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты копирование было выполнено успешно.</span><span class="sxs-lookup"><span data-stu-id="448de-145">The server responds to the **CopyItem** request with a [CopyItemResponse](http://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="448de-146">Ответ также включает **ItemId** для сообщения электронной почты в новых папка, в которой необходимо хранить из-за **ItemId** в новую папку.</span><span class="sxs-lookup"><span data-stu-id="448de-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="448de-147">См. также</span><span class="sxs-lookup"><span data-stu-id="448de-147">See also</span></span>


- [<span data-ttu-id="448de-148">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="448de-149">Отправлять сообщения электронной почты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="448de-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

