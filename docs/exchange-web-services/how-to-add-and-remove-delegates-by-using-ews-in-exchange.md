---
title: Добавление и удаление делегатов с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: cc7760bf-633b-483a-84ae-b52f437af2d3
description: Узнайте, как добавлять делегаты или удалять делегаты из почтовых ящиков пользователей с помощью управляемого API EWS или EWS в Exchange.
ms.openlocfilehash: 9db0171db51c0847d54bbcec7e28937eaed18d43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455340"
---
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a><span data-ttu-id="7bb50-103">Добавление и удаление делегатов с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb50-103">Add and remove delegates by using EWS in Exchange</span></span>

<span data-ttu-id="7bb50-104">Узнайте, как добавлять делегаты или удалять делегаты из почтовых ящиков пользователей с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bb50-104">Learn how to add delegates to or remove delegates from users' mailboxes by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="7bb50-105">Вы можете использовать управляемый API EWS или EWS, чтобы позволить представителям действовать от имени владельца почтового ящика или удалять доступ представителя к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="7bb50-105">You can use the EWS Managed API or EWS to enable delegates to act on behalf of a mailbox owner or remove a delegate's access to a mailbox.</span></span> <span data-ttu-id="7bb50-106">Пользователи, добавленные в качестве представителей и обладающие разрешениями, могут выполнять задачи от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7bb50-106">Users who are added as a delegate, and are given permissions, can perform tasks on behalf of the mailbox owner.</span></span> <span data-ttu-id="7bb50-107">Например, они могут создавать и отправлять приглашения на собрания, отправлять сообщения электронной почты и отвечать на приглашения на собрания от имени владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7bb50-107">For example, they can create and send meeting invitations, send emails, and respond to meeting requests on the mailbox owner's behalf.</span></span> 
  
<span data-ttu-id="7bb50-108">**Таблица 1. Методы управляемого API EWS и операции EWS для добавления и удаления делегатов**</span><span class="sxs-lookup"><span data-stu-id="7bb50-108">**Table 1. EWS Managed API methods and EWS operations for adding and removing delegates**</span></span>

|<span data-ttu-id="7bb50-109">**Задача**</span><span class="sxs-lookup"><span data-stu-id="7bb50-109">**Task**</span></span>|<span data-ttu-id="7bb50-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="7bb50-110">**EWS Managed API method**</span></span>|<span data-ttu-id="7bb50-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="7bb50-111">**EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7bb50-112">Добавление делегатов</span><span class="sxs-lookup"><span data-stu-id="7bb50-112">Add delegates</span></span>  <br/> |[<span data-ttu-id="7bb50-113">ExchangeService. Аддделегатес</span><span class="sxs-lookup"><span data-stu-id="7bb50-113">ExchangeService.AddDelegates</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7bb50-114">AddDelegate</span><span class="sxs-lookup"><span data-stu-id="7bb50-114">AddDelegate</span></span>](https://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="7bb50-115">Удаление делегатов</span><span class="sxs-lookup"><span data-stu-id="7bb50-115">Remove delegates</span></span>  <br/> |[<span data-ttu-id="7bb50-116">ExchangeService. Ремоведелегатес</span><span class="sxs-lookup"><span data-stu-id="7bb50-116">ExchangeService.RemoveDelegates</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="7bb50-117">RemoveDelegate</span><span class="sxs-lookup"><span data-stu-id="7bb50-117">RemoveDelegate</span></span>](https://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="7bb50-118">После предоставления представителю разрешений на доступ к папке они могут работать над элементами в папке и во всех вложенных папках в соответствии с [разрешениями делегата](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span><span class="sxs-lookup"><span data-stu-id="7bb50-118">After a delegate is granted permissions to a folder, they can act on items in the folder and any subfolders, according to their [delegate permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms).</span></span> <span data-ttu-id="7bb50-119">Разрешения для делегатов применяются только к подпапкам, созданным после предоставления доступа представителя.</span><span class="sxs-lookup"><span data-stu-id="7bb50-119">Permissions for delegates only apply to subfolders that are created after the delegate access was granted.</span></span> <span data-ttu-id="7bb50-120">Чтобы обновить разрешения папки для уже существующих папок или других папок, ознакомьтесь с [разрешениями задание разрешений для папки для другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="7bb50-120">To update folder permissions for pre-existing folders, or other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
<span data-ttu-id="7bb50-121">Обратите внимание, что делегаты можно добавлять только к учетным записям с поддержкой почтовых ящиков, включая группы безопасности с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="7bb50-121">Note that delegates can only be added to mailbox-enabled accounts, including mail-enabled security groups.</span></span> <span data-ttu-id="7bb50-122">По умолчанию один вызов делегированного доступа EWS может получить доступ к не более чем 255 разных почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="7bb50-122">By default, a single EWS delegate access call can access a maximum of 255 different mailboxes.</span></span>

<span data-ttu-id="7bb50-123"><a name="bk_adddelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7bb50-123"><a name="bk_adddelegateewsma"> </a></span></span>

## <a name="add-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="7bb50-124">Добавление делегатов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="7bb50-124">Add delegates by using the EWS Managed API</span></span>

<span data-ttu-id="7bb50-125">Вы можете добавлять делегаты в почтовый ящик с помощью метода управляемого API [аддделегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="7bb50-125">You can add delegates to a mailbox by using the [AddDelegates](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="7bb50-126">В этом примере создается новый календарь, Контактное лицо и объект электронной почты [делегатеусер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) , и каждому представителю предоставляются [разрешения редактора](delegate-access-and-ews-in-exchange.md#bk_delegateperms) для соответствующей папки.</span><span class="sxs-lookup"><span data-stu-id="7bb50-126">In this example, a new calendar, contact, and email [DelegateUser](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) object is created, and each delegate is given [Editor permissions](delegate-access-and-ews-in-exchange.md#bk_delegateperms) for their respective folder.</span></span> <span data-ttu-id="7bb50-127">Вы можете изменить этот пример, чтобы добавить делегата в любую папку, указанную в [свойствах делегатепермиссионс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), а также задать разрешения для любого значения, указанного в перечислении [делегатефолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7bb50-127">You can modify the example to add a delegate to any of the folders specified by the [DelegatePermissions properties](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), and you can set the permissions to any of the values specified by the [DelegateFolderPermissionLevel](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) enumeration.</span></span> 
  
<span data-ttu-id="7bb50-128">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bb50-128">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="7bb50-129"><a name="bk_adddelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="7bb50-129"><a name="bk_adddelegateews"> </a></span></span>

## <a name="add-delegates-by-using-ews"></a><span data-ttu-id="7bb50-130">Добавление делегатов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="7bb50-130">Add delegates by using EWS</span></span>

<span data-ttu-id="7bb50-131">В приведенном ниже примере кода показано, как добавить отдельные делегаты календаря, контакта и электронной почты с помощью операции [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="7bb50-131">The following code example shows how to add separate calendar, contact, and email delegates by using the [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="7bb50-132">Почтовые ящики, которые требуется изменить, задаются элементом [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) , а параметры [разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms) для каждого делегата хранятся в элементе [делегатеусер](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="7bb50-132">The mailbox to modify is specified by the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element, and the [permission](delegate-access-and-ews-in-exchange.md#bk_delegateperms) settings for each delegate are contained in the [DelegateUser](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) element.</span></span> <span data-ttu-id="7bb50-133">Каждому представителю были предоставлены разрешения редактора для целевой папки.</span><span class="sxs-lookup"><span data-stu-id="7bb50-133">Each of the delegates has been granted Editor permissions to their target folder.</span></span> 
  
<span data-ttu-id="7bb50-134">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **аддделегатес** для [добавления делегатов](#bk_adddelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="7bb50-134">This is also the XML request that the EWS Managed API sends when you use the **AddDelegates** method to [add delegates](#bk_adddelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="7bb50-135">Сервер отвечает на запрос **AddDelegate** с сообщением [аддделегатереспонсе](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что делегаты успешно созданы.</span><span class="sxs-lookup"><span data-stu-id="7bb50-135">The server responds to the **AddDelegate** request with an [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully created.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="888"
                         MinorBuildNumber="9"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:AddDelegateResponse ResponseClass="Success"
                           xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="7bb50-136"><a name="bk_removedelegateewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="7bb50-136"><a name="bk_removedelegateewsma"> </a></span></span>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a><span data-ttu-id="7bb50-137">Удаление делегатов с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="7bb50-137">Remove delegates by using the EWS Managed API</span></span>

<span data-ttu-id="7bb50-138">Вы можете удалить делегатов из целевого почтового ящика с помощью метода [ExchangeService. ремоведелегатес](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API.</span><span class="sxs-lookup"><span data-stu-id="7bb50-138">You can remove delegates from a target mailbox by using the [ExchangeService.RemoveDelegates](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="7bb50-139">В этом примере удаляются разрешения делегатов, заданные в [примере Add a Delegate](#bk_adddelegateewsma) .</span><span class="sxs-lookup"><span data-stu-id="7bb50-139">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateewsma) are removed.</span></span> 
  
<span data-ttu-id="7bb50-140">В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь прошел проверку подлинности на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="7bb50-140">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the mailbox owner, and that the user has been authenticated to an Exchange server.</span></span> 
  
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

<span data-ttu-id="7bb50-141"><a name="bk_removedelegateews"> </a></span><span class="sxs-lookup"><span data-stu-id="7bb50-141"><a name="bk_removedelegateews"> </a></span></span>

## <a name="remove-delegates-by-using-ews"></a><span data-ttu-id="7bb50-142">Удаление делегатов с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="7bb50-142">Remove delegates by using EWS</span></span>

<span data-ttu-id="7bb50-143">Вы можете удалить делегатов из почтового ящика с помощью операции [RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="7bb50-143">You can remove delegates from a mailbox by using the [RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="7bb50-144">В этом примере удаляются разрешения делегатов, заданные в [примере Add a Delegate](#bk_adddelegateews) .</span><span class="sxs-lookup"><span data-stu-id="7bb50-144">In this example, the delegate permissions set in the [add a delegate example](#bk_adddelegateews) are removed.</span></span> 
  
<span data-ttu-id="7bb50-145">Это также запрос XML, который отправляет управляемый API EWS при использовании метода **ремоведелегатес** для [удаления делегатов](#bk_removedelegateewsma).</span><span class="sxs-lookup"><span data-stu-id="7bb50-145">This is also the XML request that the EWS Managed API sends when you use the **RemoveDelegates** method to [remove delegates](#bk_removedelegateewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="7bb50-146">Сервер отвечает на запрос **RemoveDelegate** с сообщением [аддделегатереспонсе](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что делегаты были успешно удалены.</span><span class="sxs-lookup"><span data-stu-id="7bb50-146">The server responds to the **RemoveDelegate** request with a [AddDelegateResponse](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the delegates were successfully removed.</span></span>

<span data-ttu-id="7bb50-147"><a name="bk_nextsteps"> </a></span><span class="sxs-lookup"><span data-stu-id="7bb50-147"><a name="bk_nextsteps"> </a></span></span>

## <a name="next-steps"></a><span data-ttu-id="7bb50-148">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="7bb50-148">Next steps</span></span>

<span data-ttu-id="7bb50-149">После добавления делегатов в папки "Календарь", "Электронная почта" и "задачи" представитель может получить доступ к элементам в папках.</span><span class="sxs-lookup"><span data-stu-id="7bb50-149">After you add delegates to calendar, email, and task folders, the delegate can access the items in the folders.</span></span> <span data-ttu-id="7bb50-150">Чтобы узнать больше, ознакомьтесь со следующими статьями:</span><span class="sxs-lookup"><span data-stu-id="7bb50-150">To learn more, see the following articles:</span></span>
  
- [<span data-ttu-id="7bb50-151">Доступ к электронной почте как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb50-151">Access email as a delegate by using EWS in Exchange</span></span>](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7bb50-152">Доступ к календарю как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb50-152">Access a calendar as a delegate by using EWS in Exchange</span></span>](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="7bb50-153">Доступ к контактам как представителю с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb50-153">Access contacts as a delegate by using EWS in Exchange</span></span>](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
<span data-ttu-id="7bb50-154">Если папки, для которых были добавлены представители, содержат дочерние папки, созданные до предоставления доступа представителю, то представитель не сможет получить доступ к этим папкам без дополнительных разрешений.</span><span class="sxs-lookup"><span data-stu-id="7bb50-154">If the folders for which you added delegates include child folders that were created before you granted the delegate access, the delegate will not be able to access those folders without additional permissions.</span></span> <span data-ttu-id="7bb50-155">Чтобы добавить эти разрешения или изменить разрешения для других папок, ознакомьтесь со статьей [Set Permissions Folders for другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="7bb50-155">To add these permissions, or modify permissions for any other folders, see [Set folder permissions for another user by using EWS in Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7bb50-156">См. также</span><span class="sxs-lookup"><span data-stu-id="7bb50-156">See also</span></span>

- [<span data-ttu-id="7bb50-157">Передача прав доступа и EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7bb50-157">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="7bb50-158">Exchange 2013: Программное добавление делегатов в учетную запись электронной почты</span><span class="sxs-lookup"><span data-stu-id="7bb50-158">Exchange 2013: Add delegate users to an email account programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [<span data-ttu-id="7bb50-159">Exchange 2013: программное обновление делегатов, связанных с учетными записями электронной почты</span><span class="sxs-lookup"><span data-stu-id="7bb50-159">Exchange 2013: Update delegates associated with email accounts programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [<span data-ttu-id="7bb50-160">Exchange 2013: Программное удаление делегатов, связанных с учетными записями электронной почты</span><span class="sxs-lookup"><span data-stu-id="7bb50-160">Exchange 2013: Remove delegates associated with email accounts programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

