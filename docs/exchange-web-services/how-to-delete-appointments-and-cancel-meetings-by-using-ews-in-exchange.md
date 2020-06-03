---
title: Удаление встреч и отмена собраний с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 42412265-3968-468a-a8c2-7e8af3c6deb9
description: Сведения об удалении встреч и собраний с помощью управляемого API EWS или EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 6a2fdaa357f4088da4bbd0643187d05a5bc51c0c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528134"
---
# <a name="delete-appointments-and-cancel-meetings-by-using-ews-in-exchange"></a><span data-ttu-id="63a8e-103">Удаление встреч и отмена собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-103">Delete appointments and cancel meetings by using EWS in Exchange</span></span>

<span data-ttu-id="63a8e-104">Сведения об удалении встреч и собраний с помощью управляемого API EWS или EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="63a8e-104">Learn how to delete appointments and meetings by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="63a8e-105">Существенным различием между собраниями и встречами является то, что собрания имеют участников, а встречи — нет.</span><span class="sxs-lookup"><span data-stu-id="63a8e-105">The essential difference between meetings and appointments is that meetings have attendees, and appointments don't.</span></span> <span data-ttu-id="63a8e-106">Встречи и собрания могут быть отдельными экземплярами или частью повторяющихся рядов, но так как встречи не включают участников, комнаты или ресурсы, им не требуется отправлять сообщения.</span><span class="sxs-lookup"><span data-stu-id="63a8e-106">Both appointments and meetings can be single instances or part of a recurring series, but because appointments don't include attendees, rooms, or resources, they do not require a message to be sent.</span></span> <span data-ttu-id="63a8e-107">На внутреннем сервере Exchange использует один и тот же объект для собраний и встреч.</span><span class="sxs-lookup"><span data-stu-id="63a8e-107">Internally, Exchange uses the same object for both meetings and appointments.</span></span> <span data-ttu-id="63a8e-108">Для работы с собраниями и встречами используется [класс встречи](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) управляемого API EWS или элемент EWS [календаритем](https://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-108">You use the EWS Managed API [Appointment class](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment%28v=exchg.80%29.aspx) or the EWS [CalendarItem](https://msdn.microsoft.com/library/Title Topic ID Project Name Writer Editor Publish Preview.aspx) element to work with meetings and appointments.</span></span> 
  
<span data-ttu-id="63a8e-109">**Таблица 1. Методы управляемого API EWS и операции EWS для удаления встреч и собраний**</span><span class="sxs-lookup"><span data-stu-id="63a8e-109">**Table 1. EWS Managed API methods and EWS operations for deleting appointments and meetings**</span></span>

|<span data-ttu-id="63a8e-110">**Метод управляемого API EWS**</span><span class="sxs-lookup"><span data-stu-id="63a8e-110">**EWS Managed API method**</span></span>|<span data-ttu-id="63a8e-111">**Операция EWS**</span><span class="sxs-lookup"><span data-stu-id="63a8e-111">**EWS Operation**</span></span>|<span data-ttu-id="63a8e-112">**Действие**</span><span class="sxs-lookup"><span data-stu-id="63a8e-112">**What it does**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="63a8e-113">Встреча. Delete</span><span class="sxs-lookup"><span data-stu-id="63a8e-113">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="63a8e-114">DeleteItem</span><span class="sxs-lookup"><span data-stu-id="63a8e-114">DeleteItem</span></span>](../web-service-reference/deleteitem-operation.md) <br/> |<span data-ttu-id="63a8e-115">Удаляет встречу.</span><span class="sxs-lookup"><span data-stu-id="63a8e-115">Deletes an appointment.</span></span>  <br/> |
|[<span data-ttu-id="63a8e-116">Встреча. Delete</span><span class="sxs-lookup"><span data-stu-id="63a8e-116">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="63a8e-117">CreateItem (элемент календаря)</span><span class="sxs-lookup"><span data-stu-id="63a8e-117">CreateItem (calendar item)</span></span>](../web-service-reference/createitem-operation-calendar-item.md) <br/> |<span data-ttu-id="63a8e-118">Удаляет собрание.</span><span class="sxs-lookup"><span data-stu-id="63a8e-118">Deletes a meeting.</span></span>  <br/> |
   
<span data-ttu-id="63a8e-119">Обратите внимание, что при удалении встречи с помощью EWS вы используете операцию [DeleteItem](../web-service-reference/deleteitem-operation.md) , но при удалении собрания используется операция [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-119">Note that when you delete an appointment by using EWS, you use the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation, but when you delete a meeting, you use the [CreateItem](../web-service-reference/createitem-operation-calendar-item.md) operation.</span></span> <span data-ttu-id="63a8e-120">Это может показаться каунтеринтуитиве, но это связано с тем, что необходимо создать объект ответа на приглашение для отправки сообщений об отмене собрания участникам.</span><span class="sxs-lookup"><span data-stu-id="63a8e-120">This might seem counterintuitive, but it is because you have to create a meeting response object to send meeting cancellation messages to attendees.</span></span> 

<span data-ttu-id="63a8e-121"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="63a8e-121"><a name="bk_DeleteApptEWSMA"> </a></span></span>

## <a name="delete-an-appointment-by-using-the-ews-managed-api"></a><span data-ttu-id="63a8e-122">Удаление встречи с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="63a8e-122">Delete an appointment by using the EWS Managed API</span></span>

<span data-ttu-id="63a8e-123">В следующем примере кода показано, как использовать метод [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) для удаления встречи из папки "Календарь", а также метод [ExchangeService. FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) для проверки того, что встреча удалена, в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="63a8e-123">The following code example shows how to use the [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method to delete an appointment from your calendar folder, and the [ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) method to verify that the appointment was deleted by looking for it in the Deleted Items folder.</span></span> 
  
<span data-ttu-id="63a8e-124">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="63a8e-124">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="63a8e-125">Локальная переменная `appointmentId` — это идентификатор, связанный с существующей встречей.</span><span class="sxs-lookup"><span data-stu-id="63a8e-125">The local variable  `appointmentId` is an identifier associated with an existing appointment.</span></span> 
  
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

<span data-ttu-id="63a8e-126">В этом примере показан простой способ проверки того, что встреча удалена, путем проверки того, что тема первого элемента в папке "Удаленные" совпадает с той, что и удаленная встреча.</span><span class="sxs-lookup"><span data-stu-id="63a8e-126">This example shows a simple way to verify that the appointment was deleted, by verifying that the subject of the first item in the Deleted Items folder matches that of the deleted appointment.</span></span> <span data-ttu-id="63a8e-127">Выбор способа проверки того, что ваша встреча удалена, зависит от потребностей приложения.</span><span class="sxs-lookup"><span data-stu-id="63a8e-127">How you choose to verify that your appointment was deleted will vary based the needs of your application.</span></span>
  
<span data-ttu-id="63a8e-128">Как вы видите, удаление встречи выполняется очень просто и почти так, как вы можете ожидать.</span><span class="sxs-lookup"><span data-stu-id="63a8e-128">As you can see, deleting an appointment is straightforward and pretty much what you might expect.</span></span> <span data-ttu-id="63a8e-129">Обратите внимание, что при создании проверочного действия элемент встречи в папке "Удаленные" имеет другой идентификатор, отличный от элемента встречи в папке "Календарь".</span><span class="sxs-lookup"><span data-stu-id="63a8e-129">Note when you create your verification step that the appointment item in the Deleted Items folder has a different ItemId than the appointment item in the calendar folder.</span></span> <span data-ttu-id="63a8e-130">Элемент копируется и удаляется, а не просто перемещается в папку "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="63a8e-130">The item is copied and deleted rather than simply moved to the Deleted Items folder.</span></span> 
  
## <a name="delete-an-appointment-by-using-ews"></a><span data-ttu-id="63a8e-131">Удаление встречи с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="63a8e-131">Delete an appointment by using EWS</span></span>
<span data-ttu-id="63a8e-132"><a name="bk_DeleteApptEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="63a8e-132"><a name="bk_DeleteApptEWSMA"> </a></span></span>

<span data-ttu-id="63a8e-133">XML-код запроса и ответа в приведенных ниже примерах соответствует вызовам, выполняемым кодом управляемого API EWS в разделе [Удаление встречи с помощью управляемого API EWS](#bk_DeleteApptEWSMA).</span><span class="sxs-lookup"><span data-stu-id="63a8e-133">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete an appointment by using the EWS Managed API](#bk_DeleteApptEWSMA).</span></span> <span data-ttu-id="63a8e-134">Также отображается запрос и ответ XML, проверяющий, что элемент встречи находится в папке "Удаленные".</span><span class="sxs-lookup"><span data-stu-id="63a8e-134">The request and response XML that verifies that the appointment item is in the Deleted Items folder is shown as well.</span></span>
  
<span data-ttu-id="63a8e-135">В следующем примере показан XML-код запроса для операции [DeleteItem](../web-service-reference/deleteitem-operation.md) , чтобы удалить встречу.</span><span class="sxs-lookup"><span data-stu-id="63a8e-135">The following example shows the request XML for the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation to delete an appointment.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="63a8e-136">В следующем примере показан XML-код отклика, возвращенный операцией [DeleteItem](../web-service-reference/deleteitem-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-136">The following example shows the response XML that is returned by the [DeleteItem](../web-service-reference/deleteitem-operation.md) operation.</span></span> <span data-ttu-id="63a8e-137">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63a8e-137">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:DeleteItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:DeleteItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:DeleteItemResponseMessage>
      </m:ResponseMessages>
    </m:DeleteItemResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="63a8e-138">В следующем примере показан XML-код запроса для операции [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папке "Удаленные", чтобы сравнить тему элемента с объектом удаленной встречи.</span><span class="sxs-lookup"><span data-stu-id="63a8e-138">The following example shows the request XML for the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages
" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="63a8e-139">В следующем примере показан XML-код отклика, возвращенный операцией [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этапа проверки.</span><span class="sxs-lookup"><span data-stu-id="63a8e-139">The following example shows the response XML that is returned by the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="63a8e-140">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63a8e-140">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="63a8e-141"><a name="bk_DeleteMtgEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="63a8e-141"><a name="bk_DeleteMtgEWSMA"> </a></span></span>

## <a name="delete-a-meeting-by-using-the-ews-managed-api"></a><span data-ttu-id="63a8e-142">Удаление собрания с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="63a8e-142">Delete a meeting by using the EWS Managed API</span></span>

<span data-ttu-id="63a8e-143">Когда вы удаляете собрание, а не удаляете его из папки "Календарь", вам также может потребоваться отправить уведомления об отмене собрания участникам.</span><span class="sxs-lookup"><span data-stu-id="63a8e-143">When you delete a meeting, in addition to removing the appointment item from the calendar folder, you might also want to send meeting cancellations to attendees.</span></span> <span data-ttu-id="63a8e-144">Для отмены собрания можно использовать следующие три метода:</span><span class="sxs-lookup"><span data-stu-id="63a8e-144">You can use the following three methods to cancel a meeting:</span></span>
  
- [<span data-ttu-id="63a8e-145">Встреча. Delete</span><span class="sxs-lookup"><span data-stu-id="63a8e-145">Appointment.Delete</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="63a8e-146">Встреча. Канцелмитинг</span><span class="sxs-lookup"><span data-stu-id="63a8e-146">Appointment.CancelMeeting</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx)
    
- [<span data-ttu-id="63a8e-147">канцелмитингмессаже</span><span class="sxs-lookup"><span data-stu-id="63a8e-147">CancelMeetingMessage</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx)
    
<span data-ttu-id="63a8e-148">Выбор метода зависит от уровня детализации, который необходимо указать в сообщении об отмене.</span><span class="sxs-lookup"><span data-stu-id="63a8e-148">The method that you choose depends on the level of detail you need to provide in your cancellation message.</span></span> <span data-ttu-id="63a8e-149">[Встреча. канцелмитинг](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) упрощает обновление сообщения об отмене путем передачи обновленного сообщения в качестве параметра.</span><span class="sxs-lookup"><span data-stu-id="63a8e-149">[Appointment.CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) makes it easy to update the cancellation message by passing an updated message as a parameter.</span></span> <span data-ttu-id="63a8e-150">[Канцелмитингмессаже](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) позволяет изменять свойства своего сообщения перед отправкой отмены, поэтому вы можете выполнять такие действия, как запрос уведомления.</span><span class="sxs-lookup"><span data-stu-id="63a8e-150">[CancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.cancelmeetingmessage%28v=exchg.80%29.aspx) allows you to modify properties on your message before sending a cancellation, so you can do things like request a receipt.</span></span> 
  
<span data-ttu-id="63a8e-151">В примерах кода, приведенных в этом разделе, показаны различные способы удаления собрания и отправки сообщений об отмене собрания.</span><span class="sxs-lookup"><span data-stu-id="63a8e-151">The code examples in this section show the different ways to delete a meeting and send meeting cancellations.</span></span> <span data-ttu-id="63a8e-152">В примерах предполагается, что вы прошли проверку подлинности на сервере Exchange и получили объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="63a8e-152">The examples assume that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> <span data-ttu-id="63a8e-153">Локальная переменная `meetingId` — это идентификатор, связанный с существующим собранием, где целевой пользователь является организатором собрания.</span><span class="sxs-lookup"><span data-stu-id="63a8e-153">The local variable  `meetingId` is an identifier associated with an existing meeting where the target user is the meeting organizer.</span></span> 
  
<span data-ttu-id="63a8e-154">В приведенном ниже примере кода показано, как удалить собрание с помощью метода [встреча. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-154">The following code example shows how to delete a meeting by using the [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
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

<span data-ttu-id="63a8e-155">В приведенном ниже примере кода показано, как удалить собрание с помощью метода [канцелмитинг](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-155">The following code example shows how to delete a meeting by using the [CancelMeeting](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.cancelmeeting%28v=exchg.80%29.aspx) method.</span></span> 
  
```cs
// Instantiate an appointment object by binding to it using the ItemId.
// As a best practice, limit the properties returned to only the Appointment ID.
Appointment meeting = Appointment.Bind(service, meetingId, new PropertySet());
// Delete the meeting by using the CancelMeeting method.
meeting.CancelMeeting("The outdoor meeting has been cancelled due to hailstorms.");

```

<span data-ttu-id="63a8e-156">В приведенном ниже примере кода показано, как удалить собрание с помощью метода [встреча. креатеканцелмитингмессаже](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-156">The following code example shows how to delete a meeting by using the [Appointment.CreateCancelMeetingMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.createcancelmeetingmessage%28v=exchg.80%29.aspx) method.</span></span> 
  
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

## <a name="delete-a-meeting-by-using-ews"></a><span data-ttu-id="63a8e-157">Удаление собрания с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="63a8e-157">Delete a meeting by using EWS</span></span>
<span data-ttu-id="63a8e-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span><span class="sxs-lookup"><span data-stu-id="63a8e-158"><a name="bk_EWSDeleteApptAndMeeting"> </a></span></span>

<span data-ttu-id="63a8e-159">XML-код запроса и ответа в приведенных ниже примерах соответствует вызовам, выполняемым кодом управляемого API EWS в разделе [Удаление собрания с помощью управляемого API EWS](#bk_DeleteMtgEWSMA) с помощью метода [встречи. Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="63a8e-159">The request and response XML in the following examples correspond to calls made by the EWS Managed API code in [Delete a meeting by using the EWS Managed API](#bk_DeleteMtgEWSMA) by using the [Appointment.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx) method.</span></span> 
  
<span data-ttu-id="63a8e-160">В следующем примере показан XML-код запроса при использовании операции [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) для отправки сообщений об отмене участникам и удаления собрания.</span><span class="sxs-lookup"><span data-stu-id="63a8e-160">The following example shows the request XML when you use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to send cancellation messages to attendees and delete a meeting.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="63a8e-161">В следующем примере показан XML-код, который возвращается в ответ на запрос операции [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) , используемый для удаления собрания.</span><span class="sxs-lookup"><span data-stu-id="63a8e-161">The following example shows the XML that is returned in response to a [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation request used to delete a meeting.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="63a8e-162">Атрибуты **ItemId** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63a8e-162">The **ItemId** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:CreateItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="63a8e-163">В следующем примере показан XML-код запроса для операции [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) , который получает первый элемент в папке "Удаленные", чтобы сравнить тему элемента с объектом удаленной встречи.</span><span class="sxs-lookup"><span data-stu-id="63a8e-163">The following example shows the request XML for the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation that retrieves the first item in the Deleted Items folder in order to compare the item's subject with that of the deleted appointment object.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="63a8e-164">В следующем примере показан XML-код, возвращенный операцией [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) во время этапа проверки.</span><span class="sxs-lookup"><span data-stu-id="63a8e-164">The following example shows the XML that is returned by the [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation during the verification step.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="63a8e-165">Атрибуты **ID** и **чанжекэй** сокращаются для удобочитаемости.</span><span class="sxs-lookup"><span data-stu-id="63a8e-165">The **Id** and **ChangeKey** attributes are shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="800" MinorBuildNumber="5" Version="V2_6" 
 xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
 xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
 xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="63a8e-166">См. также</span><span class="sxs-lookup"><span data-stu-id="63a8e-166">See also</span></span>

- [<span data-ttu-id="63a8e-167">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-167">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)    
- [<span data-ttu-id="63a8e-168">Создание встреч и собраний с помощью EWS в Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="63a8e-168">Create appointments and meetings by using EWS in Exchange 2013</span></span>](how-to-create-appointments-and-meetings-by-using-ews-in-exchange-2013.md)  
- [<span data-ttu-id="63a8e-169">Получение встреч и собраний с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-169">Get appointments and meetings by using EWS in Exchange</span></span>](how-to-get-appointments-and-meetings-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="63a8e-170">Обновление встречи и собрания с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-170">Update appointments and meetings by using EWS in Exchange</span></span>](how-to-update-appointments-and-meetings-by-using-ews-in-exchange.md)  
- [<span data-ttu-id="63a8e-171">Предложение нового времени проведения собрания с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-171">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md) 
- [<span data-ttu-id="63a8e-172">Предложение нового времени проведения собрания с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="63a8e-172">Propose a new meeting time by using EWS in Exchange</span></span>](how-to-propose-a-new-meeting-time-by-using-ews-in-exchange.md)
    

