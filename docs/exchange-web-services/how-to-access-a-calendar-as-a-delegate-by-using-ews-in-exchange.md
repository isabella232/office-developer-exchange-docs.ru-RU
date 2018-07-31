---
title: Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: d7db4a1e-9ed6-41da-8529-a73ca285cdf2
description: Узнайте, как получить доступ к роли представителя календаря с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: 609e5f0bb22c78174289a2eb10210999c8391a3d
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353842"
---
#  <a name="access-a-calendar-as-a-delegate-by-using-ews-in-exchange"></a>Доступ к календарю в качестве делегата с помощью веб-служб Exchange в Exchange

Узнайте, как получить доступ к роли представителя календаря с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Можно использовать управляемый API EWS или делегирование EWS, чтобы предоставить пользователю доступ к папке календаря владельца почтового ящика. Делегат можно затем Создание приглашений на собрания от имени владельца почтового ящика, Создание встречи, ответ на приглашения на собрания и извлечь, обновление и удаление собрания из папки календаря владельца почтового ящика, в зависимости от их разрешения.
  
Роли представителя используйте ту же методов и операций на доступ к папке календаря владельца почтового ящика, которая используется для доступа к папке календаря. Основное различие —, что вам следует использовать [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicit) для поиска или создание элемента календаря или вложенной папке календаря и затем после определения идентификатор элемента или идентификатор папки можно использовать [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) для получения, обновить или удалить элемент. 
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для доступа к календарю роли представителя**

|**Задача**|**Используйте этот метод управляемый API EWS...**|**Используйте эту операцию EWS...**|
|:-----|:-----|:-----|
|Создание собрания или встречи в качестве делегата  <br/> |[Appointment.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) , где параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Создание нескольких собрания или встречи в качестве делегата  <br/> |[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика  <br/> |[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Поиск или поиск встречи или собрания в качестве делегата  <br/> |[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , где параметр **FolderId** предоставляет [явный доступ](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) к папке календаря владельца почтового ящика  <br/> |[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , где элемент [почтового ящика](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) указывает [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) владельца почтового ящика  <br/> |
|Получение встречи или собрания в качестве делегата  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|Обновление встречи или собрания в качестве делегата  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Appointment.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление встречи или собрания в качестве делегата  <br/> |[Appointment.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
> [!NOTE]
> В примерах кода в этой статье primary@contoso.com — это владелец почтового ящика. 
  
## <a name="prerequisite-tasks"></a>Обязательные задачи
<a name="bk_prereq"> </a>

Пользователь может получить доступ к папки календаря владельца почтового ящика в качестве делегата, пользователь должен быть [добавлен в качестве делегата с разрешениями](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) для папки календаря владельца почтового ящика. 
  
Делегат должен иметь почтового ящика, подключенного к своей учетной записи для обновления календаря владельца почтового ящика.
  
Если представителю требуется для работы с приглашений на собрания и ответы, можно добавить делегата к папке календаря и используйте значение перечисления управляемый API EWS [MeetingRequestsDeliveryScope.DelegatesAndSendInformationToMe](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.meetingrequestsdeliveryscope%28v=exchg.80%29.aspx) по умолчанию или [ DeliverMeetingRequests](http://msdn.microsoft.com/library/04b999af-0b27-4e6d-a8b1-400955a1afaa%28Office.15%29.aspx) веб-служб Exchange имеет значение **DelegatesAndSendInformationToMe** для отправки запросов к делегат и информационные сообщения владельцу почтового ящика. Делегат затем не требуется предоставить доступ к папке "Входящие" владельца почтового ящика. 
  
## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Создание собрания или встречи в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_createewsma"> </a>

Управляемый API EWS позволяет использовать объект службы для пользователя делегат для создания элементов календаря для владельца почтового ящика. В этом примере показано, как использовать метод [сохранения](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) для создания собрания и отправки приглашений на собрание участникам. 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) делегата и делегата предоставлены необходимые разрешения для папки календаря владельца почтового ящика. 
  
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

Обратите внимание, что при сохранении элемента вызова метода [Сохранить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) необходимо определить папки календаря владельца почтового ящика. Если папки календаря владельца почтового ящика не указан, запрос на собрание получает сохранены делегата календаря и не папки календаря владельца почтового ящика. Может включать папки календаря владельца почтового ящика в вызове метода **Сохранить** двумя способами. Рекомендуется создать новый экземпляр объекта [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) с помощью [WellKnownFolderName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) и SMTP-адреса владельца почтового ящика. 
  
```cs
meeting.Save(new FolderId(WellKnownFolderName.Calendar,
    "primary@contoso.com"), SendInvitationsMode.SendToAllAndSaveCopy);
```

Тем не менее, можно также [привязать](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) к папке календаря во-первых и затем используйте идентификатор папки в вызове метода **сохранения** . Однако следует помнить, что при этом создается дополнительных вызовов веб-служб Exchange. 
  
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

## <a name="create-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Создание собрания или встречи в качестве делегата с помощью веб-служб Exchange
<a name="bk_createews"> </a>

Веб-служб Exchange позволяет использовать объект службы для пользователя делегат для создания элементов календаря для владельца почтового ящика. В этом примере показано, как использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для создания собрания и отправки приглашений на собрание участникам. 
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **Save** для [создания собрания или встречи в качестве делегата](#bk_createewsma).
  
В следующем примере для краткости был удален заголовка SOAP.
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, это означает, что собрания был успешно создан. Ответ также содержит идентификатор элемента для только что созданный собрания.
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-the-ews-managed-api"></a>Поиск собрания или встречи в качестве делегата с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_searchewsma"> </a>

Для поиска собрания, необходимо использовать один из методов [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , включает параметр [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) , таким образом, можно указать папку календаря владельца почтового ящика. 
  
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

После вызова **FindItems** возвращает ответ с кодом, можно получить, обновлении или удалении этого собрания с помощью идентификатора и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) , и необходимо указать SMTP-адреса владельца почтового ящика. 
  
## <a name="search-for-a-meeting-or-appointment-as-a-delegate-by-using-ews"></a>Поиск собрания или встречи в качестве делегата с помощью веб-служб Exchange
<a name="bk_searchews"> </a>

Веб-служб Exchange позволяет использовать объект службы для делегата поиск встречи и собрания, которые соответствуют заданным условиям поиска. В этом примере показано, как использовать операцию [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) найти собраний в папке календаря владельца почтового ящика, содержащие слово «создание» в теме сообщения. 
  
Это также XML-запрос, который отправляет управляемый API EWS при использовании метода **FindItem** для [поиска для собрания или встречи в качестве делегата](#bk_searchewsma).
  
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

Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, которое содержит значение элемента [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что поиск успешно завершена. Ответ содержит [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) для встречи или собрания, выполнены условия поиска. В этом случае найти только одного собрания. 
  
Значение элемента [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) был усечен для удобства чтения. 
  
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

Теперь, когда у вас есть **ItemId** собрания, который соответствует условиям, можно получить, обновлении или удалении этого собрания с помощью **ItemId** и [неявный доступ](delegate-access-and-ews-in-exchange.md#bk_implicit) , и необходимо указать SMTP-адреса владельца почтового ящика. 
  
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-the-ews-managed-api"></a>Получение, обновление и удаление элементов календаря роли представителя с помощью управляемого интерфейса API веб-служб Exchange
<a name="bk_geteswma"> </a>

Можно использовать управляемый API EWS для получения, обновить или удалить собрание или встречу так же, как выполнять эти действия, если вы не используете делегированный доступ. Единственное отличие — объект службы для делегата. Идентификатор элемента, включенные в вызове метода **Привязка** уникальным образом определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика. 
  
**В таблице 2. Управляемый API EWS методы для работы с встречи и собрания роли представителя**

|**Задача**|**Метод управляемого API EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получение встречи или собрания  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[Получение элемента с помощью управляемого API EWS](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|Обновление встречи или собрания  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) следуют [обновления](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx) <br/> |[Обновление собрания с помощью управляемого интерфейса API веб-служб Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWSMA) <br/> |
|Удаление встречи или собрания  <br/> |[Привязка](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) , а затем [Удалить](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[Удаление собрания с помощью управляемого интерфейса API веб-служб Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="get-update-or-delete-calendar-items-as-a-delegate-by-using-ews"></a>Получение, обновление и удаление элементов календаря роли представителя с помощью веб-служб Exchange
<a name="bk_getews"> </a>

Чтобы получить, обновить или удалить собрания или встречи так же, как выполнять эти действия, если вы не используете делегированный доступ, можно использовать веб-служб Exchange. Единственное отличие — объект службы для делегата. Идентификатор элемента, включенные в вызове метода [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) уникальным образом определяет элемент в хранилище почтовых ящиков в папке календаря владельца почтового ящика. 
  
**В таблице 3. Операции EWS для работы с встречи и собрания в качестве делегата**

|**Задача**|**Операция служб EWS**|**Пример кода**|
|:-----|:-----|:-----|
|Получение встречи или собрания  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[Получение элемента с помощью веб-служб Exchange](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|Обновление встречи или собрания  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |[Обновление собрания с помощью веб-служб Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md#bk_UpdateMtgEWS) <br/> |
|Удаление встречи или собрания  <br/> |[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) , а затем [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |[](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md#bk_DeleteMtgEWSMA) <br/> |
   
## <a name="see-also"></a>См. также

- [Передача прав доступа и EWS в Exchange](delegate-access-and-ews-in-exchange.md)   
- [Добавление и удаление делегаты с помощью веб-служб Exchange в Exchange](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [Настройка разрешений папки другого пользователя с помощью веб-служб Exchange в Exchange](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md) 
- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)
    

