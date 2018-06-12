---
title: Получить список помещений с помощью веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 15980e4a-e41c-4194-829a-cadbdf365bf1
description: Узнайте, как получить список всех списков помещения в вашей организации или в список помещений одного из Exchange server с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.
ms.openlocfilehash: 404a31fb6c8d98bdbba4c79ed6912c333a44d04b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761011"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a><span data-ttu-id="ee11a-103">Получить список помещений с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-103">Get room lists by using EWS in Exchange</span></span>

<span data-ttu-id="ee11a-104">Узнайте, как получить список всех списков помещения в вашей организации или в список помещений одного из Exchange server с помощью управляемого интерфейса API веб-служб Exchange или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee11a-104">Learn how to get a list of all the room lists in your organization or a single room list from an Exchange server by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="ee11a-105">Для получения сведений о комнат, а также группировку комнат в вашей организации, можно использовать управляемый API EWS или веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="ee11a-105">You can use the EWS Managed API or EWS to get information about rooms and how the rooms are grouped in your organization.</span></span> <span data-ttu-id="ee11a-106">Не существует комнаты списков по умолчанию; Администратор должен создать и разместите их.</span><span class="sxs-lookup"><span data-stu-id="ee11a-106">Room lists don't exist by default; your administrator needs to create and organize them.</span></span> <span data-ttu-id="ee11a-107">Как правило они вы организованы расположения или отдела, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="ee11a-107">Typically, they're organized by location or department, as shown in the following example.</span></span>
  
<span data-ttu-id="ee11a-108">**Получение списка имен объектов Contoso комнаты и адреса электронной почты**</span><span class="sxs-lookup"><span data-stu-id="ee11a-108">**Contoso room list names and email addresses**</span></span>

|<span data-ttu-id="ee11a-109">**Имя списка помещений**</span><span class="sxs-lookup"><span data-stu-id="ee11a-109">**Name of room list**</span></span>|<span data-ttu-id="ee11a-110">**Адрес электронной почты в список помещений**</span><span class="sxs-lookup"><span data-stu-id="ee11a-110">**Email address of room list**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee11a-111">Создание списка 11 комнаты</span><span class="sxs-lookup"><span data-stu-id="ee11a-111">Building 11 room list</span></span>  <br/> |<span data-ttu-id="ee11a-112">Bldg11rooms@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee11a-112">Bldg11rooms@contoso.com</span></span>  <br/> |
|<span data-ttu-id="ee11a-113">Список помещений конференции построения науки работоспособности</span><span class="sxs-lookup"><span data-stu-id="ee11a-113">Health Science Building Conference Room List</span></span>  <br/> |<span data-ttu-id="ee11a-114">HSbldgrooms@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="ee11a-114">HSbldgrooms@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="ee11a-115">Комнаты для собраний этажа бухгалтерского учета</span><span class="sxs-lookup"><span data-stu-id="ee11a-115">Accounting Floor Meeting Rooms</span></span>  <br/> |<span data-ttu-id="ee11a-116">Acctfloor300@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee11a-116">Acctfloor300@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="ee11a-117">Каждый помещения в список помещений имеет имя и адрес электронной почты адрес, связанный с ним.</span><span class="sxs-lookup"><span data-stu-id="ee11a-117">Each room in a room list has a name and email address associated with it.</span></span>
  
<span data-ttu-id="ee11a-118">**Contoso комнаты и адреса электронной почты**</span><span class="sxs-lookup"><span data-stu-id="ee11a-118">**Contoso room names and email addresses**</span></span>

|<span data-ttu-id="ee11a-119">**Имя комнаты**</span><span class="sxs-lookup"><span data-stu-id="ee11a-119">**Name of room**</span></span>|<span data-ttu-id="ee11a-120">**Адрес электронной почты для комнаты**</span><span class="sxs-lookup"><span data-stu-id="ee11a-120">**Email address of room**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ee11a-121">Комнаты conf 11/101 (8) аудио/видео</span><span class="sxs-lookup"><span data-stu-id="ee11a-121">Conf Room 11/101 (8) AV</span></span>  <br/> |<span data-ttu-id="ee11a-122">Cf11101@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee11a-122">Cf11101@contoso.com</span></span>  <br/> |
|<span data-ttu-id="ee11a-123">Для демонстрации HS лаборатории (100)</span><span class="sxs-lookup"><span data-stu-id="ee11a-123">HS Demonstration Lab (100)</span></span>  <br/> |<span data-ttu-id="ee11a-124">Hs101@Contoso.edu</span><span class="sxs-lookup"><span data-stu-id="ee11a-124">Hs101@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="ee11a-125">Учет 305 МБ</span><span class="sxs-lookup"><span data-stu-id="ee11a-125">Accounting 305 WB</span></span>  <br/> |<span data-ttu-id="ee11a-126">Acct305@Contoso.com</span><span class="sxs-lookup"><span data-stu-id="ee11a-126">Acct305@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="ee11a-127">Можно получить список, содержащий все список помещений с помощью метода управляемый API EWS [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) или операции [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="ee11a-127">You can get a list that contains all room lists by using either the [ExchangeService.GetRoomLists](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="ee11a-128">Можно извлечь список единого места, содержащий всех комнатах для расположения или отдела, передав его адрес электронной почты с помощью метода управляемый API EWS [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) или операции EWS [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ee11a-128">You can retrieve a single room list that contains all the rooms for a location or department by supplying its email address by using the [GetRooms](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="ee11a-129">При наличии коллекцию каналы, связанные с почтового ящика помещения, затем выполнить поиск по коллекции для определения места или комнат, по которым вы путем адрес электронной почты или поиск по ключевым словам в поле имя, например «Аудио/видео» или «Лаборатория».</span><span class="sxs-lookup"><span data-stu-id="ee11a-129">When you have a collection of rooms associated with a room list, you can then search through the collection to identify the room or rooms you want, either by email address, or by looking for key words in the name, such as "AV", or "Lab".</span></span> 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a><span data-ttu-id="ee11a-130">Получение списков всех комнат с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-130">Get all room lists by using the EWS Managed API</span></span>
<span data-ttu-id="ee11a-131"><a name="bk_GetRoomListewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ee11a-131"></span></span>

<span data-ttu-id="ee11a-132">Следующем примере показано, как получить список, содержащий все список помещений в вашей организации с помощью метода [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ee11a-132">The following example shows how to get a list that contains all the room lists in your organization by using the [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) method.</span></span> 
  
<span data-ttu-id="ee11a-133">В этом примере предполагается, что прошедшие проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **службы**.</span><span class="sxs-lookup"><span data-stu-id="ee11a-133">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
```cs
// Return all the room lists in the organization.
// This method call results in a GetRoomLists call to EWS.
EmailAddressCollection myRoomLists = service.GetRoomLists();
// Display the room lists.
foreach (EmailAddress address in myRoomLists)
{
    Console.WriteLine("Email Address: {0} Mailbox Type: {1}", address.Address, address.MailboxType);
}

```

## <a name="get-all-room-lists-by-using-ews"></a><span data-ttu-id="ee11a-134">Получение списков всех комнат с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-134">Get all room lists by using EWS</span></span>
<span data-ttu-id="ee11a-135"><a name="bk_GetRoomListews"> </a></span><span class="sxs-lookup"><span data-stu-id="ee11a-135"></span></span>

<span data-ttu-id="ee11a-136">Следующем примере показано, как получить коллекцию вашей организации [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) с помощью операции [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ee11a-136">The following example shows how to get a collection of all your organization's [RoomLists](http://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) by using the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="ee11a-137">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API EWS для [получения всех списков комнаты](#bk_GetRoomListewsma).</span><span class="sxs-lookup"><span data-stu-id="ee11a-137">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all room lists](#bk_GetRoomListewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="ee11a-138">Сервер отвечает на запрос [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) с сообщением [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) , содержащий список помещений для вашей организации.</span><span class="sxs-lookup"><span data-stu-id="ee11a-138">The server responds to the [GetRoomLists](http://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) request with a [GetRoomListsResponse](http://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) message that contains the room lists for your organization.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="868" MinorBuildNumber="8" Version="V2_9" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomListsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:RoomLists>
        <t:Address>
          <t:Name>Contoso Building 1 Room List</t:Name>
          <t:EmailAddress>bldg1rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 2 Room List</t:Name>
          <t:EmailAddress>bldg2rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
        <t:Address>
          <t:Name>Contoso Building 3 Room List</t:Name>
          <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
          <t:RoutingType>SMTP</t:RoutingType>
          <t:MailboxType>PublicDL</t:MailboxType>
        </t:Address>
      </m:RoomLists>
    </m:GetRoomListsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a><span data-ttu-id="ee11a-139">Получение всех комнатах в список помещений с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-139">Get all the rooms in a room list by using the EWS Managed API</span></span>
<span data-ttu-id="ee11a-140"><a name="bk_FindRoomewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="ee11a-140"></span></span>

<span data-ttu-id="ee11a-141">Следующем примере показано, как получить коллекцию комнат в список помещений с помощью метода [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ee11a-141">The following example shows how to get a collection of rooms in a room list by using the [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) method.</span></span> 
  
```cs
EmailAddress myRoomList = "bldg3rooms@contoso.com";
// This method call results in a GetRooms call to EWS.
System.Collections.ObjectModel.Collection<EmailAddress> myRoomAddresses = service.GetRooms(myRoomList);
// Display the individual rooms.
foreach (EmailAddress address in myRoomAddresses)
{
    Console.WriteLine("Email Address: {0}", address.Address);
}

```

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a><span data-ttu-id="ee11a-142">Получение всех комнатах в список помещений с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-142">Get all the rooms in a room list by using EWS</span></span>
<span data-ttu-id="ee11a-143"><a name="bk_FindRoomews"> </a></span><span class="sxs-lookup"><span data-stu-id="ee11a-143"></span></span>

<span data-ttu-id="ee11a-144">Следующем примере показано, как получить список [помещений](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) в [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) с помощью операции [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="ee11a-144">The following example shows how to get a list of [rooms](http://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) in a [RoomList](http://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) by using the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="ee11a-145">Это также XML-запрос, который отправляет управляемый API веб-служб Exchange, когда использовать управляемый API EWS для [получения всех комнатах в список помещений](#bk_FindRoomewsma).</span><span class="sxs-lookup"><span data-stu-id="ee11a-145">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all the rooms in a room list](#bk_FindRoomewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>bldg3rooms@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="ee11a-146">Сервер отвечает на запрос [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) с сообщением [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) , содержащая помещения в список помещений.</span><span class="sxs-lookup"><span data-stu-id="ee11a-146">The server responds to the [GetRooms](http://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) request with a [GetRoomsResponse](http://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) message that contains the rooms in the room list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" 
                         Version="V2_9" xmlns:h="http://scemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomsResponse ResponseClass="Success" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                        xmlns:t="http://scemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseCode>NoError</m:ResponseCode>
      <m:Rooms>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/101 (16) AV</t:Name>
            <t:EmailAddress>cf3101@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/102 (8) AV</t:Name>
            <t:EmailAddress>cf3102@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room>
          <t:Id>
            <t:Name>Conf Room 3/103 (14) AV RoundTable</t:Name>
            <t:EmailAddress>cf3103@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </m:GetRoomsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="ee11a-147">См. также</span><span class="sxs-lookup"><span data-stu-id="ee11a-147">See also</span></span>


- [<span data-ttu-id="ee11a-148">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-148">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="ee11a-149">Получение сведений о доступности с помощью веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee11a-149">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="ee11a-150">Создание и управление ими почтовый ящик помещения</span><span class="sxs-lookup"><span data-stu-id="ee11a-150">Create and Manage Room Mailboxes</span></span>](http://technet.microsoft.com/en-us/library/jj215781%28v=exchg.150%29.aspx)
    

