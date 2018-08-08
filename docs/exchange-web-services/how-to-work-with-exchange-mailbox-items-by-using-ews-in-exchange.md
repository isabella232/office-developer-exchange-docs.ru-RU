---
title: Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
ms.openlocfilehash: a40cd7ae682c1fb0a8d2f9cfcb10d99d4ab08052
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353968"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>Работа с элементами почтовых ящиков Exchange с помощью веб-служб Exchange

Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
  
Вы можете работать с элементами в почтовом ящике с помощью управляемого API EWS или веб-служб Exchange. Вы можете использовать универсальные [элементы — объекты ](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)или типы [элементов EWS ](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) для выполнения некоторых операций (получения или удаления элемента по его идентификатору). Однако для получения и обновления элементов чаще всего приходится использовать [строго типизированные элементы](folders-and-items-in-ews-in-exchange.md#bk_item), так как вам потребуется доступ к свойствам, относящимся к строго типизированному элементу. 

Например, с помощью универсального элемента невозможно получить элемент, содержащий даты начала и окончания — для этого потребуется объект управляемого API EWS [Appointment](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или тип [CalendarItem](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx). А если вы используете управляемый API EWS, то создавать строго типизированные элементы необходимо в любом случае, так как у класса универсального **элемента ** нет конструктора. Для работы с элементом, не являющимся строго типизированным, всегда можно использовать класс базового **элемента**. 
  
**Таблица 1. Методы управляемого API EWS и операции EWS для работы с элементами**

|**Задача**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Создание универсального элемента  <br/> |С помощью управляемого API EWS можно создавать только элементы определенных типов. Создавать универсальные элементы невозможно.  <br/> |[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Получение элемента  <br/> |[Item.Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|Обновление элемента  <br/> |[Item.Update](http://msdn.microsoft.com/ru-RU/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление элемента  <br/> |[Item.Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
Из этой статьи вы узнаете, когда для выполнения задачи можно использовать универсальный базовый класс, а в каких случаях необходимо применять строго типизированный элемент. В примерах кода показано, как использовать базовый класс и что делать, если использовать базовый класс невозможно или он не соответствует вашим потребностям.
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>Создание элемента с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

В управляемом API EWS нет общедоступного конструктора для класса [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx), поэтому потребуется использовать конструктор конкретного типа, который необходим для создания элемента. Например, с помощью [конструктора класса EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) можно создать новое сообщение электронной почты и с помощью [конструктора класса контактов Contact](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) можно создавать новые контакты. Аналогичным образом, сервер никогда не возвращает в ответах объекты универсального **элемента**. Все универсальные элементы возвращаются в виде объектов **EmailMessage**. 
  
Если вы знаете тип создаваемого элемента, выполнить задачу можно всего за несколько этапов. Действия одинаковы для всех типов элементов:
  
1. Инициализируйте новый экземпляр одного из классов [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) с объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в качестве параметра. 
    
2. Задайте свойства элемента. Для всех типов элементов используются разные схемы, поэтому для разных элементов доступны разные свойства.
    
3. Сохраните элемент или сохраните и отправьте его.
    
Например, вы можете создать объект [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекта, задавать свойства для [Subject](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [Body](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx) и [ToRecipients](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx), а затем отправлять его с помощью метода [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx). 
  
```cs
// Create an email message and provide it with connection 
// configuration information by using an ExchangeService object named service.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.Subject = "Company Soccer Team";
message.Body = "Are you interested in joining?";
message.ToRecipients.Add("sadie@contoso.com");
// Send the email message and save a copy.
// This method call results in a CreateItem call to EWS.
message.SendAndSaveCopy();
```

Сведения о том, как создать элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="create-an-item-by-using-ews"></a>Создание элемента с помощью веб-служб Exchange
<a name="bk_createews"> </a>

С помощью EWS можно создать универсальный или строго типизированный элемент. Действия одинаковы для всех типов элементов.
  
1. Создайте элемент в хранилище Exchange с помощью операции [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx). 
    
2. Используйте элемент [Items](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) в качестве контейнера для одного или нескольких создаваемых элементов. 
    
3. Задайте свойства элемента.
    
Например, вы можете создать электронное сообщение и отправить его с помощью кода из представленного ниже примера. Управляемое API EWS также отправляет запрос XML при вызове метода [SendAndSaveCopy](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx). 
  
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
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com </t:EmailAddress>
              </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

В ответ на запрос **CreateItem** сервер отправляет сообщение [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что сообщение было успешно создано, и свойство [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) созданного сообщения. 
  
Сведения о том, как создать собрание или встречу с помощью EWS, см. в статье[Create appointments and meetings by using EWS in Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>Получение элемента с помощью управляемого API EWS
<a name="bk_getewsma"> </a>

Чтобы использовать управляемое API EWS для получения элемента, если вы знаете свойство [Item.Id](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) получаемого элемента, необходимо просто вызвать один из методов [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) в элементе, после чего элемент будет получен. Рекомендуем возвращать только обязательные свойства. В этом примере возвращаются свойства **Id** элемента и **Subject**. 
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

Чтобы найти элемент, отвечающий определенным условиям, сделайте следующее:
  
1. Выполните привязку к папке, содержащей получаемые элементы.
    
2. Создайте экземпляр [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) или [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) для фильтрации элементов на возврат. 
    
3. Создайте экземпляр объекта [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx), чтобы указать количество элементов на возврат. 
    
4. Вызовите метод [ExchangeService.FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [ExchangeService.FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx). 
    
Например, чтобы получить непрочитанные электронные сообщения из папки "Входящие", используйте код из приведенного ниже примера. В этом примере используется **SearchFilterCollection** для ограничения результатов метода **FindItems** до непрочитанных сообщений, а с помощью объекта **ItemView** результаты можно сократить до одного элемента. Этот конкретный код работает только в объектах [EmailMessage](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекты, поскольку значение [EmailMessageSchema.IsRead](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) является частью **SearchFilter**. 
  
```cs
// Bind the Inbox folder to the service object.
Folder inbox = Folder.Bind(service, WellKnownFolderName.Inbox);
// The search filter to get unread email.
SearchFilter sf = new SearchFilter.SearchFilterCollection(LogicalOperator.And, new SearchFilter.IsEqualTo(EmailMessageSchema.IsRead, false));
ItemView view = new ItemView(1);
// Fire the query for the unread items.
// This method call results in a FindItem call to EWS.
FindItemsResults<Item> findResults = service.FindItems(WellKnownFolderName.Inbox, sf, view);
```

Кроме того, вы можете использовать [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) чтобы ограничить результаты поиска, как показано в приведенном ниже примере кода. В этом примере используется метод [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) для получения до пяти встреч, которые произойдут в течение следующих 30 дней. Конечно, этот код работает только с элементами календаря. 
  
```cs
// Initialize values for the start and end times, and the number of appointments to retrieve.
DateTime startDate = DateTime.Now;
DateTime endDate = startDate.AddDays(30);
const int NUM_APPTS = 5;
// Bind the Calendar folder to the service object.
// This method call results in a GetFolder call to EWS.
CalendarFolder calendar = CalendarFolder.Bind(service, WellKnownFolderName.Calendar, new PropertySet());
// Set the start and end time and number of appointments to retrieve.
CalendarView cView = new CalendarView(startDate, endDate, NUM_APPTS);
// Limit the properties returned to the appointment's subject, start time, and end time.
cView.PropertySet = new PropertySet(AppointmentSchema.Subject, AppointmentSchema.Start, AppointmentSchema.End);
// Retrieve a collection of appointments by using the calendar view.
// This method call results in a FindAppointments call to EWS.
FindItemsResults<Appointment> appointments = calendar.FindAppointments(cView);
```

Обратите внимание, что данные, возвращаемые сервером в ответ на вызов метода **Bind**, отличаются от аналогичных данных, возвращаемых сервером в ответ на методы **FindItem** или **FindAppointment**. Метод **Bind** может возвращать все схематизированные свойства, в то время как методы **FindItem** и **FindAppointment** возвращают не все из этих свойств. Следовательно, если вам нужен полный доступ к элементу, то необходимо использовать метод **Bind**. Если вам неизвестно значение свойства **Id** получаемого элемента, используйте методы **FindItem** или **FindAppointment**, чтобы получить свойство Id, а затем получите необходимые свойства с помощью метода **Bind**. 
  
Сведения о том, как получить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="get-an-item-by-using-ews"></a>Получение элемента с помощью EWS
<a name="bk_getews"> </a>

Если вам известно значение свойства [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) получаемого элемента, то вы можете получить его с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). 
  
В приведенном ниже примере показан XML-запрос на получение свойства [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) элемента с определенным значением свойства **ItemId**. Управляемое API EWS также отправляет запрос XML при вызове метода [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) на **ItemId**. Для удобства значения некоторых атрибутов и элементов были сокращены.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetItem>
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:ItemIds>
        <t:ItemId Id="GJc/NAAA=" />
      </m:ItemIds>
    </m:GetItem>
  </soap:Body>
</soap:Envelope>
```

В приведенном ниже примере показан XML-ответ, возвращаемый сервером после обработки операции **GetItem**. Ответ указывает, что элемент был успешно получен. Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="815" 
                         MinorBuildNumber="6" 
                         Version="V2_7" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:ItemId Id="GJc/NAAA=" ChangeKey="CQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAGJd9Z"/>
              <t:Subject>Company Soccer Team</t:Subject>
            </t:Message>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </m:GetItemResponse>
  </s:Body>
</s:Envelope>
```

Если вы не знаете значение свойства **ItemId** получаемого элемента, его можно найти с помощью операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx). Для использования операции **FindItem** необходимо сначала определить папку для поиска. Это можно сделать с помощью свойства **DistinguinguishedFolderName** или [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). Можно использовать операцию [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) или [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx), чтобы получить нужное свойство **FolderId**. Затем с помощью операции **FindItem** найдите в папке результаты, соответствующие фильтру поиска. В отличие от управляемого API EWS, в веб-службах Exchange нет отдельной операции поиска для встреч. Операция **FindItem** получает элементы всех типов. 
  
В приведенном ниже примере показан XML-запрос с операцией **FindItem**, отправляемый на сервер для поиска в папке Calendar встреч, назначенных на следующие 30 дней. Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
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
          <t:FieldURI FieldURI="calendar:Start" />
          <t:FieldURI FieldURI="calendar:End" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:CalendarView MaxEntriesReturned="5" StartDate="2013-10-16T17:04:28.722Z" EndDate="2013-11-15T18:04:28.722Z" />
      <m:ParentFolderIds>
        <t:FolderId Id="AAAEOAAA=" ChangeKey="AgAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAAAA3" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

В ответ на запрос **FindItem** сервер возвращает сообщение [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) со значением **NoError**, которое указывает, что операция успешно выполнена. Если какие-либо элементы календаря отвечают условиям фильтра, они включаются в ответ.
  
Обратите внимание, что данные, возвращаемые сервером в ответ на вызов операции **GetItem**, отличаются от аналогичных данных для операций **FindItem** или **FindAppointment**. Операция **GetItem** может возвращать все схематизированные свойства, в то время как операции **FindItem** и **FindAppointment** возвращают не все из этих свойств. Следовательно, если вам нужен полный доступ к элементу, то необходимо использовать операцию **GetItem**. Если вам неизвестно значение свойства **ItemId** получаемого элемента, используйте операции **FindItem** или **FindAppointment**, чтобы получить свойство **ItemId**, а затем получите необходимые элементы с помощью операции **GetItem**. 
  
Сведения о том, как получить элемент собрания или встречи с помощью EWS, см. в статье [Get appointments and meetings by using EWS in Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>Изменение элемента с помощью управляемого API EWS
<a name="bk_updateewsma"> </a>

Действия для изменения элемента с помощью управляемого API EWS одинаковы для всех типов элементов. Однако элементы разных типов содержат разные свойства, а для метода [Update](http://msdn.microsoft.com/ru-RU/library/office/dd635915%28v=exchg.80%29.aspx) доступно множество перегруженных методов. Чтобы обновить элемент, сделайте следующее: 
  
1. Получите последнюю версию элемента (если ее у вас еще нет) с помощью метода [Bind](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx). Чтобы редактировать свойства, относящиеся к строго типизированному элементу, необходимо выполнить привязку к типу этого элемента. Чтобы изменить свойства, доступные для типа универсальный элемента, вы можете выполнить привязку к объекту [элемента](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx). 
    
2. Обновите свойства элемента.
    
3. Вызовите метод **Update**. 
    
Например, вы можете изменить тему сообщения с помощью универсального типа элемента, как показано в коде приведенного ниже примера.
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Update the Subject of the email.
item.Subject = "New subject";
// Save the updated email.
// This method call results in an UpdateItem call to EWS.
item.Update(ConflictResolutionMode.AlwaysOverwrite);
```

Сведения о том, как обновить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-ews"></a>Обновление элемента с помощью EWS
<a name="bk_updateews"> </a>

Чтобы обновить элемент с помощью EWS, сделайте следующее:
  
1. Получите последнюю версию элемента (если ее у вас еще нет) с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx). 
    
2. Укажите редактируемые поля и присвойте им новые значения с помощью операции [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx). 
    
В приведенном ниже примере показан XML-запрос с операцией **UpdateItem**, который отправляется на сервер для изменения свойства [Subject](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) электронного сообщения. Для удобства значения некоторых атрибутов и элементов были сокращены. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateItem MessageDisposition="SaveOnly" ConflictResolution="AlwaysOverwrite">
      <m:ItemChanges>
        <t:ItemChange>
          <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAAAPdgr" />
          <t:Updates>
            <t:SetItemField>
              <t:FieldURI FieldURI="item:Subject" />
              <t:Message>
                <t:Subject>New subject</t:Subject>
              </t:Message>
            </t:SetItemField>
          </t:Updates>
        </t:ItemChange>
      </m:ItemChanges>
    </m:UpdateItem>
  </soap:Body>
</soap:Envelope>
```

В ответ на запрос **UpdateItem** сервер отправляет сообщение [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что элемент успешно обновлен.
  
Сведения о том, как изменить элемент собрания или встречи с помощью веб-служб Exchange, см. в статье [Update appointments and meetings by using EWS in Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>Удаление элемента с помощью управляемого API EWS
<a name="bk_deleteewsma"> </a>

Вы можете удалять элементы, перемещая их в папку "Удаленные" или в корзину. Если вы знаете [ItemId](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) удаляемого элемента, то просто вызовите метод [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx) в элементе. 
  
Если перед удалением элемента необходимо его найти, сделайте следующее:
  
1. Вызовите метод [FindItems](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [FindAppointments](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx), чтобы найти удаляемый элемент. 
    
1. Создайте экземпляр [PropertySet](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и ограничьте его до свойств для возврата или используйте [SearchFilterCollection](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) для поиска определенных элементов. 
    
2. Создайте экземпляр [ItemView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [CalendarView](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx), чтобы указать количество элементов на возврат. 
    
2. Вызовите метод [Delete](http://msdn.microsoft.com/ru-RU/library/office/dd635072%28v=exchg.80%29.aspx). 
    
Например, в представленном ниже коде показано, как переместить электронное сообщение в папку "Удаленные".
  
В этом примере предполагается, что **служба** является действительным объектом [ExchangeService](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx), и что пользователь прошел проверку подлинности на сервере Exchange server. Локальная переменная *itemId* является [идентификатором](http://msdn.microsoft.com/ru-RU/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) обновляемого элемента. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

Дополнительные сведения об удалении элементов см. в статье [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md). Сведения о том, как удалить элемент собрания или встречи с помощью управляемого API EWS, см. в статье [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-ews"></a>Удаление элемента с помощью EWS
<a name="bk_deleteews"> </a>

Вы можете удалить элемент с помощью операции [DeleteItem](../web-service-reference/deleteitem-operation.md). 
  
В приведенном ниже примере кода показан XML-запрос, отправляемый на сервер для перемещения электронного сообщения в папку "Удаленные". Для удобства значения некоторых атрибутов и элементов были сокращены.
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems">
      <m:ItemIds>
        <t:ItemId Id="APdZjAAA=" ChangeKey="CQAAABYAAAAqRr3mNdNMSasqx/o9J13UAAANIFzC" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>
```

В ответ на запрос **DeleteItem** сервер отправляет сообщение [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx), включающее параметр [ResponseCode](http://msdn.microsoft.com/ru-RU/library/aa580757%28v=exchg.150%29.aspx) со значением **NoError**, которое указывает, что элемент успешно удален.
  
Дополнительные сведения об удалении элементов см. в статье [Deleting items by using EWS in Exchange](deleting-items-by-using-ews-in-exchange.md). Сведения о том, как удалить элемент собрания или встречи с помощью EWS, см. в статье [Delete appointments and cancel meetings by using EWS in Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="move-or-copy-items-to-another-mailbox"></a>Перемещение или копирование элементов в другой почтовый ящик
<a name="bk_movecopybtnmailboxes"> </a>

Вы можете перемещать и копировать элементы между почтовыми ящиками с помощью операций [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) и [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx). Дополнительные сведения см. в статье [Exporting and importing items by using EWS in Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Работа с папками с помощью EWS в Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Удаление элементов с помощью EWS в Exchange](deleting-items-by-using-ews-in-exchange.md)
    

