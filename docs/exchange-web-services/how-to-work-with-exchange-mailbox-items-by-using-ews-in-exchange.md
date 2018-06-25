---
title: Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 721deb84-f85d-45d0-84c1-0ed55f359969
description: Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
ms.openlocfilehash: e70ac499da57faa60b4bcb6082648b23d1a7e791
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761140"
---
# <a name="work-with-exchange-mailbox-items-by-using-ews-in-exchange"></a>Работа с элементами почтового ящика Exchange с помощью веб-служб Exchange в Exchange

Узнайте, как создавать, получать, редактировать и удалять элементы с помощью управляемого API EWS или служб EWS в Exchange.
  
Для работы с элементами в почтовом ящике, можно использовать управляемый API EWS или веб-служб Exchange. Можно использовать универсальный элементов — управляемый API EWS [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) объектов или типов веб-служб Exchange [элемента](http://msdn.microsoft.com/library/4dfe8f48-e7b4-444d-bdf9-a34e180f598b%28Office.15%29.aspx) — для выполнения некоторых операций (начало элемента или удаление элемента с помощью идентификатора элемента); Тем не менее в большинстве случаев, необходимо будет использовать [строго типизированных элемента](folders-and-items-in-ews-in-exchange.md#bk_item) для get и операцию обновления, поскольку он потребуется доступ к свойствам, которые относятся к строго типизированный элемент. 

Например универсальный элемент нельзя использовать для получения элемента, который содержит начать и Дата окончания — нужно объект управляемый API EWS [встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/b0c1fd27-b6da-46e5-88b8-88f00c71ba80%28Office.15%29.aspx) тип для этого. И, если вы используете управляемый API веб-служб Exchange, всегда необходимо создать строго типизированные элементы, поскольку универсальный класс **элемента** не имеет конструктора. При работе с элементом, который не является строго типизированным, всегда можно использовать базовый класс **элемента** для работы с элементом. 
  
**В таблице 1. Управляемый API EWS методы и операций веб-служб Exchange для работы с элементами**

|**Чтобы...**|**Метод управляемого API EWS**|**Операция служб EWS**|
|:-----|:-----|:-----|
|Создание универсального элемента  <br/> |Нет. С помощью управляемого API EWS можно создавать только элементы определенных типов. Создавать универсальные элементы невозможно.  <br/> |[CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> |
|Получение элемента  <br/> |[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> |
|Изменение элемента  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|Удаление элемента  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
В этой статье вы узнаете, при использовании универсального базового класса и когда следует использовать строго типизированный элемент выполнение задачи. В примере кода показано использование базового класса и что делать при базового класса или он не соответствии со своими потребностями.
  
## <a name="create-an-item-by-using-the-ews-managed-api"></a>Создание элемента с помощью управляемого API EWS
<a name="bk_createewsma"> </a>

Управляемый API EWS не имеет общедоступным конструктора для класса [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) , необходимо использовать конструктор для типа определенного элемента, который требуется создать, чтобы создать элемент. Например используйте [конструктор класса EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx) для создания нового сообщения электронной почты и [контактов конструктор класса](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contact%28v=exchg.80%29.aspx) для создания нового контакта. Аналогичным образом сервер никогда не возвращает универсальный объекты **элементов** в ответы; все элементы универсальный возвращаются в виде объектов **EmailMessage** . 
  
Если вы знаете тип создаваемого элемента, выполнить задачу можно всего за несколько этапов. Действия одинаковы для всех типов элементов:
  
1. Инициализация нового экземпляра одного из классов [элемента](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) с помощью объекта [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) как параметр. 
    
2. Задайте свойства элемента. Для всех типов элементов используются разные схемы, поэтому для разных элементов доступны разные свойства.
    
3. Сохраните элемент или сохраните и отправьте его.
    
К примеру можно создать объект [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) , Настройка параметров [Тема](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.subject%28v=exchg.80%29.aspx), [текст](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.body%28v=exchg.80%29.aspx)и [ToRecipients](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.torecipients%28v=exchg.80%29.aspx) и отправить его с помощью метода [EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) . 
  
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

Чтобы научиться создавать собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="create-an-item-by-using-ews"></a>Создание элемента с помощью веб-служб Exchange
<a name="bk_createews"> </a>

С помощью веб-служб Exchange можно создать универсальный или строго типизированный элемент. Действия одинаковы для всех типов элементов:
  
1. С помощью операции [CreateItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) для создания элемента в хранилище Exchange. 
    
2. Используйте элемент [элементов](http://msdn.microsoft.com/library/0811a73e-bf1f-4889-9219-73902dd47639%28Office.15%29.aspx) содержит один или несколько элементов для создания. 
    
3. Задайте свойства элемента.
    
Например можно создавать сообщения электронной почты и отправьте его с помощью кода в следующем примере. Это также запроса XML, то при вызове метода [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) отправляет управляемый API веб-служб Exchange. 
  
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

Сервер отвечает на запрос **CreateItem** [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что сообщение электронной почты был успешно создан, и [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) из вновь сообщение о создании. 
  
Чтобы научиться создавать собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md).
  
## <a name="get-an-item-by-using-the-ews-managed-api"></a>Получение элемента с помощью управляемого API EWS
<a name="bk_getewsma"> </a>

Чтобы использовать управляемый API EWS для получения элемента, если вы знаете [элемент.идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для извлечения, можно просто вызвать один из методов [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для элемента, а элемент извлекается. Рекомендуется рекомендуется ограничить возвращаемые только теми надстройками, которые необходимы свойства. В этом примере возвращаются свойства **Id** элемента и свойство **Subject** . 
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления. 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, ItemSchema.Subject);
// Bind to the existing item by using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId, propSet);

```

Если вы ищете элемента, который соответствует определенному набору условий, выполните следующее:
  
1. Выполните привязку к папке, содержащей получаемые элементы.
    
2. Создайте экземпляр [SearchFilter.SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) или [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) для фильтрации элементов для возврата. 
    
3. Создайте экземпляр объекта [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) для определения количества элементов для возврата. 
    
4. Вызовите метод [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [ExchangeService.FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) . 
    
Например если вы хотите получать сообщения непрочитанные сообщения электронной почты в папке "Входящие", используйте код в следующем примере. В этом примере использует **SearchFilterCollection** для ограничения результатов метод **FindItems** , непрочитанных сообщений и ограничения для **ItemView** , чтобы ограничить результаты одного элемента. Этот код конкретного работает только с [EmailMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) объекты [EmailMessageSchema.IsRead](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema.isread%28v=exchg.80%29.aspx) значение является частью **SearchFilter**. 
  
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

Кроме того можно использовать [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) , чтобы ограничить результаты поиска, как показано в следующем примере кода. В этом примере используется метод [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) для получения до пяти встреч, которые происходят в течение 30 дней. Этот код безусловно работает только с элементами календаря. 
  
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

Обратите внимание, что в ответ **привязать** метод возвращает сведения о сервере, отличается от сведений, сервер возвращает метод отклика **FindItem** или **FindAppointment** . Метод **Bind** можно вернуть Схематизированный свойства, тогда как методы **FindItem** и **FindAppointment** не возвращают Схематизированный свойства. Поэтому если вам требуется полный доступ к элементу, вам придется использовать метод **привязки** . Если у элемента нет **идентификатор** элемента, вы хотите получать, использовать методы **FindItem** или **FindAppointment** для получения идентификатора и затем использовать метод **привязки** для извлечения свойств, необходимую. 
  
Чтобы узнать, как получить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="get-an-item-by-using-ews"></a>Получение элемента с помощью веб-служб Exchange
<a name="bk_getews"> </a>

Если вы знаете [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) элемента для извлечения, вы получаете элемента с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) . 
  
В следующем примере показано XML-запрос, чтобы получить [тему](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) элемента с определенным **ItemId**. Это также запроса XML, управляемый API EWS отправляет при вызове метода [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) на **идентификатор элемента**. Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы.
  
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

В следующем примере показано XML-ответ, что сервер возвращает после обработки операции **GetItem** . Ответ указывает, что элемент был успешно извлечен. Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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

Если вы не знаете **ItemId** элемента, которую необходимо получить, можно с помощью операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) поиск элемента. Чтобы использовать операции **FindItem** , необходимо сначала определить к папке, где выполняется поиск. Можно определить папку с помощью его **DistinguinguishedFolderName** или с помощью [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx). Параметр [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) или [SyncFolderHierarchy](http://msdn.microsoft.com/library/b31916b1-bc6c-4451-a475-b7c5417f752d%28Office.15%29.aspx) операции можно использовать для получения **FolderId** необходимые. Затем с помощью операции **FindItem** для поиска этой папки для результатов, которые соответствуют фильтру поиска. В отличие от управляемый API веб-служб Exchange веб-служб Exchange не поддерживает операцию отдельные поиска для встреч. Операция **FindItem** извлекает элементы всех типов. 
  
В следующем примере показано XML **FindItem** операция запроса, который отправляется на сервер для поиска встреч в папке календаря, найденных в течение 30 дней. Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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

Сервер отвечает на запрос **FindItem** [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) **NoError**, который указывает, что операция выполнена успешно. Если все элементы календаря не отвечает условий фильтрации, их необходимо включить в ответе.
  
Обратите внимание, что возвращает сведения о сервере в ответ операции **GetItem** , отличается от сведения, которые сервер возвращает **FindItem** или **FindAppointment** операция ответа. Операции **GetItem** может вернуть Схематизированный свойства, тогда как операций **FindItem** и **FindAppointment** не возвращает все Схематизированный свойства. Поэтому если вам требуется полный доступ к элементу, необходимо хранить с помощью операции **GetItem** . Если у вас нет **ItemId** элемента требуется получать, операции **FindItem** или **FindAppointment** использовать для получения **ItemId**и затем с помощью операции **GetItem** элементы, которые необходимо получить. 
  
Чтобы узнать, как получить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [получить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-the-ews-managed-api"></a>Изменение элемента с помощью управляемого API EWS
<a name="bk_updateewsma"> </a>

Действия для обновления элемента с помощью управляемого интерфейса API EWS аналогичны и для всех типов элементов; Тем не менее свойства элемента различны для каждого типа элемента и метод [Update](http://msdn.microsoft.com/en-us/library/office/dd635915%28v=exchg.80%29.aspx) имеет много перегруженных методов, из которых можно выбрать. Чтобы обновить элемент: 
  
1. Метод [привязки](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) для получения последней версии элемента, если у вас уже есть его. Для обновления свойств, относящихся к элементу строго типизированные, необходимо хранить связана с этим типом элемента. Обновляет свойства, доступные на тип универсального элемента, можно привязать к объекту [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) . 
    
2. Измените свойства элемента.
    
3. Вызовите метод **Update** . 
    
Например, вы можете изменить тему сообщения с помощью универсального типа элемента, как показано в коде приведенного ниже примера.
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления. 
  
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

Чтобы узнать, как обновить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [Обновить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="update-an-item-by-using-ews"></a>Изменение элемента с помощью веб-служб Exchange
<a name="bk_updateews"> </a>

Чтобы изменить элемент с помощью веб-служб Exchange, сделайте следующее:
  
1. Если у вас уже есть его с помощью операции [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) для получения последней версии элемента. 
    
2. Используйте операцию [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) для определения полей для обновления и назначить новые значения к этим полям. 
    
В следующем примере показано XML **UpdateItem** операция запроса, который отправляется на сервер для обновления значение [темы](http://msdn.microsoft.com/library/c140d6c2-deb1-4f67-a908-9397197c4ae7%28Office.15%29.aspx) сообщения электронной почты. Для удобства чтения URL были сокращены значения некоторые атрибуты и элементы. 
  
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

Сервер отвечает на запрос **UpdateItem** [UpdateItemResponse](http://msdn.microsoft.com/library/023b79b4-c675-4669-9112-d85499ec4fc4%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что элемент обновление выполнено успешно.
  
Чтобы узнать, как обновить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [Обновить встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-the-ews-managed-api"></a>Удаление элемента с помощью управляемого API EWS
<a name="bk_deleteewsma"> </a>

Можно удалять элементы при перемещении их для папки «Удаленные» или в корзину. Если вы знаете [ItemId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для удаления, просто вызовите метод [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) для элемента. 
  
Если перед удалением элемента необходимо его найти, сделайте следующее:
  
1. Вызовите метод [FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) или [FindAppointments](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findappointments%28v=exchg.80%29.aspx) , чтобы найти элемент, чтобы удалить. 
    
1. Создайте экземпляр [PropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx) и ограничить возвращаемых свойств или использование [SearchFilterCollection](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfilter.searchfiltercollection%28v=exchg.80%29.aspx) для поиска конкретных элементов. 
    
2. Создайте экземпляр [ItemView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemview%28v=EXCHG.80%29.aspx) или [представления календаря](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarview%28v=exchg.80%29.aspx) для указания числа элементов для возврата. 
    
2. Вызовите метод [Delete](http://msdn.microsoft.com/en-us/library/office/dd635072%28v=exchg.80%29.aspx) . 
    
Например, в представленном ниже коде показано, как переместить электронное сообщение в папку "Удаленные".
  
В этом примере предполагается, что эта **Служба** является допустимым объектом [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) и пользователь прошел проверку подлинности на сервере Exchange. Локальной переменной *itemId* — это [идентификатор](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.id%28v=exchg.80%29.aspx) элемента для обновления. 
  
```cs
// Bind to the existing item, using the ItemId.
// This method call results in a GetItem call to EWS.
Item item = Item.Bind(service, itemId);
// Delete the item by moving it to the Deleted Items folder.
// This method call results in a DeleteItem call to EWS.
item.Delete(DeleteMode.MoveToDeletedItems);
```

Для получения дополнительных сведений об удалении элементов видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md). Чтобы узнать, как удалить собрания или встречи с помощью управляемого интерфейса API веб-служб Exchange, обратитесь к разделу [удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="delete-an-item-by-using-ews"></a>Удаление элемента с помощью веб-служб Exchange
<a name="bk_deleteews"> </a>

Элемент можно удалить с помощью операции [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) . 
  
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

Сервер отвечает на запрос **DeleteItem** [DeleteItemResponse](http://msdn.microsoft.com/library/86463d66-fe47-4a19-a81b-e24841e816ab%28Office.15%29.aspx) сообщение, содержащее значение [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**, это означает, что удаления элемента прошла успешно.
  
Для получения дополнительных сведений об удалении элементов видеть [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md). Чтобы узнать, как удалить собрания или встречи с помощью веб-служб Exchange, обратитесь к разделу [удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange](how-to-delete-appointments-and-cancel-meetings-by-using-ews-in-exchange.md).
  
## <a name="move-or-copy-items-to-another-mailbox"></a>Перемещение или копирование элементов в другой почтовый ящик
<a name="bk_movecopybtnmailboxes"> </a>

Можно переместить или скопировать элементы между почтовыми ящиками с помощью операции [ExportItems](http://msdn.microsoft.com/library/e2846abb-0b16-4732-bbd8-038a674672f6%28Office.15%29.aspx) и [UploadItems](http://msdn.microsoft.com/library/a88cbe99-7968-454d-a545-4f92c330909f%28Office.15%29.aspx) . Чтобы получить дополнительные сведения, обратитесь к разделу [Экспорт и импорт элементов с помощью веб-служб Exchange в Exchange](exporting-and-importing-items-by-using-ews-in-exchange.md).
  
## <a name="see-also"></a>См. также

- [Папки и элементы в веб-службах Exchange](folders-and-items-in-ews-in-exchange.md)    
- [Работа с папками с помощью веб-служб Exchange в Exchange](how-to-work-with-folders-by-using-ews-in-exchange.md)    
- [Удаление элементов с помощью веб-служб Exchange в Exchange](deleting-items-by-using-ews-in-exchange.md)
    

