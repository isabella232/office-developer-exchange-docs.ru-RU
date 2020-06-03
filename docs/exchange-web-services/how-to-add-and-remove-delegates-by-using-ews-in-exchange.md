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
# <a name="add-and-remove-delegates-by-using-ews-in-exchange"></a>Добавление и удаление делегатов с помощью EWS в Exchange

Узнайте, как добавлять делегаты или удалять делегаты из почтовых ящиков пользователей с помощью управляемого API EWS или EWS в Exchange.
  
Вы можете использовать управляемый API EWS или EWS, чтобы позволить представителям действовать от имени владельца почтового ящика или удалять доступ представителя к почтовому ящику. Пользователи, добавленные в качестве представителей и обладающие разрешениями, могут выполнять задачи от имени владельца почтового ящика. Например, они могут создавать и отправлять приглашения на собрания, отправлять сообщения электронной почты и отвечать на приглашения на собрания от имени владельца почтового ящика. 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для добавления и удаления делегатов**

|**Задача**|**Метод управляемого API EWS**|**Операция EWS**|
|:-----|:-----|:-----|
|Добавление делегатов  <br/> |[ExchangeService. Аддделегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) <br/> |[AddDelegate](https://msdn.microsoft.com/library/646fb994-229e-4d90-8b95-6541191cb3ae%28Office.15%29.aspx) <br/> |
|Удаление делегатов  <br/> |[ExchangeService. Ремоведелегатес](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) <br/> |[RemoveDelegate](https://msdn.microsoft.com/library/f21c5171-62e7-47c8-99b1-22e1ff5883bb%28Office.15%29.aspx) <br/> |
   
После предоставления представителю разрешений на доступ к папке они могут работать над элементами в папке и во всех вложенных папках в соответствии с [разрешениями делегата](delegate-access-and-ews-in-exchange.md#bk_delegateperms). Разрешения для делегатов применяются только к подпапкам, созданным после предоставления доступа представителя. Чтобы обновить разрешения папки для уже существующих папок или других папок, ознакомьтесь с [разрешениями задание разрешений для папки для другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
Обратите внимание, что делегаты можно добавлять только к учетным записям с поддержкой почтовых ящиков, включая группы безопасности с включенной поддержкой почты. По умолчанию один вызов делегированного доступа EWS может получить доступ к не более чем 255 разных почтовых ящиков.

<a name="bk_adddelegateewsma"> </a>

## <a name="add-delegates-by-using-the-ews-managed-api"></a>Добавление делегатов с помощью управляемого API EWS

Вы можете добавлять делегаты в почтовый ящик с помощью метода управляемого API [аддделегатес](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.adddelegates%28v=exchg.80%29.aspx) EWS. В этом примере создается новый календарь, Контактное лицо и объект электронной почты [делегатеусер](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegateuser%28v=exchg.80%29.aspx) , и каждому представителю предоставляются [разрешения редактора](delegate-access-and-ews-in-exchange.md#bk_delegateperms) для соответствующей папки. Вы можете изменить этот пример, чтобы добавить делегата в любую папку, указанную в [свойствах делегатепермиссионс](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatepermissions_properties%28v=exchg.80%29.aspx), а также задать разрешения для любого значения, указанного в перечислении [делегатефолдерпермиссионлевел](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.delegatefolderpermissionlevel%28v=exchg.80%29.aspx) . 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь прошел проверку подлинности на сервере Exchange. 
  
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

<a name="bk_adddelegateews"> </a>

## <a name="add-delegates-by-using-ews"></a>Добавление делегатов с помощью EWS

В приведенном ниже примере кода показано, как добавить отдельные делегаты календаря, контакта и электронной почты с помощью операции [AddDelegate](https://msdn.microsoft.com/library/012d8cc5-648c-4ba0-a155-15c422b1e994%28Office.15%29.aspx) EWS. Почтовые ящики, которые требуется изменить, задаются элементом [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) , а параметры [разрешений](delegate-access-and-ews-in-exchange.md#bk_delegateperms) для каждого делегата хранятся в элементе [делегатеусер](https://msdn.microsoft.com/library/aac4e74e-f69b-4c41-a0c9-489610330fbf%28Office.15%29.aspx) . Каждому представителю были предоставлены разрешения редактора для целевой папки. 
  
Это также запрос XML, который отправляет управляемый API EWS при использовании метода **аддделегатес** для [добавления делегатов](#bk_adddelegateewsma).
  
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

Сервер отвечает на запрос **AddDelegate** с сообщением [аддделегатереспонсе](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что делегаты успешно созданы.
  
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

<a name="bk_removedelegateewsma"> </a>

## <a name="remove-delegates-by-using-the-ews-managed-api"></a>Удаление делегатов с помощью управляемого API EWS

Вы можете удалить делегатов из целевого почтового ящика с помощью метода [ExchangeService. ремоведелегатес](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.removedelegates%28v=exchg.80%29.aspx) EWS Managed API. В этом примере удаляются разрешения делегатов, заданные в [примере Add a Delegate](#bk_adddelegateewsma) . 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для владельца почтового ящика и что пользователь прошел проверку подлинности на сервере Exchange. 
  
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

<a name="bk_removedelegateews"> </a>

## <a name="remove-delegates-by-using-ews"></a>Удаление делегатов с помощью EWS

Вы можете удалить делегатов из почтового ящика с помощью операции [RemoveDelegate](https://msdn.microsoft.com/library/1d42d5ff-8fde-4f8a-b18d-57b1ef7a946a%28Office.15%29.aspx) EWS. В этом примере удаляются разрешения делегатов, заданные в [примере Add a Delegate](#bk_adddelegateews) . 
  
Это также запрос XML, который отправляет управляемый API EWS при использовании метода **ремоведелегатес** для [удаления делегатов](#bk_removedelegateewsma).
  
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

Сервер отвечает на запрос **RemoveDelegate** с сообщением [аддделегатереспонсе](https://msdn.microsoft.com/library/d7e6bebb-5dbf-43c1-aacf-4b3ca6a7c429%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что делегаты были успешно удалены.

<a name="bk_nextsteps"> </a>

## <a name="next-steps"></a>Дальнейшие действия

После добавления делегатов в папки "Календарь", "Электронная почта" и "задачи" представитель может получить доступ к элементам в папках. Чтобы узнать больше, ознакомьтесь со следующими статьями:
  
- [Доступ к электронной почте как представителю с помощью EWS в Exchange](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к календарю как представителю с помощью EWS в Exchange](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Доступ к контактам как представителю с помощью EWS в Exchange](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
Если папки, для которых были добавлены представители, содержат дочерние папки, созданные до предоставления доступа представителю, то представитель не сможет получить доступ к этим папкам без дополнительных разрешений. Чтобы добавить эти разрешения или изменить разрешения для других папок, ознакомьтесь со статьей [Set Permissions Folders for другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)
- [Exchange 2013: Программное добавление делегатов в учетную запись электронной почты](https://code.msdn.microsoft.com/exchange/Exchange-2013-Adding-1024511f)   
- [Exchange 2013: программное обновление делегатов, связанных с учетными записями электронной почты](https://code.msdn.microsoft.com/exchange/Exchange-2013-Update-b40d3bac)   
- [Exchange 2013: Программное удаление делегатов, связанных с учетными записями электронной почты](https://code.msdn.microsoft.com/exchange/Exchange-2013-Remove-686f7714)
    

