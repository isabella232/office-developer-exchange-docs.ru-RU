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
# <a name="move-and-copy-email-messages-by-using-ews-in-exchange"></a><span data-ttu-id="3398f-103">Перемещение и копирование сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="3398f-103">Move and copy email messages by using EWS in Exchange</span></span>

<span data-ttu-id="3398f-104">Сведения о том, как перемещать и копировать сообщения электронной почты с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="3398f-104">Learn how to move and copy email messages by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="3398f-105">Для перемещения и копирования сообщений электронной почты в почтовый ящик можно использовать управляемый API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="3398f-105">You can use the EWS Managed API or EWS to move and copy email messages in a mailbox.</span></span>
  
<span data-ttu-id="3398f-106">**Таблица 1. Методы управляемого API EWS и операции EWS для перемещения и копирования сообщений электронной почты**</span><span class="sxs-lookup"><span data-stu-id="3398f-106">**Table 1. EWS Managed API methods and EWS operations for moving and copying email messages**</span></span>

|<span data-ttu-id="3398f-107">**Задача**</span><span class="sxs-lookup"><span data-stu-id="3398f-107">**Task**</span></span>|<span data-ttu-id="3398f-108">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="3398f-108">**EWS Managed API method**</span></span>|<span data-ttu-id="3398f-109">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="3398f-109">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3398f-110">Перемещение сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="3398f-110">Move an email message</span></span>  <br/> |[<span data-ttu-id="3398f-111">EmailMessage. Move</span><span class="sxs-lookup"><span data-stu-id="3398f-111">EmailMessage.Move</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="3398f-112">MoveItem</span><span class="sxs-lookup"><span data-stu-id="3398f-112">MoveItem</span></span>](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="3398f-113">Копирование сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="3398f-113">Copy an email message</span></span>  <br/> |[<span data-ttu-id="3398f-114">EmailMessage. Copy</span><span class="sxs-lookup"><span data-stu-id="3398f-114">EmailMessage.Copy</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="3398f-115">CopyItem</span><span class="sxs-lookup"><span data-stu-id="3398f-115">CopyItem</span></span>](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="3398f-116">Важно отметить, что при перемещении или копировании сообщения электронной почты в другую папку в новой папке создается новый элемент с уникальным ИДЕНТИФИКАТОРом элемента, а исходное сообщение удаляется.</span><span class="sxs-lookup"><span data-stu-id="3398f-116">It's important to note that when you move or copy an email message into a different folder, a new item is created in the new folder with a unique item ID, and the original message is deleted.</span></span> <span data-ttu-id="3398f-117">Если вы перемещаете или копируете сообщение электронной почты между двумя папками в одном почтовом ящике, в ответе возвращается новый элемент, который предоставляет доступ к новому ИДЕНТИФИКАТОРу элемента.</span><span class="sxs-lookup"><span data-stu-id="3398f-117">If you're moving or copying an email message between two folders in the same mailbox, the new item is returned in the response, which gives you access to the new item ID.</span></span> <span data-ttu-id="3398f-118">Однако если вы перемещаете или копируете сообщение электронной почты между двумя почтовыми ящиками, а также между почтовым ящиком и общедоступной папкой, новый элемент не возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="3398f-118">However, if you're moving or copying an email message between two mailboxes or between a mailbox and a public folder, the new item is not returned in the response.</span></span> <span data-ttu-id="3398f-119">Чтобы получить доступ к перемещенному сообщению в этом сценарии, используйте метод [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) управляемого API EWS или операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , [Создайте определение расширенного свойства](properties-and-extended-properties-in-ews-in-exchange.md) для свойства [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) или создайте и задайте пользовательское расширенное свойство, а затем выполните поиск настраиваемого расширенного свойства в новой папке.</span><span class="sxs-lookup"><span data-stu-id="3398f-119">To access the moved message in that scenario, use the EWS Managed API [FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method or EWS [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation, [create an extended property definition](properties-and-extended-properties-in-ews-in-exchange.md) for the [PidTagSearchKey](https://msdn.microsoft.com/library/cc839918.aspx) (0x300B0102) property, or create and set a custom extended property and then search for the custom extended property in the new folder.</span></span> 
  
<span data-ttu-id="3398f-120">Удаление сообщения электронной почты отличается от перемещения элемента в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="3398f-120">Deleting an email message is different than moving an item to the Deleted Items folder.</span></span> <span data-ttu-id="3398f-121">Если вы используете метод [Item. Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) управляемого API EWS или EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) , элемент, указанный в запросе, удаляется из исходной папки, а копия помещается в папку "Удаленные" с новым идентификатором элемента.</span><span class="sxs-lookup"><span data-stu-id="3398f-121">If you use the EWS Managed API [Item.Delete](https://msdn.microsoft.com/library/office/dd635072%28v=exchg.80%29.aspx) method or the EWS [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, the item specified in the request is removed from the original folder, and a copy is placed in the Deleted Items folder with a new item ID.</span></span> <span data-ttu-id="3398f-122">В отличие от того, что вы перемещаете или копируете какой-либо элемент, новый элемент не возвращается в методе **Delete** или ответе операции **DeleteItem** .</span><span class="sxs-lookup"><span data-stu-id="3398f-122">Unlike when you move or copy any item, the new item is not returned in the **Delete** method or the **DeleteItem** operation response.</span></span> <span data-ttu-id="3398f-123">Действия, выполняемые при [удалении электронной почты с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) или [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) , такие же, как и для удаления любого универсального элемента из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="3398f-123">The steps involved in [deleting an email by using the EWS Managed API](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) or [EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) are the same as those for deleting any generic item from the Exchange store.</span></span> 
  
## <a name="move-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="3398f-124">Перемещение сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3398f-124">Move an email message by using the EWS Managed API</span></span>
<span data-ttu-id="3398f-125"><a name="bk_moveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3398f-125"><a name="bk_moveewsma"> </a></span></span>

<span data-ttu-id="3398f-126">В приведенном ниже примере кода показано, как с помощью метода [EmailMessage. Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) переместить существующее сообщение электронной почты из одной папки в другую.</span><span class="sxs-lookup"><span data-stu-id="3398f-126">The following code example shows how to use the [EmailMessage.Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method to move an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="3398f-127">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а идентификатор **ItemId** — [идентификатором](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) сообщения электронной почты, которое необходимо переместить или скопировать.</span><span class="sxs-lookup"><span data-stu-id="3398f-127">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to move or copy.</span></span> 
  
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

## <a name="move-an-email-message-by-using-ews"></a><span data-ttu-id="3398f-128">Перемещение сообщения электронной почты с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="3398f-128">Move an email message by using EWS</span></span>
<span data-ttu-id="3398f-129"><a name="bk_moveews"> </a></span><span class="sxs-lookup"><span data-stu-id="3398f-129"><a name="bk_moveews"> </a></span></span>

<span data-ttu-id="3398f-130">В приведенном ниже примере кода показано, как с помощью операции [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) переместить сообщение электронной почты в папку нежелательной почты.</span><span class="sxs-lookup"><span data-stu-id="3398f-130">The following code example shows how to use the [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) operation to move an email message to the Junk Email folder.</span></span> 
  
<span data-ttu-id="3398f-131">Это также XML-запрос, который отправляется управляемым API EWS при вызове метода [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3398f-131">This is also the XML request that is sent by the EWS Managed API when calling the [Move](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.move%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="3398f-132">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="3398f-132">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="3398f-133">Сервер отвечает на запрос **MoveItem** с сообщением [мовеитемреспонсе](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение электронной почты было перемещено успешно.</span><span class="sxs-lookup"><span data-stu-id="3398f-133">The server responds to the **MoveItem** request with a [MoveItemResponse](https://msdn.microsoft.com/library/77be5104-1e09-4d50-abec-4fadb3a230e5%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was moved successfully.</span></span> <span data-ttu-id="3398f-134">Ответ также включает идентификатор **ItemId** для сообщения электронной почты в новой папке, который важен для хранения, так как идентификатор элемента ( **ItemId** ) отличается в новой папке.</span><span class="sxs-lookup"><span data-stu-id="3398f-134">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="copy-an-email-message-by-using-the-ews-managed-api"></a><span data-ttu-id="3398f-135">Копирование сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="3398f-135">Copy an email message by using the EWS Managed API</span></span>
<span data-ttu-id="3398f-136"><a name="bk_copyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="3398f-136"><a name="bk_copyewsma"> </a></span></span>

<span data-ttu-id="3398f-137">В приведенном ниже примере кода показано, как с помощью метода [EmailMessage. Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) скопировать существующее сообщение электронной почты из одной папки в другую.</span><span class="sxs-lookup"><span data-stu-id="3398f-137">The following code example shows how to use the [EmailMessage.Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method to copy an existing email message from one folder to another.</span></span> 
  
<span data-ttu-id="3398f-138">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , а идентификатор **ItemId** — [идентификатором](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) сообщения электронной почты, которое необходимо скопировать.</span><span class="sxs-lookup"><span data-stu-id="3398f-138">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, and that **ItemId** is the [Id](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) of the email message to copy.</span></span> <span data-ttu-id="3398f-139">Значения некоторых параметров были сокращены для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="3398f-139">The values of some parameters have been shortened for readability.</span></span> 
  
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

## <a name="copy-an-email-message-by-using-ews"></a><span data-ttu-id="3398f-140">Копирование электронного сообщения с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="3398f-140">Copy an email message by using EWS</span></span>
<span data-ttu-id="3398f-141"><a name="bk_copyews"> </a></span><span class="sxs-lookup"><span data-stu-id="3398f-141"><a name="bk_copyews"> </a></span></span>

<span data-ttu-id="3398f-142">В следующем примере кода показано, как с помощью операции [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) скопировать сообщение электронной почты в другую папку в том же почтовом ящике, отправив идентификатор [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) сообщения электронной почты для перемещения и указав папку назначения в элементе [тофолдерид](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3398f-142">The following code example shows how to use the [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) operation to copy an email message to different folder in the same mailbox by sending the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the email message to move, and specifying the destination folder in the [ToFolderId](https://msdn.microsoft.com/library/bd6a4265-ad40-43f6-bcc4-0bf5df4e984c%28Office.15%29.aspx) element.</span></span> 
  
<span data-ttu-id="3398f-143">Это также XML-запрос, который отправляется управляемым API EWS при вызове метода [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="3398f-143">This is also the XML request that is sent by the EWS Managed API when calling the [Copy](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.copy%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="3398f-144">Для удобства значения некоторых атрибутов и элементов были сокращены.</span><span class="sxs-lookup"><span data-stu-id="3398f-144">The values of some attributes and elements have been shortened for readability.</span></span> 
  
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

<span data-ttu-id="3398f-145">Сервер отвечает на запрос **CopyItem** с сообщением [копитемреспонсе](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) , которое содержит значение [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **, указывающее, что**сообщение электронной почты было успешно скопировано.</span><span class="sxs-lookup"><span data-stu-id="3398f-145">The server responds to the **CopyItem** request with a [CopyItemResponse](https://msdn.microsoft.com/library/ae402bc1-4589-45e0-a929-f368c916a7e4%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError**, which indicates that the email message was copied successfully.</span></span> <span data-ttu-id="3398f-146">Ответ также включает идентификатор **ItemId** для сообщения электронной почты в новой папке, который важен для хранения, так как идентификатор элемента ( **ItemId** ) отличается в новой папке.</span><span class="sxs-lookup"><span data-stu-id="3398f-146">The response also includes the **ItemId** for the email message in the new folder, which is important to store because the **ItemId** is different in the new folder.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3398f-147">См. также</span><span class="sxs-lookup"><span data-stu-id="3398f-147">See also</span></span>


- [<span data-ttu-id="3398f-148">Электронная почта и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="3398f-148">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
    
- [<span data-ttu-id="3398f-149">Отправка сообщений электронной почты с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="3398f-149">Send email messages by using EWS in Exchange</span></span>](how-to-send-email-messages-by-using-ews-in-exchange.md)
    

