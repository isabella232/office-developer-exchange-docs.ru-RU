---
title: Удаление вложений с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 71871ac7-ee1a-4f93-9e81-77f312d432f4
description: Узнайте, как удалять вложения из элементов с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 458331f81493283efc20d24c7e2bebe0e74bbdbd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761004"
---
# <a name="delete-attachments-by-using-ews-in-exchange"></a><span data-ttu-id="550e1-103">Удаление вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="550e1-103">Delete attachments by using EWS in Exchange</span></span>

<span data-ttu-id="550e1-104">Узнайте, как удалять вложения из элементов с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="550e1-104">Learn how to delete attachments from items by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="550e1-105">Существует несколько вариантов удаления вложенных файлов и элементов из элементов с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="550e1-105">You have a number of options when it comes to deleting file and item attachments from items by using the EWS Managed API.</span></span> <span data-ttu-id="550e1-106">Вы можете удалить все вложения из сообщения, удалить его по имени или удалить по позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="550e1-106">You can delete all the attachments from the message, delete by a file name, or delete by position in the collection.</span></span> <span data-ttu-id="550e1-107">Для каждого из этих параметров существует метод [аттачментколлектион](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="550e1-107">For each of these options, there is an [AttachmentCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="550e1-108">С другой стороны, у вас независимо от того, вы удаляете все вложения из элемента или только из одной, последовательность операций одинакова.</span><span class="sxs-lookup"><span data-stu-id="550e1-108">Conversely, with EWS, no matter whether you're deleting all attachments from an item or just one, the sequence of operations is same.</span></span> <span data-ttu-id="550e1-109">В отличие от управляемого API EWS, EWS не включает отдельные операции для удаления в зависимости от имени или положения в массиве вложений.</span><span class="sxs-lookup"><span data-stu-id="550e1-109">Unlike the EWS Managed API, EWS does not include separate operations to delete based on name or position in the attachments array.</span></span>
  
<span data-ttu-id="550e1-110">**Таблица 1. Методы управляемого API EWS и операции EWS для удаления вложений**</span><span class="sxs-lookup"><span data-stu-id="550e1-110">**Table 1. EWS Managed API methods and EWS operations for deleting attachments**</span></span>

|<span data-ttu-id="550e1-111">**Задача**</span><span class="sxs-lookup"><span data-stu-id="550e1-111">**Task**</span></span>|<span data-ttu-id="550e1-112">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="550e1-112">**EWS Managed API method**</span></span>|<span data-ttu-id="550e1-113">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="550e1-113">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="550e1-114">Удаление всех вложений из элемента.</span><span class="sxs-lookup"><span data-stu-id="550e1-114">Delete all attachments from an item.</span></span>  <br/> |<span data-ttu-id="550e1-115">[Item. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [аттачментколлектион. Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-115">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="550e1-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-116">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="550e1-117">Удаление вложения из элемента по имени.</span><span class="sxs-lookup"><span data-stu-id="550e1-117">Delete an attachment from an item by name.</span></span>  <br/> |<span data-ttu-id="550e1-118">[Item. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [Аттачментколлектион. Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-118">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="550e1-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-119">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="550e1-120">Удаление вложения из элемента по позиции в коллекции.</span><span class="sxs-lookup"><span data-stu-id="550e1-120">Delete an attachment from an item by position in the collection.</span></span>  <br/> |<span data-ttu-id="550e1-121">[Item. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), за которым следует [аттачментколлектион. RemoveAt](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), за которым следует [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-121">[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx), followed by [AttachmentCollection.RemoveAt](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.removeat%28v=exchg.80%29.aspx), followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="550e1-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) , за которым следует [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="550e1-122">[GetItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) followed by [DeleteAttachment](http://msdn.microsoft.com/library/43d0c1cb-92ca-4399-9b3a-acb2b5c22624%28Office.15%29.aspx)</span></span> <br/> |
   
## <a name="delete-all-attachments-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="550e1-123">Удаление всех вложений из электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="550e1-123">Delete all attachments from an email by using the EWS Managed API</span></span>
<span data-ttu-id="550e1-124"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="550e1-124"><a name="bk_deleteattachewsma"> </a></span></span>

<span data-ttu-id="550e1-125">В приведенном ниже примере кода показано, как удалить все вложения из сообщения электронной почты, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="550e1-125">The following code example shows how to delete all attachments from an email by:</span></span>
  
1. <span data-ttu-id="550e1-126">С помощью метода [EmailMessage. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="550e1-126">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="550e1-127">Использование метода [аттачментколлектион. Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) для удаления всех вложений из электронной почты.</span><span class="sxs-lookup"><span data-stu-id="550e1-127">Using the [AttachmentCollection.Clear](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.clear%28v=exchg.80%29.aspx) method to delete all the attachments from the email.</span></span> 
    
3. <span data-ttu-id="550e1-128">Использование метода [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="550e1-128">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="550e1-129">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , идентификатором **ItemId** является идентификатором [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляются вложения, и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="550e1-129">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which attachments will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-an-attachment-by-name-from-an-email-by-using-the-ews-managed-api"></a><span data-ttu-id="550e1-130">Удаление вложения по имени из сообщения электронной почты с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="550e1-130">Delete an attachment by name from an email by using the EWS Managed API</span></span>
<span data-ttu-id="550e1-131"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="550e1-131"><a name="bk_deleteattachewsma"> </a></span></span>

<span data-ttu-id="550e1-132">В приведенном ниже примере кода показано, как удалить вложение по имени, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="550e1-132">The following code example shows how delete an attachment by name by:</span></span>
  
1. <span data-ttu-id="550e1-133">С помощью метода [EmailMessage. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="550e1-133">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx).</span></span>
    
2. <span data-ttu-id="550e1-134">Использование метода [аттачментколлектион. Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) для удаления вложения с именем FileAttachment. txt.</span><span class="sxs-lookup"><span data-stu-id="550e1-134">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete an attachment named FileAttachment.txt.</span></span> 
    
3. <span data-ttu-id="550e1-135">Использование метода [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="550e1-135">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="550e1-136">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **ItemId** — [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляется вложение, и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="550e1-136">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-attachments-by-position-by-using-the-ews-managed-api"></a><span data-ttu-id="550e1-137">Удаление вложений по положению с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="550e1-137">Delete attachments by position by using the EWS Managed API</span></span>
<span data-ttu-id="550e1-138"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="550e1-138"><a name="bk_deleteattachewsma"> </a></span></span>

<span data-ttu-id="550e1-139">В приведенном ниже примере кода показано, как удалить вложение по позиции, выполнив следующие действия:</span><span class="sxs-lookup"><span data-stu-id="550e1-139">The following code example shows how to delete an attachment by position by:</span></span>
  
1. <span data-ttu-id="550e1-140">С помощью метода [EmailMessage. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) можно выполнить присоединение к существующему сообщению электронной почты и получить коллекцию [вложений](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) и свойство [EmailMessage. HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="550e1-140">Using the [EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) method to bind to an existing email message and retrieve the collection of [Attachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.attachments%28v=exchg.80%29.aspx) and the [EmailMessage.HasAttachments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.hasattachments%28v=exchg.80%29.aspx) property.</span></span> 
    
2. <span data-ttu-id="550e1-141">Использование метода [аттачментколлектион. Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) для удаления первого вложения в коллекции.</span><span class="sxs-lookup"><span data-stu-id="550e1-141">Using the [AttachmentCollection.Remove](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.attachmentcollection.remove%28v=exchg.80%29.aspx) method to delete the first attachment in the collection.</span></span> 
    
3. <span data-ttu-id="550e1-142">Использование метода [EmailMessage. Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) для сохранения изменений.</span><span class="sxs-lookup"><span data-stu-id="550e1-142">Using the [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx) method to save the changes.</span></span> 
    
<span data-ttu-id="550e1-143">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) , **ItemId** — [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) сообщения, из которого удаляется вложение, и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="550e1-143">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object, **itemId** is the [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) of the message from which the attachment will be deleted, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

## <a name="delete-attachments-from-an-item-by-using-ews"></a><span data-ttu-id="550e1-144">Удаление вложений из элемента с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="550e1-144">Delete attachments from an item by using EWS</span></span>
<span data-ttu-id="550e1-145"><a name="bk_deleteattachewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="550e1-145"><a name="bk_deleteattachewsma"> </a></span></span>

<span data-ttu-id="550e1-146">Чтобы удалить вложения с помощью EWS, сначала необходимо получить сообщение и коллекцию вложений, чтобы определить [AttachmentId (GetAttachment и DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) вложения, которое требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="550e1-146">To delete attachments by using EWS, you first need to retrieve the message and the attachment collection to determine the [AttachmentId (GetAttachment and DeleteAttachment)](http://msdn.microsoft.com/library/4bea1cb5-0a0f-4e14-9b09-f91af8cf9899%28Office.15%29.aspx) of the attachment to delete.</span></span> <span data-ttu-id="550e1-147">После удаления одного или нескольких значений **AttachmentId** вызовите операцию [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) , чтобы удалить указанные вложения из сообщения.</span><span class="sxs-lookup"><span data-stu-id="550e1-147">After you have one or more **AttachmentId** values to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation to remove the specified attachments from the message.</span></span> 
  
<span data-ttu-id="550e1-148">В следующем примере кода показано, как использовать операцию [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) для получения сообщения электронной почты и коллекции вложений сообщения.</span><span class="sxs-lookup"><span data-stu-id="550e1-148">The following code example shows how to use the [GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) operation to get an email message and the collection of attachments on the message.</span></span> <span data-ttu-id="550e1-149">Кроме того, это первый XML-запрос, который отправляет управляемый API EWS при использовании управляемого API EWS для [удаления всех вложений из электронной почты](#bk_deleteattachewsma).</span><span class="sxs-lookup"><span data-stu-id="550e1-149">This is also the first XML request that the EWS Managed API sends when you use the EWS Managed API to [delete all attachments from an email](#bk_deleteattachewsma).</span></span> <span data-ttu-id="550e1-150">Значения некоторых атрибутов укорочены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="550e1-150">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="550e1-151">В ответ на запрос **GetItem** сервер отправляет сообщение [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx), содержащее элемент [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError** (что говорит об успешном извлечении письма) и значения [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) существующих вложений.</span><span class="sxs-lookup"><span data-stu-id="550e1-151">The server responds to the **GetItem** request with a [GetItemResponse](http://msdn.microsoft.com/library/8b66de1b-26a6-476c-9585-a96059125716%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) value of **NoError**, which indicates that the email was retrieved successfully, and the [AttachmentId](http://msdn.microsoft.com/library/55a5fd77-60d1-40fa-8144-770600cedc6a%28Office.15%29.aspx) values of the existing attachments.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
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

<span data-ttu-id="550e1-152">Определив вложение, которое необходимо удалить, вызовите операцию [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) и добавьте значения **AttachmentId** для удаляемых вложений.</span><span class="sxs-lookup"><span data-stu-id="550e1-152">After you determine which attachment to delete, call the [DeleteAttachment](http://msdn.microsoft.com/library/4d48e595-b98c-48e7-bbeb-cacf91d12a78%28Office.15%29.aspx) operation and include the **AttachmentId** values of the attachments to delete.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос DeleteAttachment с сообщением [делетеаттачментреспонсе](http://msdn.microsoft.com/library/24099a88-4ab6-4bf3-8ed5-efec8e07b9b9%28Office.15%29.aspx) , которое включает в [себя значение](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **DeleteAttachment** **для каждого** [делетеаттачментреспонсемессаже](http://msdn.microsoft.com/library/1edb085f-1674-48e5-8ec3-42351adeac7d%28Office.15%29.aspx), что означает, что каждое вложение было удалено успешно. <span data-ttu-id="550e1-154">Значения некоторых атрибутов укорочены для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="550e1-154">The values of some attributes are shortened for readability.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="939"
                         MinorBuildNumber="12"
                         Version="V2_11"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="550e1-155">См. также</span><span class="sxs-lookup"><span data-stu-id="550e1-155">See also</span></span>


- [<span data-ttu-id="550e1-156">Вложение и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="550e1-156">Attachments and EWS in Exchange</span></span>](attachments-and-ews-in-exchange.md)
    
- [<span data-ttu-id="550e1-157">Добавление вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="550e1-157">Add attachments by using EWS in Exchange</span></span>](how-to-add-attachments-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="550e1-158">Получение вложений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="550e1-158">Get attachments by using EWS in Exchange</span></span>](how-to-get-attachments-by-using-ews-in-exchange.md)
    

