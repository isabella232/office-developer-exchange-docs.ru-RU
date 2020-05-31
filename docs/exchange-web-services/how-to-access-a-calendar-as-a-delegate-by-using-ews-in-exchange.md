---
title: Доступ к календарю как представителю с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Узнайте, как получить доступ к календарю в качестве делегата с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 609e5f0bb22c78174289a2eb10210999c8391a3d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353842"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="18b10-103">Доступ к календарю как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="18b10-104">Узнайте, как получить доступ к календарю в качестве делегата с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="18b10-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="18b10-105">С помощью управляемого API EWS или EWS вы можете предоставить представителю пользователя доступ к папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="18b10-106">После этого делегат может создавать приглашения на собрания от имени владельца почтового ящика, создавать встречи, отвечать на приглашения на собрания, а также получать, обновлять и удалять собрания из папки календаря владельца почтового ящика в зависимости от их разрешений.</span><span class="sxs-lookup"><span data-stu-id="18b10-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="18b10-107">Как представитель вы используете одни и те же методы и операции для доступа к папке календаря владельца почтового ящика, которая используется для доступа к собственной папке календаря.</span><span class="sxs-lookup"><span data-stu-id="18b10-107">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder.</span></span> <span data-ttu-id="18b10-108">Основное отличие заключается в том, что вам необходимо использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создания папки календаря или папки календаря, а затем после определения идентификатора элемента или идентификатора папки можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновления или удаления элемента.</span><span class="sxs-lookup"><span data-stu-id="18b10-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="18b10-109">**Таблица 1. Методы управляемого API EWS и операции EWS для доступа к календарю в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="18b10-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="18b10-110">**Задача**</span><span class="sxs-lookup"><span data-stu-id="18b10-110">**If you want to…**</span></span>|<span data-ttu-id="18b10-111">**Используйте этот метод управляемого API EWS...**</span><span class="sxs-lookup"><span data-stu-id="18b10-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="18b10-112">**Используйте эту операцию EWS...**</span><span class="sxs-lookup"><span data-stu-id="18b10-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18b10-113">Создание собрания или встречи в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="18b10-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="18b10-114">[Встреча. Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="18b10-114">[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="18b10-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="18b10-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="18b10-116">Создание нескольких собраний или встреч в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="18b10-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="18b10-117">[ExchangeService. CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="18b10-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="18b10-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="18b10-119">Поиск или Поиск встречи или собрания в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="18b10-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="18b10-120">[ExchangeService. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-120">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="18b10-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="18b10-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="18b10-122">Получение встречи или собрания в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="18b10-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="18b10-123">Встреча. Bind</span><span class="sxs-lookup"><span data-stu-id="18b10-123">Appointment.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="18b10-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="18b10-124">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="18b10-125">Обновление встречи или собрания в качестве представителя</span><span class="sxs-lookup"><span data-stu-id="18b10-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="18b10-126">[Встреча. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которыми следует [встреча. обновление](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-126">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="18b10-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="18b10-128">Удаление встречи или собрания в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="18b10-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="18b10-129">[Встреча. Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которыми следует [встреча. Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-129">[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="18b10-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="18b10-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="18b10-131">В примерах кода, приведенных в этой статье, primary@contoso.com является владельцем почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="18b10-132">Предварительные задачи</span><span class="sxs-lookup"><span data-stu-id="18b10-132">Prerequisite tasks</span></span>
<span data-ttu-id="18b10-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-133"><a name="bk_prereq"> </a></span></span>

<span data-ttu-id="18b10-134">Прежде чем пользователь сможет получить доступ к папке календаря владельца почтового ящика в качестве представителя, пользователь должен быть [добавлен в качестве представителя с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) в папку календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="18b10-135">Представителю должен быть назначен почтовый ящик, подключенный к своей учетной записи, чтобы обновить календарь владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="18b10-136">Если представителю требуется работать только с приглашениями на собрания и ответами, вы можете добавить делегата в папку "Календарь" и использовать значение перечисления [митингрекуестсделиверископе. делегатесандсендинформатионтоме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS управляемого API или значение **DelegatesAndSendInformationToMe** элемента [деливермитингрекуестс](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS для отправки запросов представителю и информационным сообщениям владельцу почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="18b10-137">После этого делегату не требуется предоставлять доступ к папке "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="18b10-138">Создание собрания или встречи в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="18b10-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-139"><a name="bk_createewsma"> </a></span></span>

<span data-ttu-id="18b10-140">Управляемый API EWS позволяет использовать объект Service для делегированного пользователя для создания элементов календаря для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="18b10-141">В этом примере показано, как использовать метод [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="18b10-141">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="18b10-142">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для делегата, а представителю предоставлены соответствующие разрешения для папки календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
```cs
private static void DelegateAccessCreateMeeting(ExchangeService service)
{
    Appointment meeting = new Appointment(service);
    // Set the properties on the meeting object to create the meeting.
    meeting.Subject = "Team building exercise";
    meeting.Body = "Let's learn to really work as a team and then have lunch!";
    meeting.Start = DateTime.Now.AddDays(2);
    meeting.End = meeting.Start.AddHours(4);
    meeting.Location = "Conference Room 12";
    meeting.RequiredAttendees.Add("sadie@contoso.com");
    meeting.ReminderMinutesBeforeStart = 60;
    // Save the meeting to the Calendar folder for 
    // the mailbox owner and send the meeting request.
    // This method call results in a CreateItem call to EWS.
    meeting.Save(new FolderId(WellKnownFolderName.Calendar, 
        "primary@contoso.com"), 
        SendInvitationsMode.SendToAllAndSaveCopy);
    // Verify that the meeting was created.
    Item item = Item.Bind(service, meeting.Id, new PropertySet(ItemSchema.Subject));
    Console.WriteLine("\nMeeting created: " + item.Subject + "\n");
}
```

<span data-ttu-id="18b10-143">Обратите внимание, что при сохранении элемента вызов метода [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) должен определить папку календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="18b10-144">Если папка календарь владельца почтового ящика не указана, то запрос на собрание сохраняется в календаре представителя, а не в папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="18b10-145">Вы можете включить папку календаря владельца почтового ящика в вызов метода **Save** двумя способами.</span><span class="sxs-lookup"><span data-stu-id="18b10-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="18b10-146">Мы рекомендуем создать экземпляр нового экземпляра объекта [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [веллкновнфолдернаме](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="18b10-147">Тем не менее, сначала можно [выполнить привязывание](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке календаря, а затем использовать идентификатор папки в вызове метода **Save** .</span><span class="sxs-lookup"><span data-stu-id="18b10-147">However, you can also [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="18b10-148">Однако имейте в виду, что при этом создается дополнительный вызов EWS.</span><span class="sxs-lookup"><span data-stu-id="18b10-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address
    // and bind to their Calendar folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryCalendar = Folder.Bind(service, 
        new FolderId(WellKnownFolderName.Calendar, primary)); 
…
    // Save the meeting to the Calendar folder for the mailbox owner and send the meeting request.
    meeting.Save(primaryCalendar.Id, 
        SendInvitationsMode.SendToAllAndSaveCopy);
```

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="18b10-149">Создание собрания или встречи в качестве делегата с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="18b10-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-150"><a name="bk_createews"> </a></span></span>

<span data-ttu-id="18b10-151">Служба EWS позволяет использовать объект Service для делегированного пользователя, чтобы создавать элементы календаря для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-151">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="18b10-152">В этом примере показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="18b10-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="18b10-153">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **Save** для [создания собрания или встречи в качестве делегата](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="18b10-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="18b10-154">Заголовок SOAP был удален из следующего примера для краткости.</span><span class="sxs-lookup"><span data-stu-id="18b10-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
…
  <soap:Body>
    <m:CreateItem SendMeetingInvitations="SendToAllAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:CalendarItem>
          <t:Subject>Team building exercise</t:Subject>
          <t:Body BodyType="HTML">Let's learn to really work as a 
              team and then have lunch!</t:Body>
          <t:ReminderMinutesBeforeStart>60</t:ReminderMinutesBeforeStart>
          <t:Start>2014-03-09T23:26:33.756-05:00</t:Start>
          <t:End>2014-03-10T03:26:33.756-05:00</t:End>
          <t:Location>Conference Room 12</t:Location>
          <t:RequiredAttendees>
            <t:Attendee>
              <t:Mailbox>
                <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
              </t:Mailbox>
            </t:Attendee>
          </t:RequiredAttendees>
        </t:CalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="18b10-155">Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что собрание было создано успешно.</span><span class="sxs-lookup"><span data-stu-id="18b10-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully.</span></span> <span data-ttu-id="18b10-156">Ответ также содержит идентификатор вновь созданного собрания.</span><span class="sxs-lookup"><span data-stu-id="18b10-156">The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="18b10-157">Поиск собрания или встречи в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="18b10-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-158"><a name="bk_searchewsma"> </a></span></span>

<span data-ttu-id="18b10-159">Чтобы найти собрание, необходимо использовать один из методов [ExchangeService. FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включающий параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , чтобы можно было указать папку календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
```cs
static void DelegateAccessSearchWithFilter
    (ExchangeService service, SearchFilter filter)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Define the sort order.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching calendar items. 
        // The FindItems parameters must denote the mailbox owner,
        // mailbox, and Calendar folder.
        // This method call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(
        new FolderId(WellKnownFolderName.Calendar, 
            "primary@contoso.com"), 
            filter, 
            view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while 
            enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="18b10-160">После того как вызов **FindItems** возвратит ответ с идентификатором, вы можете получить, изменить или удалить это собрание с помощью идентификатора и [неявного доступа](delegate-access-and-ews-in-exchange.md#bk_implicit) , а также не указывать SMTP-адрес владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="18b10-161">Поиск собрания или встречи в качестве делегата с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="18b10-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-162"><a name="bk_searchews"> </a></span></span>

<span data-ttu-id="18b10-163">Служба EWS позволяет использовать объект Service для делегированного пользователя для поиска встреч и собраний, соответствующих набору критериев поиска.</span><span class="sxs-lookup"><span data-stu-id="18b10-163">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria.</span></span> <span data-ttu-id="18b10-164">В этом примере показано, как использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для поиска собраний в папке календаря владельца почтового ящика, содержащей слово "здание" в теме.</span><span class="sxs-lookup"><span data-stu-id="18b10-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="18b10-165">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **FindItem** для [поиска собрания или встречи в качестве делегата](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="18b10-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
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
          <t:Constant Value="building" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="18b10-166">Сервер отвечает на запрос **FindItem** с сообщением [финдитемреспонсе](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что поиск успешно завершен.</span><span class="sxs-lookup"><span data-stu-id="18b10-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="18b10-167">Ответ содержит [календаритем](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для всех встреч или собраний, отвечающих условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="18b10-167">The response contains a [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria.</span></span> <span data-ttu-id="18b10-168">В этом случае найдено только одно собрание.</span><span class="sxs-lookup"><span data-stu-id="18b10-168">In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="18b10-169">Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) было сокращено для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="18b10-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
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
              <t:CalendarItem>
                <t:ItemId Id="IJpUAAA="
                          ChangeKey="DwAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAAAIKhS" />
                <t:Subject>Team building exercise</t:Subject>
                <t:DateTimeReceived>2014-03-04T21:27:22Z</t:DateTimeReceived>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="18b10-170">Теперь, когда у вас есть **идентификатор элемента для** собрания, который соответствует вашим условиям, вы можете получить, изменить или удалить это собрание с помощью элемента **ItemId** и [неявного доступа](delegate-access-and-ews-in-exchange.md#bk_implicit) , а также не указывать SMTP-адрес владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="18b10-171">Получение, обновление и удаление элементов календаря в качестве делегата с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="18b10-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-172"><a name="bk_geteswma"> </a></span></span>

<span data-ttu-id="18b10-173">С помощью управляемого API EWS можно получить, обновить или удалить собрание или встречу так же, как и при использовании делегированного доступа.</span><span class="sxs-lookup"><span data-stu-id="18b10-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="18b10-174">Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="18b10-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="18b10-175">Идентификатор элемента, включенный в вызов метода **BIND** , уникальным образом определяет элемент в хранилище почтовых ящиков в папке "Календарь" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="18b10-176">**Таблица 2. Методы управляемого API EWS для работы с встречами и собраниями в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="18b10-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="18b10-177">**Задача**</span><span class="sxs-lookup"><span data-stu-id="18b10-177">**Task**</span></span>|<span data-ttu-id="18b10-178">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="18b10-178">**EWS Managed API method**</span></span>|<span data-ttu-id="18b10-179">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="18b10-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18b10-180">Получение встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="18b10-181">Базу</span><span class="sxs-lookup"><span data-stu-id="18b10-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="18b10-182">Получение элемента с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="18b10-183">Обновление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="18b10-184">[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Обновление](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="18b10-185">Обновление собрания с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="18b10-186">Удаление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="18b10-187">[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Удаление](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="18b10-188">Удаление собрания с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="18b10-189">Получение, обновление и удаление элементов календаря в качестве делегата с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="18b10-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="18b10-190"><a name="bk_getews"> </a></span></span>

<span data-ttu-id="18b10-191">С помощью EWS можно получить, обновить или удалить собрание или встречу так же, как и при использовании делегированного доступа.</span><span class="sxs-lookup"><span data-stu-id="18b10-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="18b10-192">Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя.</span><span class="sxs-lookup"><span data-stu-id="18b10-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="18b10-193">Идентификатор элемента, включенный в вызов метода [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , однозначно определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="18b10-193">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="18b10-194">**Таблица 3. Операции EWS для работы с встречами и собраниями в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="18b10-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="18b10-195">**Task**</span><span class="sxs-lookup"><span data-stu-id="18b10-195">**Task**</span></span>|<span data-ttu-id="18b10-196">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="18b10-196">**EWS operation**</span></span>|<span data-ttu-id="18b10-197">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="18b10-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="18b10-198">Получение встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="18b10-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="18b10-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="18b10-200">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="18b10-201">Обновление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="18b10-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="18b10-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="18b10-203">Обновление собрания с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="18b10-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="18b10-204">Удаление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="18b10-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="18b10-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="18b10-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="18b10-206">См. также</span><span class="sxs-lookup"><span data-stu-id="18b10-206">See also</span></span>

- [<span data-ttu-id="18b10-207">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="18b10-208">Добавление и удаление делегатов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="18b10-209">Задание разрешений для папки другого пользователя с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="18b10-210">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="18b10-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

