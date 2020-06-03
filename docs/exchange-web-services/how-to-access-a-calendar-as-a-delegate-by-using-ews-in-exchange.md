---
title: Доступ к календарю как представителю с помощью EWS в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Узнайте, как получить доступ к календарю в качестве делегата с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 20ec294ddc4ccf014f0b2148c786c8c3ef8a6069
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528295"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>Доступ к календарю как представителю с помощью EWS в Exchange

Узнайте, как получить доступ к календарю в качестве делегата с помощью управляемого API EWS или EWS в Exchange.
  
С помощью управляемого API EWS или EWS вы можете предоставить представителю пользователя доступ к папке календаря владельца почтового ящика. После этого делегат может создавать приглашения на собрания от имени владельца почтового ящика, создавать встречи, отвечать на приглашения на собрания, а также получать, обновлять и удалять собрания из папки календаря владельца почтового ящика в зависимости от их разрешений.
  
Как представитель вы используете одни и те же методы и операции для доступа к папке календаря владельца почтового ящика, которая используется для доступа к собственной папке календаря. Основное отличие заключается в том, что вам необходимо использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создания папки календаря или папки календаря, а затем после определения идентификатора элемента или идентификатора папки можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновления или удаления элемента. 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для доступа к календарю в качестве делегата**

|**Задача**|**Используйте этот метод управляемого API EWS...**|**Используйте эту операцию EWS...**|
|:-----|:-----|:-----|
|Создание собрания или встречи в качестве представителя  <br/> |[Встреча. Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) , где параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Создание нескольких собраний или встреч в качестве делегата  <br/> |[ExchangeService. CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика.  <br/> |[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Поиск или Поиск встречи или собрания в качестве представителя  <br/> |[ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика.  <br/> |[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) определяет значение [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Получение встречи или собрания в качестве представителя  <br/> |[Встреча. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Обновление встречи или собрания в качестве представителя  <br/> |[Встреча. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которыми следует [встреча. обновление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление встречи или собрания в качестве делегата  <br/> |[Встреча. Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которыми следует [встреча. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> В примерах кода, приведенных в этой статье, primary@contoso.com является владельцем почтового ящика. 
  
## <a name="prerequisite-tasks"></a>Предварительные задачи
<a name="bk_prereq"> </a>

Прежде чем пользователь сможет получить доступ к папке календаря владельца почтового ящика в качестве представителя, пользователь должен быть [добавлен в качестве представителя с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) в папку календаря владельца почтового ящика. 
  
Представителю должен быть назначен почтовый ящик, подключенный к своей учетной записи, чтобы обновить календарь владельца почтового ящика.
  
Если представителю требуется работать только с приглашениями на собрания и ответами, вы можете добавить делегата в папку "Календарь" и использовать значение перечисления [митингрекуестсделиверископе. делегатесандсендинформатионтоме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) EWS управляемого API или значение **DelegatesAndSendInformationToMe** элемента [деливермитингрекуестс](https://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) EWS для отправки запросов представителю и информационным сообщениям владельцу почтового ящика. После этого делегату не требуется предоставлять доступ к папке "Входящие" владельца почтового ящика. 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Создание собрания или встречи в качестве делегата с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

Управляемый API EWS позволяет использовать объект Service для делегированного пользователя для создания элементов календаря для владельца почтового ящика. В этом примере показано, как использовать метод [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам. 
  
В этом примере предполагается, что **Служба** является допустимым объектом [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) для делегата, а представителю предоставлены соответствующие разрешения для папки календаря владельца почтового ящика. 
  
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

Обратите внимание, что при сохранении элемента вызов метода [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) должен определить папку календаря владельца почтового ящика. Если папка календарь владельца почтового ящика не указана, то запрос на собрание сохраняется в календаре представителя, а не в папке календаря владельца почтового ящика. Вы можете включить папку календаря владельца почтового ящика в вызов метода **Save** двумя способами. Мы рекомендуем создать экземпляр нового экземпляра объекта [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [веллкновнфолдернаме](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика. 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

Тем не менее, сначала можно [выполнить привязывание](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке календаря, а затем использовать идентификатор папки в вызове метода **Save** . Однако имейте в виду, что при этом создается дополнительный вызов EWS. 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Создание собрания или встречи в качестве делегата с помощью EWS
<a name="bk_createews"> </a>

Служба EWS позволяет использовать объект Service для делегированного пользователя, чтобы создавать элементы календаря для владельца почтового ящика. В этом примере показано, как использовать операцию [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания и отправки приглашений на собрание участникам. 
  
Это также запрос XML, который отправляет управляемый API EWS при использовании метода **Save** для [создания собрания или встречи в качестве делегата](#bk_createewsma).
  
Заголовок SOAP был удален из следующего примера для краткости.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
         xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
         xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

Сервер отвечает на запрос **CreateItem** с сообщением [креатеитемреспонсе](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает на то, что собрание было создано успешно. Ответ также содержит идентификатор вновь созданного собрания.
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Поиск собрания или встречи в качестве делегата с помощью управляемого API EWS
<a name="bk_searchewsma"> </a>

Чтобы найти собрание, необходимо использовать один из методов [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включающий параметр [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , чтобы можно было указать папку календаря владельца почтового ящика. 
  
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

После того как вызов **FindItems** возвратит ответ с идентификатором, вы можете получить, изменить или удалить это собрание с помощью идентификатора и [неявного доступа](delegate-access-and-ews-in-exchange.md#bk_implicit) , а также не указывать SMTP-адрес владельца почтового ящика. 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Поиск собрания или встречи в качестве делегата с помощью EWS
<a name="bk_searchews"> </a>

Служба EWS позволяет использовать объект Service для делегированного пользователя для поиска встреч и собраний, соответствующих набору критериев поиска. В этом примере показано, как использовать операцию [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) для поиска собраний в папке календаря владельца почтового ящика, содержащей слово "здание" в теме. 
  
Это также запрос XML, который отправляет управляемый API EWS при использовании метода **FindItem** для [поиска собрания или встречи в качестве делегата](#bk_searchewsma).
  
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

Сервер отвечает на запрос **FindItem** с сообщением [финдитемреспонсе](https://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) , которое содержит значение **ошибки**элемента [респонсекоде](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) , которое указывает, что поиск успешно завершен. Ответ содержит [календаритем](https://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для всех встреч или собраний, отвечающих условиям поиска. В этом случае найдено только одно собрание. 
  
Значение элемента [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) было сокращено для удобочитаемости. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

Теперь, когда у вас есть **идентификатор элемента для** собрания, который соответствует вашим условиям, вы можете получить, изменить или удалить это собрание с помощью элемента **ItemId** и [неявного доступа](delegate-access-and-ews-in-exchange.md#bk_implicit) , а также не указывать SMTP-адрес владельца почтового ящика. 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>Получение, обновление и удаление элементов календаря в качестве делегата с помощью управляемого API EWS
<a name="bk_geteswma"> </a>

С помощью управляемого API EWS можно получить, обновить или удалить собрание или встречу так же, как и при использовании делегированного доступа. Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя. Идентификатор элемента, включенный в вызов метода **BIND** , уникальным образом определяет элемент в хранилище почтовых ящиков в папке "Календарь" владельца почтового ящика. 
  
**Таблица 2. Методы управляемого API EWS для работы с встречами и собраниями в качестве делегата**

|**Задача**|**Метод управляемого API EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получение встречи или собрания  <br/> |[Базу](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Получение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Обновление встречи или собрания  <br/> |[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Обновление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Обновление собрания с помощью управляемого API EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|Удаление встречи или собрания  <br/> |[Привязка](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , за которой следует [Удаление](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Удаление собрания с помощью управляемого API EWS](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>Получение, обновление и удаление элементов календаря в качестве делегата с помощью EWS
<a name="bk_getews"> </a>

С помощью EWS можно получить, обновить или удалить собрание или встречу так же, как и при использовании делегированного доступа. Единственное отличие заключается в том, что объект службы предназначен для делегированного пользователя. Идентификатор элемента, включенный в вызов метода [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , однозначно определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика. 
  
**Таблица 3. Операции EWS для работы с встречами и собраниями в качестве делегата**

|**Task**|**Операция служб EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получение встречи или собрания  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Получение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Обновление встречи или собрания  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Обновление собрания с помощью EWS](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|Удаление встречи или собрания  <br/> |[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , за которым следует [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)   
- [Добавление и удаление делегатов с помощью EWS в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Задание разрешений для папки другого пользователя с помощью EWS в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    

