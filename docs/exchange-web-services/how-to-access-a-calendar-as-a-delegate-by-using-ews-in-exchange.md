---
title: Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Узнайте, как получить доступ к роли представителя календаря с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 24327c28f58e728807fc5581b480d3c01d3b7208
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760974"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="aae60-103">Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-103">Access a calendar as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="aae60-104">Узнайте, как получить доступ к роли представителя календаря с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="aae60-104">Learn how to access a calendar as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="aae60-105">Можно использовать управляемый API EWS или делегирование EWS, чтобы предоставить пользователю доступ к папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-105">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Calendar folder.</span></span> <span data-ttu-id="aae60-106">Делегат можно затем Создание приглашений на собрания от имени владельца почтового ящика, Создание встречи, ответ на приглашения на собрания и извлечь, обновление и удаление собрания из папки календаря владельца почтового ящика, в зависимости от их разрешения.</span><span class="sxs-lookup"><span data-stu-id="aae60-106">The delegate can then create meeting requests on behalf of the mailbox owner, create appointments, respond to meeting requests, and retrieve, update, and delete meetings from the mailbox owner's Calendar folder, depending on their permissions.</span></span>
  
<span data-ttu-id="aae60-107">Роли представителя используйте ту же методов и операций на доступ к папке календаря владельца почтового ящика, которая используется для доступа к папке календаря.</span><span class="sxs-lookup"><span data-stu-id="aae60-107">As a delegate, you use the same methods and operations to access a mailbox owner's Calendar folder that you use to access your own Calendar folder.</span></span> <span data-ttu-id="aae60-108">Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создание элемента календаря или вложенной папке календаря и затем после определения идентификатор элемента или идентификатор папки можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент.</span><span class="sxs-lookup"><span data-stu-id="aae60-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a calendar item or calendar subfolder, and then after you identify the item ID or folder ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="aae60-109">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к календарю роли представителя**</span><span class="sxs-lookup"><span data-stu-id="aae60-109">**Table 1. EWS Managed API methods and EWS operations for accessing a calendar as a delegate**</span></span>

|<span data-ttu-id="aae60-110">**Если вы хотите...**</span><span class="sxs-lookup"><span data-stu-id="aae60-110">**If you want to…**</span></span>|<span data-ttu-id="aae60-111">**Используйте этот метод управляемый API EWS...**</span><span class="sxs-lookup"><span data-stu-id="aae60-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="aae60-112">**Используйте эту операцию EWS...**</span><span class="sxs-lookup"><span data-stu-id="aae60-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aae60-113">Создание собрания или встречи в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-113">Create a meeting or appointment as a delegate</span></span>  <br/> |<span data-ttu-id="aae60-114">[Appointment.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-114">[Appointment.Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="aae60-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="aae60-116">Создание нескольких собрания или встречи в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-116">Create multiple meetings or appointments as a delegate</span></span>  <br/> |<span data-ttu-id="aae60-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="aae60-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="aae60-119">Поиск или поиск встречи или собрания в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-119">Search for or find an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="aae60-120">[ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-120">[ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Calendar folder</span></span>  <br/> |<span data-ttu-id="aae60-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика</span><span class="sxs-lookup"><span data-stu-id="aae60-121">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="aae60-122">Получение встречи или собрания в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-122">Get an appointment or meeting as a delegate</span></span>  <br/> |[<span data-ttu-id="aae60-123">Appointment.Bind</span><span class="sxs-lookup"><span data-stu-id="aae60-123">Appointment.Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="aae60-124">GetItem</span><span class="sxs-lookup"><span data-stu-id="aae60-124">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="aae60-125">Обновление встречи или собрания в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-125">Update an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="aae60-126">[Appointment.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Appointment.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-126">[Appointment.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="aae60-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-127">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="aae60-128">Удаление встречи или собрания в качестве делегата</span><span class="sxs-lookup"><span data-stu-id="aae60-128">Delete an appointment or meeting as a delegate</span></span>  <br/> |<span data-ttu-id="aae60-129">[Appointment.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-129">[Appointment.Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="aae60-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="aae60-131">В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-131">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="aae60-132">Обязательные задачи</span><span class="sxs-lookup"><span data-stu-id="aae60-132">Prerequisite tasks</span></span>
<span data-ttu-id="aae60-133"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-133"></span></span>

<span data-ttu-id="aae60-134">Пользователь может получить доступ к папки календаря владельца почтового ящика в качестве делегата, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-134">Before a user can access a mailbox owner's Calendar folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="aae60-135">Делегат должен иметь почтового ящика, подключенного к своей учетной записи для обновления календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-135">A delegate must have a mailbox attached to their account to update the calendar of a mailbox owner.</span></span>
  
<span data-ttu-id="aae60-136">Если представителю требуется для работы с приглашений на собрания и ответы, можно добавить делегата к папке календаря и используйте значение перечисления управляемый API EWS [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) по умолчанию или [ DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) веб-служб Exchange имеет значение **DelegatesAndSendInformationToMe** для отправки запросов к делегат и информационные сообщения владельцу почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-136">If a delegate needs to work with meeting requests and responses only, you can add the delegate to the Calendar folder, and use the default [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS Managed API enumeration value or the [DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS element value of **DelegatesAndSendInformationToMe** to send the requests to the delegate and informational messages to the mailbox owner.</span></span> <span data-ttu-id="aae60-137">Делегат затем не требуется предоставить доступ к папке "Входящие" владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-137">The delegate then does not need to be given access to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="aae60-138">Создание собрания или встречи в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-138">Create a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="aae60-139"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-139"></span></span>

<span data-ttu-id="aae60-140">Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания элементов календаря для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-140">The EWS Managed API enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="aae60-141">В этом примере показано, как использовать метод [сохранения](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="aae60-141">This example shows how to use the [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="aae60-142">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата предоставлены необходимые разрешения для папки календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="aae60-143">Обратите внимание, что при сохранении элемента вызова метода [Сохранить](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) необходимо определить папки календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="aae60-144">Если папки календаря владельца почтового ящика не указан, запрос на собрание получает сохранены делегата календаря и не папки календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-144">If the mailbox owner's Calendar folder is not specified, the meeting request gets saved to the delegate's calendar and not the mailbox owner's Calendar folder.</span></span> <span data-ttu-id="aae60-145">Может включать папки календаря владельца почтового ящика в вызове метода **Сохранить** двумя способами.</span><span class="sxs-lookup"><span data-stu-id="aae60-145">You can include the mailbox owner's Calendar folder in the **Save** method call in two ways.</span></span> <span data-ttu-id="aae60-146">Рекомендуется создать новый экземпляр объекта [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

<span data-ttu-id="aae60-147">Тем не менее, можно также [привязать](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке календаря во-первых и затем используйте идентификатор папки в вызове метода **сохранения** .</span><span class="sxs-lookup"><span data-stu-id="aae60-147">However, you can also [Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Calendar folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="aae60-148">Однако следует помнить, что при этом создается дополнительных вызовов веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="aae60-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="aae60-149">Создание собрания или встречи в качестве делегата с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-149">Create a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="aae60-150"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-150"></span></span>

<span data-ttu-id="aae60-151">Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания элементов календаря для владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-151">EWS enables you to use the service object for the delegate user to create calendar items for the mailbox owner.</span></span> <span data-ttu-id="aae60-152">В этом примере показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания и отправки приглашений на собрание участникам.</span><span class="sxs-lookup"><span data-stu-id="aae60-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="aae60-153">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **Save** для [создания собрания или встречи в качестве делегата](#bk_createewsma).</span><span class="sxs-lookup"><span data-stu-id="aae60-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a meeting or appointment as a delegate](#bk_createewsma).</span></span>
  
<span data-ttu-id="aae60-154">В следующем примере для краткости был удален заголовка SOAP.</span><span class="sxs-lookup"><span data-stu-id="aae60-154">The SOAP header has been removed from the following example for brevity.</span></span>
  
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

<span data-ttu-id="aae60-155">Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что собрания был успешно создан.</span><span class="sxs-lookup"><span data-stu-id="aae60-155">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the meeting was created successfully.</span></span> <span data-ttu-id="aae60-156">Ответ также содержит идентификатор элемента для только что созданный собрания.</span><span class="sxs-lookup"><span data-stu-id="aae60-156">The response also contains the item ID of the newly created meeting.</span></span>
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="aae60-157">Поиск собрания или встречи в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-157">Search for a meeting or appointment as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="aae60-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-158"></span></span>

<span data-ttu-id="aae60-159">Для поиска собрания, необходимо использовать один из методов [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-159">To search for a meeting, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Calendar folder.</span></span> 
  
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

<span data-ttu-id="aae60-160">После вызова **FindItems** возвращает ответ с кодом, можно получить, обновлении или удалении этого собрания с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) , и необходимо указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that meeting by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a><span data-ttu-id="aae60-161">Поиск собрания или встречи в качестве делегата с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-161">Search for a meeting or appointment as a delegate by using EWS</span></span>
<span data-ttu-id="aae60-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-162"></span></span>

<span data-ttu-id="aae60-163">Веб-служб Exchange позволяет использовать объект службы для делегата поиск встречи и собрания, которые соответствуют заданным условиям поиска.</span><span class="sxs-lookup"><span data-stu-id="aae60-163">EWS enables you to use the service object for the delegate user to search for appointments and meetings that meet a set of search criteria.</span></span> <span data-ttu-id="aae60-164">В этом примере показано, как использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) найти собраний в папке календаря владельца почтового ящика, содержащие слово «создание» в теме сообщения.</span><span class="sxs-lookup"><span data-stu-id="aae60-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Calendar folder that contain the word "building" in the subject.</span></span> 
  
<span data-ttu-id="aae60-165">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindItem** для [поиска для собрания или встречи в качестве делегата](#bk_searchewsma).</span><span class="sxs-lookup"><span data-stu-id="aae60-165">This is also the XML request that the EWS Managed API sends when you use the **FindItem** method to [search for a meeting or appointment as a delegate](#bk_searchewsma).</span></span>
  
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

<span data-ttu-id="aae60-166">Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что поиск успешно завершена.</span><span class="sxs-lookup"><span data-stu-id="aae60-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="aae60-167">Ответ содержит [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для встречи или собрания, выполнены условия поиска.</span><span class="sxs-lookup"><span data-stu-id="aae60-167">The response contains a [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) for any appointments or meetings that met the search criteria.</span></span> <span data-ttu-id="aae60-168">В этом случае найти только одного собрания.</span><span class="sxs-lookup"><span data-stu-id="aae60-168">In this case, only one meeting is found.</span></span> 
  
<span data-ttu-id="aae60-169">Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="aae60-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="aae60-170">Теперь, когда у вас есть **ItemId** собрания, который соответствует условиям, можно получить, обновлении или удалении этого собрания с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) , и необходимо указать SMTP-адреса владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-170">Now that you have the **ItemId** for the meeting that meets your criteria, you can get, update, or delete that meeting by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) — and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="aae60-171">Получение, обновление и удаление элементов календаря роли представителя с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-171">Get, update, or delete calendar items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="aae60-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-172"></span></span>

<span data-ttu-id="aae60-173">Можно использовать управляемый API EWS для получения, обновить или удалить собрание или встречу так же, как выполнять эти действия, если вы не используете делегированный доступ.</span><span class="sxs-lookup"><span data-stu-id="aae60-173">You can use the EWS Managed API to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="aae60-174">Единственное отличие — объект службы для делегата.</span><span class="sxs-lookup"><span data-stu-id="aae60-174">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="aae60-175">Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="aae60-176">**В таблице 2. Управляемый API EWS методы для работы с встречи и собрания роли представителя**</span><span class="sxs-lookup"><span data-stu-id="aae60-176">**Table 2. EWS Managed API methods for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="aae60-177">**Задача**</span><span class="sxs-lookup"><span data-stu-id="aae60-177">**Task**</span></span>|<span data-ttu-id="aae60-178">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="aae60-178">**EWS Managed API method**</span></span>|<span data-ttu-id="aae60-179">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="aae60-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aae60-180">Получение встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-180">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="aae60-181">Привязка</span><span class="sxs-lookup"><span data-stu-id="aae60-181">Bind</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="aae60-182">Получение элемента с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="aae60-183">Обновление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-183">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="aae60-184">[Привязка](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-184">[Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="aae60-185">Обновление собрания с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-185">Update a meeting by using the EWS Managed API</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|<span data-ttu-id="aae60-186">Удаление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-186">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="aae60-187">[Привязка](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-187">[Bind](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="aae60-188">Удаление собрания с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-188">Delete a meeting by using the EWS Managed API</span></span>](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="aae60-189">Получение, обновление и удаление элементов календаря роли представителя с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-189">Get, update, or delete calendar items as a delegate by using EWS</span></span>
<span data-ttu-id="aae60-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="aae60-190"></span></span>

<span data-ttu-id="aae60-191">Чтобы получить, обновить или удалить собрания или встречи так же, как выполнять эти действия, если вы не используете делегированный доступ, можно использовать веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="aae60-191">You can use EWS to get, update, or delete a meeting or appointment in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="aae60-192">Единственное отличие — объект службы для делегата.</span><span class="sxs-lookup"><span data-stu-id="aae60-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="aae60-193">Идентификатор элемента, включенные в вызове метода [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) уникальным образом определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="aae60-193">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) method call uniquely identifies the item in the mailbox store, in the mailbox owner's Calendar folder.</span></span> 
  
<span data-ttu-id="aae60-194">**В таблице 3. Операции EWS для работы с встречи и собрания в качестве делегата**</span><span class="sxs-lookup"><span data-stu-id="aae60-194">**Table 3. EWS operations for working with appointments and meetings as a delegate**</span></span>

|<span data-ttu-id="aae60-195">**Задача**</span><span class="sxs-lookup"><span data-stu-id="aae60-195">**Task**</span></span>|<span data-ttu-id="aae60-196">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="aae60-196">**EWS operation**</span></span>|<span data-ttu-id="aae60-197">**Пример кода**</span><span class="sxs-lookup"><span data-stu-id="aae60-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="aae60-198">Получение встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-198">Get an appointment or meeting</span></span>  <br/> |[<span data-ttu-id="aae60-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="aae60-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="aae60-200">Получение элемента с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="aae60-201">Обновление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-201">Update an appointment or meeting</span></span>  <br/> |<span data-ttu-id="aae60-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="aae60-203">Обновление собрания с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-203">Update a meeting by using EWS</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|<span data-ttu-id="aae60-204">Удаление встречи или собрания</span><span class="sxs-lookup"><span data-stu-id="aae60-204">Delete an appointment or meeting</span></span>  <br/> |<span data-ttu-id="aae60-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="aae60-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aae60-206">См. также</span><span class="sxs-lookup"><span data-stu-id="aae60-206">See also</span></span>

- [<span data-ttu-id="aae60-207">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-207">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)   
- [<span data-ttu-id="aae60-208">Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-208">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="aae60-209">Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-209">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="aae60-210">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="aae60-210">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

