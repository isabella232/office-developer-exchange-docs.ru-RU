---
title: Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Узнайте, как удалить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: c71272bf753432a9f343adc917b444424fe3ba33
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354080"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a>Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange

Узнайте, как удалить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
  
Важные различия между собраний и встреч —, что у участников собрания, а не встреч. Встречи и собрания могут быть отдельные экземпляры или частью серии повторяющихся, но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение. Для внутреннего использования Exchange использует тот же объект для собраний и встреч. Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) для работы с собраний и встреч. 
  
**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для удаления встречи и собрания**

|**Метод управляемого API EWS**|**Операция EWS**|**Назначение**|
|:-----|:-----|:-----|
|[Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |Удаляет встречи.  <br/> |
|[Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[CreateItem (элемента календаря)](../web-service-reference/createitem-operation-calendar-item.md) <br/> |Удаление собрания.  <br/> |
   
Обратите внимание на то, что при удалении встречи с помощью веб-служб Exchange, используйте операцию [DeleteItem](../web-service-reference/deleteitem-operation.md) , но при удалении собрания можно использовать операцию [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) . Это может показаться нелогичным, но поскольку необходимо создать собрание объект ответа для отправки отмены собрания сообщений участникам. 

<a name="bk_DeleteApptEWSMA"> </a>

## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a>Удаление встречи с помощью управляемого интерфейса API веб-служб Exchange

В следующем примере кода показано, как использовать метод [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) для удаления встречу из папки календаря и метод [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , чтобы убедиться, что встречи был удален, найти его в папку «Удаленные». 
  
В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. Локальной переменной `appointmentId` — это идентификатор, связанный с существующей встречи. 
  
```cs
// Instantiate an appointment object by binding to it by using the ItemId.
// As a best practice, limit the properties returned to only the ones you need.
Appointment appointment = Appointment.Bind(service, appointmentId, new PropertySet());
// Delete the appointment. Note that the item ID will change when the item is moved to the Deleted Items folder.
appointment.Delete(DeleteMode.MoveToDeletedItems);
// Verify that the appointment has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The appointment " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

В этом примере показано простое, проверять, был удален встречи, убедитесь, что тему к первому элементу в папку «Удаленные», совпадает с удаленного встречи. Зависит от способа убедитесь, что было удалено встречи на основе требований приложения.
  
Как вы видите, удаление встречи не вызывает затруднений и практически ожиданиям. Примечание для создания вашего этап проверки различных ItemId чем элемента встречи в папке календаря на наличие элемента встречи в папку «Удаленные». Элемент — это скопировать и удалении, а не просто перемещено в папку «Удаленные». 
  
## <a name="delete-an-appointment-by-using-ews"></a>Удаление встречи с помощью веб-служб Exchange
<a name="bk_DeleteApptEWSMA"> </a>

Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [Удаление встречи с помощью управляемого интерфейса API веб-служб Exchange](#bk_DeleteApptEWSMA). Запрос и ответ также показан XML-кода, проверяет, является ли элемента встречи в папку «Удаленные».
  
В следующем примере показано запроса XML для операции [DeleteItem](../web-service-reference/deleteitem-operation.md) удаление встречи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:DeleteItem DeleteType="MoveToDeletedItems" SendMeetingCancellations="SendToAllAndSaveCopy">
      <m:ItemIds>
        <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
      </m:ItemIds>
    </m:DeleteItem>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML, возвращенные операцией [DeleteItem](../web-service-reference/deleteitem-operation.md) ответа. Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

В следующем примере показано запроса XML для операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папку «Удаленные» для сравнения Тема элемента с помощью объекта удаленного встречи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages
" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано ответа XML, возвращенные операцией [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этап проверки. 
  
> [!NOTE]
> Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10748" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA=" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Tennis lesson</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

<a name="bk_DeleteMtgEWSMA"> </a>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a>Удаление собрания с помощью управляемого интерфейса API веб-служб Exchange

При удалении собрания, кроме удаления элемента встречи из папки "Календарь" можно также отправить отмен собрания участникам. Отмена собрания можно использовать следующие три метода:
  
- [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
Выбор метода зависит от уровня детализации, которые необходимо указать в сообщении отмены. [Appointment.CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) позволяет обновить сообщение об отмене, передавая обновленные сообщения в качестве параметра. [CancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) позволяет изменять свойства сообщения перед отправкой отмен собрания, что позволяет выполнять такие запроса на уведомление о. 
  
В примерах кода в этом разделе показано, различные способы удаления собрания и отправить отмен собрания. В примерах предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**. Локальной переменной `meetingId` — это идентификатор, связанный с существующего собрания, где конечного пользователя является организатором собрания. 
  
В следующем примере кода показано, как удалить собрание с помощью метода [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) . 
  
```cs
// Instantiate an appointment object for the meeting by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
            
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the Delete method.
meeting.Delete(DeleteMode.MoveToDeletedItems, SendCancellationsMode.SendToAllAndSaveCopy);
// Verify that the meeting has been deleted by looking for a matching subject in the Deleted Items folder's first entry.
ItemView itemView = new ItemView(1);
itemView.Traversal = ItemTraversal.Shallow;
// Just retrieve the properties you need.
itemView.PropertySet = new PropertySet(ItemSchema.Id, ItemSchema.ParentFolderId, ItemSchema.Subject);
// Note that the FindItems method results in a call to EWS.
FindItemsResults<Item> deletedItems = service.FindItems(WellKnownFolderName.DeletedItems, itemView);
Item deletedItem = deletedItems.First();
Folder parentFolder = Folder.Bind(service, deletedItem.ParentFolderId, new PropertySet(FolderSchema.DisplayName));
Console.WriteLine("The meeting " + "\"" + deletedItem.Subject + "\"" + " is now in the " + parentFolder.DisplayName + " folder.");

```

В следующем примере кода показано, как удалить собрание с помощью метода [CancelMeeting](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) . 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

В следующем примере кода показано, как удалить собрание с помощью метода [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) . 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CreateCancelMeetingMessage method.
CancelMeetingMessage cancelMessage = meeting.CreateCancelMeetingMessage();
cancelMessage.Body = new MessageBody("The outdoor meeting has been canceled due to hailstorms.");
cancelMessage.IsReadReceiptRequested = true;
cancelMessage.SendAndSaveCopy();

```

## <a name="delete-a-meeting-by-using-ews"></a>Удаление собрания с помощью веб-служб Exchange
<a name="bk_EWSDeleteApptAndMeeting"> </a>

Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [Удалить собрание с помощью управляемого интерфейса API веб-служб Exchange](#bk_DeleteMtgEWSMA) с помощью метода [Appointment.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) . 
  
В следующем примере показано запроса XML при использовании операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для отмены сообщения для участников и удаление собрания. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SendAndSaveCopy">
      <m:Items>
        <t:CancelCalendarItem>
          <t:ReferenceItemId Id="AAMkA" ChangeKey="DwAAA" />
          <t:NewBodyContent BodyType="HTML">The outdoor meeting has been canceled due to hailstorms.</t:NewBodyContent>
        </t:CancelCalendarItem>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML-код, который возвращается в ответ на запрос [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) операции, используется для удаления собрания. 
  
> [!NOTE]
> Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
            </t:CalendarItem>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>

```

В следующем примере показано запроса XML для операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папку «Удаленные» для сравнения Тема элемента с помощью объекта удаленного встречи. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Pacific Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:ItemId" />
          <t:FieldURI FieldURI="item:ParentFolderId" />
          <t:FieldURI FieldURI="item:Subject" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="deleteditems" />
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>

```

В следующем примере показано XML-данные, возвращенные операцией [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этап проверки. 
  
> [!NOTE]
> Атрибуты **Id** и **ChangeKey** сокращаются для удобства чтения. 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1" TotalItemsInView="10750" IncludesLastItemInRange="false">
            <t:Items>
              <t:CalendarItem>
                <t:ItemId Id="AAMkA" ChangeKey="DwAAA" />
                <t:ParentFolderId Id="AAMkA" ChangeKey="AQAAA" />
                <t:Subject>Team building exercise</t:Subject>
              </t:CalendarItem>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a>См. также

- [Календари и веб-службах Exchange](calendars-and-ews-in-exchange.md)    
- [Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [Получение встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [Обновление встречи и собрания с помощью веб-служб Exchange в Exchange](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

