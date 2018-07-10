---
title: Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Узнайте, как удалить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.
ms.openlocfilehash: bd7eac803fedffc51133324259f68fd25652fcff
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761002"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="110ed-103">Удаление встреч и отмены собраний с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-103">Delete appointments and cancel meetings by using EWS in Exchange</span></span>

<span data-ttu-id="110ed-104">Узнайте, как удалить встречи и собрания с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange в Exchange.</span><span class="sxs-lookup"><span data-stu-id="110ed-104">Learn how to delete appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="110ed-105">Важные различия между собраний и встреч —, что у участников собрания, а не встреч.</span><span class="sxs-lookup"><span data-stu-id="110ed-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="110ed-106">Встречи и собрания могут быть отдельные экземпляры или частью серии повторяющихся, но поскольку встреч не включать участников, комнат или ресурсов, не требуется отправить сообщение.</span><span class="sxs-lookup"><span data-stu-id="110ed-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="110ed-107">Для внутреннего использования Exchange использует тот же объект для собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="110ed-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="110ed-108">Использовать управляемый API EWS [класс встречи](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) или элемент веб-служб Exchange [элемента календаря, имеющего](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) для работы с собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="110ed-108">You use the EWS Managed API [Appointment class](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](http://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="110ed-109">**В таблице 1. Управляемый API EWS методы и операции веб-служб Exchange для удаления встречи и собрания**</span><span class="sxs-lookup"><span data-stu-id="110ed-109">**Table 1. EWS Managed API methods and EWS operations for deleting appointments and meetings**</span></span>

|<span data-ttu-id="110ed-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="110ed-110">**EWS Managed API method**</span></span>|<span data-ttu-id="110ed-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="110ed-111">**EWS Operation**</span></span>|<span data-ttu-id="110ed-112">**Назначение**</span><span class="sxs-lookup"><span data-stu-id="110ed-112">**What it does**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="110ed-113">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="110ed-113">Appointment.Delete</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="110ed-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="110ed-114">DeleteItem</span></span>](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |<span data-ttu-id="110ed-115">Удаляет встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-115">Deletes an appointment.</span></span>  <br/> |
|[<span data-ttu-id="110ed-116">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="110ed-116">Appointment.Delete</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="110ed-117">CreateItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="110ed-117">CreateItem (calendar item)</span></span>](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) <br/> |<span data-ttu-id="110ed-118">Удаление собрания.</span><span class="sxs-lookup"><span data-stu-id="110ed-118">Deletes a meeting.</span></span>  <br/> |
   
<span data-ttu-id="110ed-119">Обратите внимание на то, что при удалении встречи с помощью веб-служб Exchange, используйте операцию [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) , но при удалении собрания можно использовать операцию [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="110ed-119">Note that when you delete an appointment by using EWS, you use the [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) operation, but when you delete a meeting, you use the [CreateItem ](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="110ed-120">Это может показаться нелогичным, но поскольку необходимо создать собрание объект ответа для отправки отмены собрания сообщений участникам.</span><span class="sxs-lookup"><span data-stu-id="110ed-120">This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> 
  
## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="110ed-121">Удаление встречи с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-121">Delete an appointment by using the EWS Managed API</span></span>
<span data-ttu-id="110ed-122"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="110ed-122"></span></span>

<span data-ttu-id="110ed-123">В следующем примере кода показано, как использовать метод [Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) для удаления встречу из папки календаря и метод [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) , чтобы убедиться, что встречи был удален, найти его в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="110ed-123">The following code example shows how to use the [Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method to delete an appointment from your calendar folder, and the [ExchangeService.FindItems](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method to verify that the appointment was deleted by looking for it in the Deleted Items folder.</span></span> 
  
<span data-ttu-id="110ed-124">В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="110ed-124">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="110ed-125">Локальной переменной `appointmentId` — это идентификатор, связанный с существующей встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-125">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
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

<span data-ttu-id="110ed-126">В этом примере показано простое, проверять, был удален встречи, убедитесь, что тему к первому элементу в папку «Удаленные», совпадает с удаленного встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-126">This example shows a simple way to verify that the appointment was deleted, by verifying that the subject of the first item in the Deleted Items folder matches that of the deleted appointment.</span></span> <span data-ttu-id="110ed-127">Зависит от способа убедитесь, что было удалено встречи на основе требований приложения.</span><span class="sxs-lookup"><span data-stu-id="110ed-127">How you choose to verify that your appointment was deleted will vary based the needs of your application.</span></span>
  
<span data-ttu-id="110ed-128">Как вы видите, удаление встречи не вызывает затруднений и практически ожиданиям.</span><span class="sxs-lookup"><span data-stu-id="110ed-128">As you can see, deleting an appointment is straightforward and pretty much what you might expect.</span></span> <span data-ttu-id="110ed-129">Примечание для создания вашего этап проверки различных ItemId чем элемента встречи в папке календаря на наличие элемента встречи в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="110ed-129">Note when you create your verification step that the appointment item in the Deleted Items folder has a different ItemId than the appointment item in the calendar folder.</span></span> <span data-ttu-id="110ed-130">Элемент — это скопировать и удалении, а не просто перемещено в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="110ed-130">The item is copied and deleted rather than simply moved to the Deleted Items folder.</span></span> 
  
## <a name="delete-an-appointment-by-using-ews"></a><span data-ttu-id="110ed-131">Удаление встречи с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-131">Delete an appointment by using EWS</span></span>
<span data-ttu-id="110ed-132"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="110ed-132"></span></span>

<span data-ttu-id="110ed-133">Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [Удаление встречи с помощью управляемого интерфейса API веб-служб Exchange](#bk_DeleteApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="110ed-133">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete an appointment by using the EWS Managed API](#bk_DeleteApptEWSMA).</span></span> <span data-ttu-id="110ed-134">Запрос и ответ также показан XML-кода, проверяет, является ли элемента встречи в папку «Удаленные».</span><span class="sxs-lookup"><span data-stu-id="110ed-134">The request and response XML that verifies that the appointment item is in the Deleted Items folder is shown as well.</span></span>
  
<span data-ttu-id="110ed-135">В следующем примере показано запроса XML для операции [DeleteItem](http://msdn.microsoft.com/library/e2152410-41ce-1fe7-8169-f206d5081ebc%28Office.15%29.aspx) удаление встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-135">The following example shows the request XML for the [DeleteItem](http://msdn.microsoft.com/library/e2152410-41ce-1fe7-8169-f206d5081ebc%28Office.15%29.aspx) operation to delete an appointment.</span></span> 
  
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

<span data-ttu-id="110ed-136">В следующем примере показано ответа XML, возвращенные [DeleteItem операции](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="110ed-136">The following example shows the response XML that is returned by the [DeleteItem operation](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx).</span></span> <span data-ttu-id="110ed-137">Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="110ed-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="110ed-138">В следующем примере показано запроса XML для операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папку «Удаленные» для сравнения Тема элемента с помощью объекта удаленного встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-138">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
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

<span data-ttu-id="110ed-139">В следующем примере показано ответа XML, возвращенные операцией [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этап проверки.</span><span class="sxs-lookup"><span data-stu-id="110ed-139">The following example shows the response XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="110ed-140">Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="110ed-140">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="110ed-141"><a name="bk_DeleteMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="110ed-141"></span></span>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="110ed-142">Удаление собрания с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-142">Delete a meeting by using the EWS Managed API</span></span>

<span data-ttu-id="110ed-143">При удалении собрания, кроме удаления элемента встречи из папки "Календарь" можно также отправить отмен собрания участникам.</span><span class="sxs-lookup"><span data-stu-id="110ed-143">When you delete a meeting, in addition to removing the appointment item from the calendar folder, you might also want to send meeting cancellations to attendees.</span></span> <span data-ttu-id="110ed-144">Отмена собрания можно использовать следующие три метода:</span><span class="sxs-lookup"><span data-stu-id="110ed-144">You can use the following three methods to cancel a meeting:</span></span>
  
- [<span data-ttu-id="110ed-145">Appointment.Delete</span><span class="sxs-lookup"><span data-stu-id="110ed-145">Appointment.Delete</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="110ed-146">Appointment.CancelMeeting</span><span class="sxs-lookup"><span data-stu-id="110ed-146">Appointment.CancelMeeting</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="110ed-147">CancelMeetingMessage</span><span class="sxs-lookup"><span data-stu-id="110ed-147">CancelMeetingMessage</span></span>](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
<span data-ttu-id="110ed-148">Выбор метода зависит от уровня детализации, которые необходимо указать в сообщении отмены.</span><span class="sxs-lookup"><span data-stu-id="110ed-148">The method that you choose depends on the level of detail you need to provide in your cancellation message.</span></span> <span data-ttu-id="110ed-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) позволяет обновить сообщение об отмене, передавая обновленные сообщения в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="110ed-149">[Appointment.CancelMeeting](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) makes it easy to update the cancellation message by passing an updated message as a parameter.</span></span> <span data-ttu-id="110ed-150">[CancelMeetingMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) позволяет изменять свойства сообщения перед отправкой отмен собрания, что позволяет выполнять такие запроса на уведомление о.</span><span class="sxs-lookup"><span data-stu-id="110ed-150">[CancelMeetingMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) allows you to modify properties on your message before sending a cancellation, so you can do things like request a receipt.</span></span> 
  
<span data-ttu-id="110ed-151">В примерах кода в этом разделе показано, различные способы удаления собрания и отправить отмен собрания.</span><span class="sxs-lookup"><span data-stu-id="110ed-151">The code examples in this section show the different ways to delete a meeting and send meeting cancellations.</span></span> <span data-ttu-id="110ed-152">В примерах предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="110ed-152">The examples assume that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="110ed-153">Локальной переменной `meetingId` — это идентификатор, связанный с существующего собрания, где конечного пользователя является организатором собрания.</span><span class="sxs-lookup"><span data-stu-id="110ed-153">The local variable  `meetingId` is an identifier associated with an existing meeting where the target user is the meeting organizer.</span></span> 
  
<span data-ttu-id="110ed-154">В следующем примере кода показано, как удалить собрание с помощью метода [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="110ed-154">The following code example shows how to delete a meeting by using the [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="110ed-155">В следующем примере кода показано, как удалить собрание с помощью метода [CancelMeeting](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="110ed-155">The following code example shows how to delete a meeting by using the [CancelMeeting](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

<span data-ttu-id="110ed-156">В следующем примере кода показано, как удалить собрание с помощью метода [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="110ed-156">The following code example shows how to delete a meeting by using the [Appointment.CreateCancelMeetingMessage](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) method.</span></span> 
  
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

## <a name="delete-a-meeting-by-using-ews"></a><span data-ttu-id="110ed-157">Удаление собрания с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-157">Delete a meeting by using EWS</span></span>
<span data-ttu-id="110ed-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span><span class="sxs-lookup"><span data-stu-id="110ed-158"></span></span>

<span data-ttu-id="110ed-159">Запрос и ответ XML в следующих примерах соответствуют вызовов, сделанных с помощью кода управляемый API EWS в [Удалить собрание с помощью управляемого интерфейса API веб-служб Exchange](#bk_DeleteMtgEWSMA) с помощью метода [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="110ed-159">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete a meeting by using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the [Appointment.Delete](http://msdn.microsoft.com/ru-ru/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="110ed-160">В следующем примере показано запроса XML при использовании операции [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для отмены сообщения для участников и удаление собрания.</span><span class="sxs-lookup"><span data-stu-id="110ed-160">The following example shows the request XML when you use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to send cancellation messages to attendees and delete a meeting.</span></span> 
  
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

<span data-ttu-id="110ed-161">В следующем примере показано XML-код, который возвращается в ответ на запрос [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) операции, используется для удаления собрания.</span><span class="sxs-lookup"><span data-stu-id="110ed-161">The following example shows the XML that is returned in response to a [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation request used to delete a meeting.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="110ed-162">Атрибуты **ItemId** и **ChangeKey** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="110ed-162">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

<span data-ttu-id="110ed-163">В следующем примере показано запроса XML для операции [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папку «Удаленные» для сравнения Тема элемента с помощью объекта удаленного встречи.</span><span class="sxs-lookup"><span data-stu-id="110ed-163">The following example shows the request XML for the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
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

<span data-ttu-id="110ed-164">В следующем примере показано XML-данные, возвращенные операцией [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этап проверки.</span><span class="sxs-lookup"><span data-stu-id="110ed-164">The following example shows the XML that is returned by the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="110ed-165">Атрибуты **Id** и **ChangeKey** сокращаются для удобства чтения.</span><span class="sxs-lookup"><span data-stu-id="110ed-165">The **Id** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
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

## <a name="see-also"></a><span data-ttu-id="110ed-166">См. также</span><span class="sxs-lookup"><span data-stu-id="110ed-166">See also</span></span>

- [<span data-ttu-id="110ed-167">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-167">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)    
- [<span data-ttu-id="110ed-168">Создание встречи и собрания с помощью веб-служб Exchange в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="110ed-168">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="110ed-169">Получение встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-169">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="110ed-170">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-170">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="110ed-171">Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-171">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="110ed-172">Предложение нового времени проведения собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="110ed-172">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

