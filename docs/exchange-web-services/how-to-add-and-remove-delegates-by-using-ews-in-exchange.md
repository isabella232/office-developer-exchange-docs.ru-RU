---
title: Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Узнайте, как делегатов, которые будут добавлять или удалять делегатов из почтовых ящиков пользователей с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: d55ef6c5c4e434603d293dbe30c6147ceb73b08b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760970"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a><span data-ttu-id="37e2c-103">Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-103">Add and remove delegates by using EWS in Exchange</span></span>

<span data-ttu-id="37e2c-104">Узнайте, как делегатов, которые будут добавлять или удалять делегатов из почтовых ящиков пользователей с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-104">Learn how to add delegates to or remove delegates from users' mailboxes by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="37e2c-105">Можно использовать управляемый API EWS или веб-служб Exchange для включения делегатов, которые будут действовать от имени владельца почтового ящика или удаления делегированный доступ к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="37e2c-105">You can use the EWS Managed API or EWS to enable delegates to act on behalf of a mailbox owner or remove a delegate's access to a mailbox.</span></span> <span data-ttu-id="37e2c-106">Пользователи, использующие добавляются в качестве делегата, предоставляемые разрешения, может выполнять задачи от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37e2c-106">Users who are added as a delegate, and are given permissions, can perform tasks on behalf of the mailbox owner.</span></span> <span data-ttu-id="37e2c-107">Например их можно создавать и отправлять приглашения на собрания, отправлять по электронной почте и ответ на приглашение на собрание от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="37e2c-107">For example, they can create and send meeting invitations, send emails, and respond to meeting requests on the mailbox owner's behalf.</span></span> 
  
<span data-ttu-id="37e2c-108">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для добавления и удаления делегатов**</span><span class="sxs-lookup"><span data-stu-id="37e2c-108">**Table 1. EWS Managed API methods and EWS operations for adding and removing delegates**</span></span>

|<span data-ttu-id="37e2c-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="37e2c-109">**Task**</span></span>|<span data-ttu-id="37e2c-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="37e2c-110">**EWS Managed API method**</span></span>|<span data-ttu-id="37e2c-111">**Операция служб EWS**</span><span class="sxs-lookup"><span data-stu-id="37e2c-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="37e2c-112">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="37e2c-112">Add delegates</span></span>  <br/> |[<span data-ttu-id="37e2c-113">ExchangeService.AddDelegates</span><span class="sxs-lookup"><span data-stu-id="37e2c-113">ExchangeService.AddDelegates</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="37e2c-114">Метод AddDelegate</span><span class="sxs-lookup"><span data-stu-id="37e2c-114">AddDelegate</span></span>](http://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="37e2c-115">Удаление делегатов</span><span class="sxs-lookup"><span data-stu-id="37e2c-115">Remove delegates</span></span>  <br/> |[<span data-ttu-id="37e2c-116">ExchangeService.RemoveDelegates</span><span class="sxs-lookup"><span data-stu-id="37e2c-116">ExchangeService.RemoveDelegates</span></span>](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="37e2c-117">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="37e2c-117">RemoveDelegate</span></span>](http://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="37e2c-118">После предоставления разрешений на папку делегата, они влияют на элементы в папке и всех вложенных папках в соответствии с их [делегировать разрешения](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="37e2c-118">After a delegate is granted permissions to a folder, they can act on items in the folder and any subfolders, according to their [delegate permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span> <span data-ttu-id="37e2c-119">Разрешения для делегатов применяются только к вложенных папок, созданных после предоставления доступа делегата.</span><span class="sxs-lookup"><span data-stu-id="37e2c-119">Permissions for delegates only apply to subfolders that are created after the delegate access was granted.</span></span> <span data-ttu-id="37e2c-120">Обновление разрешений папки для уже существующей папки или другие папки, см [папки другого пользователя с помощью веб-служб Exchange в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="37e2c-120">To update folder permissions for pre-existing folders, or other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="37e2c-121">Обратите внимание на то, что делегаты можно добавить только в почтовые ящики, включая группы безопасности с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="37e2c-121">Note that delegates can only be added to mailbox-enabled accounts, including mail-enabled security groups.</span></span> <span data-ttu-id="37e2c-122">По умолчанию в одном вызове доступа делегата веб-служб Exchange можно получить доступ не более 255 разных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="37e2c-122">By default, a single EWS delegate access call can access a maximum of 255 different mailboxes.</span></span>

<span data-ttu-id="37e2c-123"><a name="bk_adddelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="37e2c-123"></span></span>

## <a name="add-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="37e2c-124">Добавление делегатов с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-124">Add delegates by using the EWS Managed API</span></span>

<span data-ttu-id="37e2c-125">Можно добавить делегатов к почтовому ящику с помощью метода [AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-125">You can add delegates to a mailbox by using the [AddDelegates](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="37e2c-126">В этом примере, нового календаря, контактов и электронной почты [DelegateUser](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) создается объект, и каждый делегат предоставляется [Редактор разрешения](delegate-access-and-ews-in-exchange.md#bk_delegateperms) соответствующей папке.</span><span class="sxs-lookup"><span data-stu-id="37e2c-126">In this example, a new calendar, contact, and email [DelegateUser](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) object is created, and each delegate is given [Editor permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms) for their respective folder.</span></span> <span data-ttu-id="37e2c-127">Пример, чтобы добавить делегат для любой из папки, указанные с помощью [Свойства DelegatePermissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx)можно изменить, и можно задать разрешения для любого значения, заданные в перечислении [DelegateFolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="37e2c-127">You can modify the example to add a delegate to any of the folders specified by the [DelegatePermissions properties](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), and you can set the permissions to any of the values specified by the [DelegateFolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) enumeration.</span></span> 
  
<span data-ttu-id="37e2c-128">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-128">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> AddDelegates(ExchangeService service)
{
    // Create a list to hold the new delegates to add.
    List<DelegateUser> newDelegates = new System.Collections.Generic.List<DelegateUser>();
    // Create a new delegate that has editor access to the mailbox owner's Calendar folder.
    DelegateUser calendarDelegate = new DelegateUser("calendardelegate@contoso.com");
    calendarDelegate.Permissions.CalendarFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(calendarDelegate);
    // Create a new delegate that has editor access to the mailbox owner's Contacts folder.
    DelegateUser contactDelegate = new DelegateUser("contactdelegate@contoso.com");
    contactDelegate.Permissions.ContactsFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(contactDelegate);
            
    // Create a new delegate that has editor access to the mailbox owner's Inbox folder.
    DelegateUser emailDelegate = new DelegateUser("emaildelegate@contoso.com");
    emailDelegate.Permissions.InboxFolderPermissionLevel = DelegateFolderPermissionLevel.Editor;
    // Add the delegate to the list of new delegates.
    newDelegates.Add(emailDelegate);
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.AddDelegates(mailbox, MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe, newDelegates);
            
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("For delegate " + resp.DelegateUser.UserId.PrimarySmtpAddress.ToString());
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
        Console.WriteLine("\r\n");
    }
    return response;
}
```

<span data-ttu-id="37e2c-129"><a name="bk_adddelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="37e2c-129"></span></span>

## <a name="add-delegates-by-using-ews"></a><span data-ttu-id="37e2c-130">Добавление делегатов с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-130">Add delegates by using EWS</span></span>

<span data-ttu-id="37e2c-131">В следующем примере кода показано, как добавить отдельный календарь, контакта и делегаты электронной почты с помощью операции [AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-131">The following code example shows how to add separate calendar, contact, and email delegates by using the [AddDelegate](http://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="37e2c-132">Почтовый ящик для изменения задается с помощью элемента [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) и параметры [разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms) для каждого делегата содержащиеся в элементе [DelegateUser](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="37e2c-132">The mailbox to modify is specified by the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element, and the [permission](delegate-access-and-ews-in-exchange.md#bk_delegateperms) settings for each delegate are contained in the [DelegateUser](http://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="37e2c-133">Каждый из делегаты имеет разрешений редактора их целевую папку.</span><span class="sxs-lookup"><span data-stu-id="37e2c-133">Each of the delegates has been granted Editor permissions to their target folder.</span></span> 
  
<span data-ttu-id="37e2c-134">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **AddDelegates** для [добавления делегатов](#bk_adddelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="37e2c-134">This is also the XML request that the EWS Managed API sends when you use the **AddDelegates** method to [add delegates](#bk_adddelegateewsma).</span></span>
  
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
    <m:AddDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:DelegateUsers>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>Editor</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>None</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>Editor</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
        <t:DelegateUser>
          <t:UserId>
            <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
          </t:UserId>
          <t:DelegatePermissions>
            <t:CalendarFolderPermissionLevel>None</t:CalendarFolderPermissionLevel>
            <t:TasksFolderPermissionLevel>None</t:TasksFolderPermissionLevel>
            <t:InboxFolderPermissionLevel>Editor</t:InboxFolderPermissionLevel>
            <t:ContactsFolderPermissionLevel>None</t:ContactsFolderPermissionLevel>
            <t:NotesFolderPermissionLevel>None</t:NotesFolderPermissionLevel>
            <t:JournalFolderPermissionLevel>None</t:JournalFolderPermissionLevel>
          </t:DelegatePermissions>
          <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
          <t:ViewPrivateItems>false</t:ViewPrivateItems>
        </t:DelegateUser>
      </m:DelegateUsers>
      <m:DeliverMeetingRequests>DelegatesAndSendInformationToMe</m:DeliverMeetingRequests>
    </m:AddDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="37e2c-135">Сервер отвечает на запрос **AddDelegate** с [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) сообщения, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что делегаты успешно созданы.</span><span class="sxs-lookup"><span data-stu-id="37e2c-135">The server responds to the **AddDelegate** request with an [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully created.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:ResponseMessages>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535221</t:SID>
              <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>calendardelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535264</t:SID>
              <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>contactdelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
        <m:DelegateUserResponseMessageType ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:DelegateUser>
            <t:UserId>
              <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
              <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
              <t:DisplayName>emaildelegate</t:DisplayName>
            </t:UserId>
            <t:ReceiveCopiesOfMeetingMessages>false</t:ReceiveCopiesOfMeetingMessages>
            <t:ViewPrivateItems>false</t:ViewPrivateItems>
          </m:DelegateUser>
        </m:DelegateUserResponseMessageType>
      </m:ResponseMessages>
    </m:AddDelegateResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="37e2c-136"><a name="bk_removedelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="37e2c-136"></span></span>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="37e2c-137">Удаление делегаты с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-137">Remove delegates by using the EWS Managed API</span></span>

<span data-ttu-id="37e2c-138">Делегаты можно удалить из целевого почтового ящика с помощью метода [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-138">You can remove delegates from a target mailbox by using the [ExchangeService.RemoveDelegates](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="37e2c-139">В этом примере удаляются делегат разрешения, заданные в разделе [Добавление примера делегата](#bk_adddelegateewsma) .</span><span class="sxs-lookup"><span data-stu-id="37e2c-139">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateewsma) are removed.</span></span> 
  
<span data-ttu-id="37e2c-140">В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) владельца почтового ящика, а пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-140">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
public static Collection<DelegateUserResponse> RemoveDelegates(ExchangeService service)
{
    // Create a list to hold the delegates to delete.
    List<UserId> deletedDelegates = new System.Collections.Generic.List<UserId>();
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("calendardelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("contactdelegate@contoso.com");
    // Add the delegate to the list of new delegates.
    deletedDelegates.Add("emaildelegate@contoso.com");
    // Create a mailbox object that represents the mailbox owner.
    Mailbox mailbox = new Mailbox("primary@contoso.com");
    // Call the AddDelegates method to add the delegates to the target mailbox.
    Collection<DelegateUserResponse> response = service.RemoveDelegates(mailbox, deletedDelegates);
    foreach (DelegateUserResponse resp in response)
    {
        // Print out the result and the last eight characters of the item ID.
        Console.WriteLine("Result: {0}", resp.Result);
        Console.WriteLine("Error Code: {0}", resp.ErrorCode);
        Console.WriteLine("ErrorMessage: {0}\r\n", resp.ErrorMessage);
    }
    return response;
}
```

<span data-ttu-id="37e2c-141"><a name="bk_removedelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="37e2c-141"></span></span>

## <a name="remove-delegates-by-using-ews"></a><span data-ttu-id="37e2c-142">Удаление делегаты с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-142">Remove delegates by using EWS</span></span>

<span data-ttu-id="37e2c-143">Делегаты можно удалить из почтового ящика с помощью операции [RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="37e2c-143">You can remove delegates from a mailbox by using the [RemoveDelegate](http://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="37e2c-144">В этом примере удаляются делегат разрешения, заданные в разделе [Добавление примера делегата](#bk_adddelegateews) .</span><span class="sxs-lookup"><span data-stu-id="37e2c-144">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateews) are removed.</span></span> 
  
<span data-ttu-id="37e2c-145">Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **RemoveDelegates** для [удаления делегатов](#bk_removedelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="37e2c-145">This is also the XML request that the EWS Managed API sends when you use the **RemoveDelegates** method to [remove delegates](#bk_removedelegateewsma).</span></span>
  
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
    <m:RemoveDelegate>
      <m:Mailbox>
        <t:EmailAddress>primary@contoso.com</t:EmailAddress>
      </m:Mailbox>
      <m:UserIds>
        <t:UserId>
          <t:PrimarySmtpAddress>calendardelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>contactdelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
        <t:UserId>
          <t:PrimarySmtpAddress>emaildelegate@contoso.com</t:PrimarySmtpAddress>
        </t:UserId>
      </m:UserIds>
    </m:RemoveDelegate>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="37e2c-146">Сервер отвечает на запрос **RemoveDelegate** [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что делегаты были успешно удалены.</span><span class="sxs-lookup"><span data-stu-id="37e2c-146">The server responds to the **RemoveDelegate** request with a [AddDelegateResponse](http://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully removed.</span></span>

<span data-ttu-id="37e2c-147"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="37e2c-147"></span></span>

## <a name="next-steps"></a><span data-ttu-id="37e2c-148">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="37e2c-148">Next steps</span></span>

<span data-ttu-id="37e2c-149">После добавления делегатов календаря, электронной почты и папки задач делегат может получить доступ к элементов в папках.</span><span class="sxs-lookup"><span data-stu-id="37e2c-149">After you add delegates to calendar, email, and task folders, the delegate can access the items in the folders.</span></span> <span data-ttu-id="37e2c-150">Для получения дополнительных сведений обратитесь к следующим статьям:</span><span class="sxs-lookup"><span data-stu-id="37e2c-150">To learn more, see the following articles:</span></span>
  
- [<span data-ttu-id="37e2c-151">Доступ к электронной почте в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-151">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="37e2c-152">Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-152">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="37e2c-153">Контакты доступа роли представителя с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-153">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
<span data-ttu-id="37e2c-154">Папки, для которых вы добавили делегаты включается дочерних папок, которые были созданы перед предоставлением делегированный доступ, делегат не сможет получить доступ к этих папок без дополнительных разрешений.</span><span class="sxs-lookup"><span data-stu-id="37e2c-154">If the folders for which you added delegates include child folders that were created before you granted the delegate access, the delegate will not be able to access those folders without additional permissions.</span></span> <span data-ttu-id="37e2c-155">Для добавления разрешений или изменение разрешений для других папок, содержатся в разделе [Задание разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="37e2c-155">To add these permissions, or modify permissions for any other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="37e2c-156">См. также</span><span class="sxs-lookup"><span data-stu-id="37e2c-156">See also</span></span>

- [<span data-ttu-id="37e2c-157">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="37e2c-157">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="37e2c-158">Exchange 2013: Добавление программным путем делегирования пользователей учетной записи электронной почты</span><span class="sxs-lookup"><span data-stu-id="37e2c-158">Exchange 2013: Add delegate users to an email account programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [<span data-ttu-id="37e2c-159">Exchange 2013: Обновление делегаты, связанные с учетными записями электронной почты программными средствами</span><span class="sxs-lookup"><span data-stu-id="37e2c-159">Exchange 2013: Update delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [<span data-ttu-id="37e2c-160">Exchange 2013: Удаление делегатов, связанные с учетными записями электронной почты программными средствами</span><span class="sxs-lookup"><span data-stu-id="37e2c-160">Exchange 2013: Remove delegates associated with email accounts programmatically</span></span>](http://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

