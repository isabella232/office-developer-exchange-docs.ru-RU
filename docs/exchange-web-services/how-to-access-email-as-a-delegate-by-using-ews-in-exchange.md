---
title: Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Узнайте, как получить доступ к электронной почте роли представителя с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 8331f337136426913347cf6941d64b4611922d74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760972"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="1ce6f-103">Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-103">Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="1ce6f-104">Узнайте, как получить доступ к электронной почте роли представителя с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="1ce6f-105">Можно использовать управляемый API EWS или делегирование EWS, чтобы предоставить пользователю доступ к папке "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder.</span></span> <span data-ttu-id="1ce6f-106">Делегат можно затем Создание приглашений на собрания от имени владельца почтового ящика, поиск электронной почты и извлечь, обновление и удаление электронной почты из папки "Входящие" владельца почтового ящика, в зависимости от их разрешения.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-106">The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="1ce6f-107">Роли представителя используйте ту же методов и операций на доступ к папке "Входящие" владельца почтового ящика, которая используется для доступа к папке "Входящие" без делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-107">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access.</span></span> <span data-ttu-id="1ce6f-108">Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создать элемент электронной почты, и затем после определения идентификатора элемента, можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="1ce6f-109">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к электронной почте в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-109">**Table 1. EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="1ce6f-110">**Если вы хотите...**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-110">**If you want to…**</span></span>|<span data-ttu-id="1ce6f-111">**Используйте этот метод управляемый API EWS...**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="1ce6f-112">**Используйте эту операцию EWS...**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ce6f-113">Создание и отправка сообщения электронной почты как делегат</span><span class="sxs-lookup"><span data-stu-id="1ce6f-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="1ce6f-114">[EmailMessage.Save](http://msdn.microsoft.com/ru-ru/library/dd635209%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке «Черновики» владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-114">[EmailMessage.Save](http://msdn.microsoft.com/ru-ru/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="1ce6f-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ru-ru/library/dd634248%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Отправленные" владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ru-ru/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="1ce6f-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="1ce6f-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="1ce6f-118">Создание нескольких сообщений электронной почты в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="1ce6f-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="1ce6f-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Входящие" владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="1ce6f-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="1ce6f-121">Поиск и искать сообщения электронной почты в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="1ce6f-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="1ce6f-122">[ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке "Входящие" владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-122">[ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="1ce6f-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ce6f-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="1ce6f-124">Получите сообщение электронной почты как делегат</span><span class="sxs-lookup"><span data-stu-id="1ce6f-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="1ce6f-125">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="1ce6f-125">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1ce6f-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="1ce6f-126">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="1ce6f-127">Обновление сообщения электронной почты в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="1ce6f-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="1ce6f-128">[EmailMessage.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [EmailMessage.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-128">[EmailMessage.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="1ce6f-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="1ce6f-130">Удаление сообщения электронной почты как делегат</span><span class="sxs-lookup"><span data-stu-id="1ce6f-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="1ce6f-131">[EmailMessage.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [EmailMessage.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-131">[EmailMessage.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="1ce6f-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
<span data-ttu-id="1ce6f-133">При работе с по электронной почте в качестве делегата, следует в виду следующее.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="1ce6f-134">Если делегат должен работать с приглашений на собрания и ответы, делегат необходим доступ к папке "Входящие".</span><span class="sxs-lookup"><span data-stu-id="1ce6f-134">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder.</span></span> <span data-ttu-id="1ce6f-135">Для получения дополнительных сведений см [обязательные задачи для доступа к календарям в качестве делегата](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span><span class="sxs-lookup"><span data-stu-id="1ce6f-135">For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="1ce6f-136">Когда получатель получает сообщение, которое было отправлено от имени владельца почтового ящика, отправителя отображается как « *делегат* от имени *владельца почтового ящика* ».</span><span class="sxs-lookup"><span data-stu-id="1ce6f-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as " *Delegate*  on behalf of  *mailbox owner*  ."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="1ce6f-137">В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="1ce6f-138">Обязательные задачи</span><span class="sxs-lookup"><span data-stu-id="1ce6f-138">Prerequisite tasks</span></span>
<span data-ttu-id="1ce6f-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-139"></span></span>

<span data-ttu-id="1ce6f-140">Пользователь может получить доступ к папки "Входящие" владельца почтового ящика роли представителя, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="1ce6f-141">Создание и отправка сообщения электронной почты как делегат с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="1ce6f-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-142"></span></span>

<span data-ttu-id="1ce6f-143">Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания и отправки электронной почты от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="1ce6f-144">В этом примере показано, как использовать метод [Save](http://msdn.microsoft.com/ru-ru/library/dd635209%28v=exchg.80%29.aspx) , чтобы сохранить сообщение в папке «Черновики» владельца почтового ящика, а затем метод [SendAndSaveCopy](http://msdn.microsoft.com/ru-ru/library/dd634248%28v=exchg.80%29.aspx) для отправки почты и сохранить сообщение в папке "Отправленные" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-144">This example shows how to use the [Save](http://msdn.microsoft.com/ru-ru/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopy](http://msdn.microsoft.com/ru-ru/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="1ce6f-145">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата имеет [соответствующие разрешения для папки «Входящие», «Черновики» и отправленные владельца почтового ящика](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="1ce6f-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="1ce6f-146">Создание и отправка сообщения электронной почты как делегат с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="1ce6f-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-147"></span></span>

<span data-ttu-id="1ce6f-148">Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания и отправки электронной почты от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-148">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="1ce6f-149">В этом примере показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания сообщения электронной почты и операции [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) отправлять время и сохраните его в папке "Отправленные" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-149">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="1ce6f-150">Это первый запрос XML, который отправляет управляемый API EWS при использовании метода **Save** для [создания и отправки сообщения электронной почты](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="1ce6f-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
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
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
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

<span data-ttu-id="1ce6f-151">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что сообщение электронной почты был создан и успешно сохранен.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully.</span></span> <span data-ttu-id="1ce6f-152">Ответ также содержит идентификатор только что созданный сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-152">The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="1ce6f-153">Значение **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-153">The **ItemId** value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1ce6f-154">Затем используйте операции **SendItem** отправлять сообщения от имени владельца почтового ящика и сохраните его в папке "Отправленные" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="1ce6f-155">Значение **ItemId** был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-155">The **ItemId** value has been shortened for readability.</span></span> 
  
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
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1ce6f-156">Сервер отвечает на запрос **SendItem** [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что сообщение электронной почты было отправлено и сохраняются в папке "Отправленные" владельца почтового ящика успешно.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-156">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="1ce6f-157">Поиск сообщения электронной почты в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="1ce6f-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-158"></span></span>

<span data-ttu-id="1ce6f-159">Для поиска сообщения электронной почты, необходимо использовать один из методов [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-159">To search for an email, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="1ce6f-160">После вызова **FindItems** возвращает ответ с Идентификатором, можно получить, update или delete, электронной почты с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) - вам не нужно указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="1ce6f-161">Поиск сообщения электронной почты в качестве делегата с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="1ce6f-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-162"></span></span>

<span data-ttu-id="1ce6f-163">Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для поиска по электронной почте, которые соответствуют набору условий поиска.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-163">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria.</span></span> <span data-ttu-id="1ce6f-164">В этом примере показано, как использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для поиска сообщений в папке "Входящие" владельца почтового, содержащие слово «футбольных» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="1ce6f-165">Это также запроса XML, что управляемый API EWS отправляет при [поиска для сообщения электронной почты](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="1ce6f-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
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
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1ce6f-166">Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что поиск успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="1ce6f-167">Ответ содержит элемент [сообщения](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) для любого по электронной почте, выполнены условия поиска.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-167">The response contains a [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria.</span></span> <span data-ttu-id="1ce6f-168">В этом случае найти только один электронной почты.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-168">In this case, only one email is found.</span></span> 
  
<span data-ttu-id="1ce6f-169">Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="1ce6f-170">Теперь, когда у вас есть **идентификатор элемента** для электронной почты, который соответствует условиям, можно получить, update или delete, электронной почты с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) - вам не нужно указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="1ce6f-171">Получение, обновление и удаление элементов электронной почты роли представителя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="1ce6f-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-172"></span></span>

<span data-ttu-id="1ce6f-173">Можно использовать управляемый API EWS для получения, обновлять или удалять сообщения электронной почты так же, как выполнять эти действия, если вы не используете делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-173">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="1ce6f-174">Единственное отличие — объект **ExchangeService** для делегата.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-174">The only difference is that the **ExchangeService** object is for the delegate user.</span></span> <span data-ttu-id="1ce6f-175">Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков, в папке "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="1ce6f-176">**В таблице 2. Управляемый API EWS методы работы с электронной почты в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-176">**Table 2. EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="1ce6f-177">**Задача**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-177">**Task**</span></span>|<span data-ttu-id="1ce6f-178">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-178">**EWS Managed API method**</span></span>|<span data-ttu-id="1ce6f-179">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ce6f-180">Получите сообщение электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-180">Get an email</span></span>  <br/> |[<span data-ttu-id="1ce6f-181">Привязка</span><span class="sxs-lookup"><span data-stu-id="1ce6f-181">Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="1ce6f-182">Получение элемента с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="1ce6f-183">Обновление сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-183">Update an email</span></span>  <br/> |<span data-ttu-id="1ce6f-184">[Привязка](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-184">[Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="1ce6f-185">Обновление элемента с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="1ce6f-186">Удаление сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-186">Delete an email</span></span>  <br/> |<span data-ttu-id="1ce6f-187">[Привязка](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-187">[Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="1ce6f-188">Удаление элемента с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="1ce6f-189">Получение, обновление и удаление элементов электронной почты роли представителя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="1ce6f-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="1ce6f-190"></span></span>

<span data-ttu-id="1ce6f-191">Можно использовать управляемый API EWS для получения, обновлять или удалять сообщения электронной почты так же, как выполнять эти действия, если вы не используете делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-191">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="1ce6f-192">Единственное отличие — объект службы для делегата.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="1ce6f-193">Идентификатор элемента, включенных в запрос **GetItem** уникальным образом определяет элемент в хранилище почтовых ящиков, в папке "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ce6f-193">The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="1ce6f-194">**В таблице 3. Операции EWS для работы с электронной почты в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-194">**Table 3. EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="1ce6f-195">**Задача**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-195">**Task**</span></span>|<span data-ttu-id="1ce6f-196">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-196">**EWS operation**</span></span>|<span data-ttu-id="1ce6f-197">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="1ce6f-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ce6f-198">Получите сообщение электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-198">Get an email</span></span>  <br/> |[<span data-ttu-id="1ce6f-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="1ce6f-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="1ce6f-200">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="1ce6f-201">Обновление сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-201">Update an email</span></span>  <br/> |<span data-ttu-id="1ce6f-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="1ce6f-203">Обновление элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="1ce6f-204">Удаление сообщения электронной почты</span><span class="sxs-lookup"><span data-stu-id="1ce6f-204">Delete an email</span></span>  <br/> |<span data-ttu-id="1ce6f-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="1ce6f-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="1ce6f-206">Удаление элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ce6f-207">См. также</span><span class="sxs-lookup"><span data-stu-id="1ce6f-207">See also</span></span>

- [<span data-ttu-id="1ce6f-208">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="1ce6f-209">Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-209">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="1ce6f-210">Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-210">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="1ce6f-211">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="1ce6f-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

