---
title: Получение списков помещений с помощью EWS в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 15980e4a-e41c-4194-829a-cadbdf365bf1
description: Узнайте, как получить список всех списков помещений в организации или список из одного комнаты на сервере Exchange с помощью управляемого API EWS или EWS.
localization_priority: Priority
ms.openlocfilehash: 7c571b0550f861552cdbe8c5b30138101c9fc788
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455795"
---
# <a name="get-room-lists-by-using-ews-in-exchange"></a><span data-ttu-id="e66e9-103">Получение списков помещений с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e66e9-103">Get room lists by using EWS in Exchange</span></span>

<span data-ttu-id="e66e9-104">Узнайте, как получить список всех списков помещений в организации или список из одного комнаты на сервере Exchange с помощью управляемого API EWS или EWS.</span><span class="sxs-lookup"><span data-stu-id="e66e9-104">Learn how to get a list of all the room lists in your organization or a single room list from an Exchange server by using the EWS Managed API or EWS.</span></span>
  
<span data-ttu-id="e66e9-105">Вы можете использовать управляемый API EWS или EWS для получения сведений о комнатах и о том, как комнаты группируются в Организации.</span><span class="sxs-lookup"><span data-stu-id="e66e9-105">You can use the EWS Managed API or EWS to get information about rooms and how the rooms are grouped in your organization.</span></span> <span data-ttu-id="e66e9-106">По умолчанию списки помещений не существуют; Администратор должен создать и упорядочить их.</span><span class="sxs-lookup"><span data-stu-id="e66e9-106">Room lists don't exist by default; your administrator needs to create and organize them.</span></span> <span data-ttu-id="e66e9-107">Как правило, они организованы по расположению или Отделу, как показано в следующем примере.</span><span class="sxs-lookup"><span data-stu-id="e66e9-107">Typically, they're organized by location or department, as shown in the following example.</span></span>
  
<span data-ttu-id="e66e9-108">**Имена и адреса электронной почты в списке помещений contoso**</span><span class="sxs-lookup"><span data-stu-id="e66e9-108">**Contoso room list names and email addresses**</span></span>

|<span data-ttu-id="e66e9-109">**Имя списка помещений**</span><span class="sxs-lookup"><span data-stu-id="e66e9-109">**Name of room list**</span></span>|<span data-ttu-id="e66e9-110">**Адрес электронной почты списка помещений**</span><span class="sxs-lookup"><span data-stu-id="e66e9-110">**Email address of room list**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e66e9-111">Создание списка с 11 комнатами</span><span class="sxs-lookup"><span data-stu-id="e66e9-111">Building 11 room list</span></span>  <br/> |<span data-ttu-id="e66e9-112">Bldg11rooms@contoso.com</span><span class="sxs-lookup"><span data-stu-id="e66e9-112">Bldg11rooms@contoso.com</span></span>  <br/> |
|<span data-ttu-id="e66e9-113">Список конференц-зала здания по охране здания</span><span class="sxs-lookup"><span data-stu-id="e66e9-113">Health Science Building Conference Room List</span></span>  <br/> |<span data-ttu-id="e66e9-114">HSbldgrooms@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="e66e9-114">HSbldgrooms@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="e66e9-115">Комнаты для собраний для бухгалтерского учета</span><span class="sxs-lookup"><span data-stu-id="e66e9-115">Accounting Floor Meeting Rooms</span></span>  <br/> |<span data-ttu-id="e66e9-116">Acctfloor300@contoso.com</span><span class="sxs-lookup"><span data-stu-id="e66e9-116">Acctfloor300@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="e66e9-117">Каждая комната в списке помещений имеет имя и адрес электронной почты, связанные с ним.</span><span class="sxs-lookup"><span data-stu-id="e66e9-117">Each room in a room list has a name and email address associated with it.</span></span>
  
<span data-ttu-id="e66e9-118">**Имена комнат Contoso и адреса электронной почты**</span><span class="sxs-lookup"><span data-stu-id="e66e9-118">**Contoso room names and email addresses**</span></span>

|<span data-ttu-id="e66e9-119">**Имя комнаты**</span><span class="sxs-lookup"><span data-stu-id="e66e9-119">**Name of room**</span></span>|<span data-ttu-id="e66e9-120">**Адрес электронной почты комнаты**</span><span class="sxs-lookup"><span data-stu-id="e66e9-120">**Email address of room**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e66e9-121">Conf комната 11/101 (8) AV</span><span class="sxs-lookup"><span data-stu-id="e66e9-121">Conf Room 11/101 (8) AV</span></span>  <br/> |<span data-ttu-id="e66e9-122">Cf11101@contoso.com</span><span class="sxs-lookup"><span data-stu-id="e66e9-122">Cf11101@contoso.com</span></span>  <br/> |
|<span data-ttu-id="e66e9-123">Демонстрационная лаборатория HS (100)</span><span class="sxs-lookup"><span data-stu-id="e66e9-123">HS Demonstration Lab (100)</span></span>  <br/> |<span data-ttu-id="e66e9-124">Hs101@contoso.edu</span><span class="sxs-lookup"><span data-stu-id="e66e9-124">Hs101@contoso.edu</span></span>  <br/> |
|<span data-ttu-id="e66e9-125">Учет 305 Интернете</span><span class="sxs-lookup"><span data-stu-id="e66e9-125">Accounting 305 WB</span></span>  <br/> |<span data-ttu-id="e66e9-126">Acct305@contoso.com</span><span class="sxs-lookup"><span data-stu-id="e66e9-126">Acct305@contoso.com</span></span>  <br/> |
   
<span data-ttu-id="e66e9-127">Список, содержащий все списки помещений, можно получить с помощью метода [ExchangeService. GetRoomLists](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS или из операции [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS.</span><span class="sxs-lookup"><span data-stu-id="e66e9-127">You can get a list that contains all room lists by using either the [ExchangeService.GetRoomLists](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getroomlists%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) EWS operation.</span></span> 
  
<span data-ttu-id="e66e9-128">Вы можете получить список из одного комнаты, который содержит все комнаты для расположения или отдела, указав его адрес электронной почты с помощью метода управления веб-служб "веб-служб Exchange" или " [кабинеты](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) [EWS".](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="e66e9-128">You can retrieve a single room list that contains all the rooms for a location or department by supplying its email address by using the [GetRooms](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getrooms%28v=exchg.80%29.aspx) EWS Managed API method or the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) EWS operation.</span></span> <span data-ttu-id="e66e9-129">При наличии коллекции комнат, связанных со списком помещений, можно выполнить поиск по коллекции, чтобы определить требуемые комнаты или комнаты, по адресу электронной почты или с помощью поиска ключевых слов в имени, например "AV" или "Lab".</span><span class="sxs-lookup"><span data-stu-id="e66e9-129">When you have a collection of rooms associated with a room list, you can then search through the collection to identify the room or rooms you want, either by email address, or by looking for key words in the name, such as "AV", or "Lab".</span></span> 
  
## <a name="get-all-room-lists-by-using-the-ews-managed-api"></a><span data-ttu-id="e66e9-130">Получение всех списков помещений с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e66e9-130">Get all room lists by using the EWS Managed API</span></span>
<span data-ttu-id="e66e9-131"><a name="bk_GetRoomListewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e66e9-131"><a name="bk_GetRoomListewsma"> </a></span></span>

<span data-ttu-id="e66e9-132">В приведенном ниже примере показано, как получить список, содержащий все списки помещений в Организации, с помощью метода [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e66e9-132">The following example shows how to get a list that contains all the room lists in your organization by using the [GetRoomLists](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRoomLists.aspx) method.</span></span> 
  
<span data-ttu-id="e66e9-133">В этом примере предполагается, что вы прошли проверку подлинности на сервере Exchange и приобрели объект [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) с именем **Service**.</span><span class="sxs-lookup"><span data-stu-id="e66e9-133">This example assumes that you have authenticated to an Exchange server and have acquired an [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object named **service**.</span></span> 
  
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

## <a name="get-all-room-lists-by-using-ews"></a><span data-ttu-id="e66e9-134">Получение всех списков помещений с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e66e9-134">Get all room lists by using EWS</span></span>
<span data-ttu-id="e66e9-135"><a name="bk_GetRoomListews"> </a></span><span class="sxs-lookup"><span data-stu-id="e66e9-135"><a name="bk_GetRoomListews"> </a></span></span>

<span data-ttu-id="e66e9-136">В приведенном ниже примере показано, как получить коллекцию всех [румлистс](https://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) Организации с помощью операции [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e66e9-136">The following example shows how to get a collection of all your organization's [RoomLists](https://msdn.microsoft.com/library/2b190823-b11e-4635-97e4-3aba5865fd05%28Office.15%29.aspx) by using the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="e66e9-137">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS для [получения всех списков помещений](#bk_GetRoomListewsma).</span><span class="sxs-lookup"><span data-stu-id="e66e9-137">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all room lists](#bk_GetRoomListewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetRoomLists />
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="e66e9-138">Сервер отвечает на запрос [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) с сообщением [жетрумлистсреспонсе](https://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) , которое содержит списки помещений для Организации.</span><span class="sxs-lookup"><span data-stu-id="e66e9-138">The server responds to the [GetRoomLists](https://msdn.microsoft.com/library/55d451f9-547f-44ac-872e-9cb220ea7b7c%28Office.15%29.aspx) request with a [GetRoomListsResponse](https://msdn.microsoft.com/library/8c736f68-1026-496a-b12f-c169c078abd0%28Office.15%29.aspx) message that contains the room lists for your organization.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="868" MinorBuildNumber="8" Version="V2_9" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomListsResponse ResponseClass="Success" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="get-all-the-rooms-in-a-room-list-by-using-the-ews-managed-api"></a><span data-ttu-id="e66e9-139">Получение всех комнат в списке помещений с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="e66e9-139">Get all the rooms in a room list by using the EWS Managed API</span></span>
<span data-ttu-id="e66e9-140"><a name="bk_FindRoomewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="e66e9-140"><a name="bk_FindRoomewsma"> </a></span></span>

<span data-ttu-id="e66e9-141">В приведенном ниже примере показано, как получить коллекцию комнат в списке помещений с помощью метода [Rooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) .</span><span class="sxs-lookup"><span data-stu-id="e66e9-141">The following example shows how to get a collection of rooms in a room list by using the [GetRooms](https://msdn.microsoft.com/library/Microsoft.Exchange.WebServices.Data.ExchangeService.GetRooms.aspx) method.</span></span> 
  
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

## <a name="get-all-the-rooms-in-a-room-list-by-using-ews"></a><span data-ttu-id="e66e9-142">Получение всех комнат в списке помещений с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="e66e9-142">Get all the rooms in a room list by using EWS</span></span>
<span data-ttu-id="e66e9-143"><a name="bk_FindRoomews"> </a></span><span class="sxs-lookup"><span data-stu-id="e66e9-143"><a name="bk_FindRoomews"> </a></span></span>

<span data-ttu-id="e66e9-144">В приведенном ниже примере показано, как получить список [комнат](https://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) в [RoomList принимают одиночные](https://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) с помощью операции " [высвободить](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) ".</span><span class="sxs-lookup"><span data-stu-id="e66e9-144">The following example shows how to get a list of [rooms](https://msdn.microsoft.com/library/57b6079a-3d83-4429-861e-c551e9e1a991%28Office.15%29.aspx) in a [RoomList](https://msdn.microsoft.com/library/cb02bdf0-df9f-4e31-b7dd-cd9f2f2cc2b2%28Office.15%29.aspx) by using the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="e66e9-145">Это также запрос XML, который отправляет управляемый API EWS, когда вы используете управляемый API EWS, чтобы [получить все комнаты в списке помещений](#bk_FindRoomewsma).</span><span class="sxs-lookup"><span data-stu-id="e66e9-145">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [get all the rooms in a room list](#bk_FindRoomewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="e66e9-146">Сервер отвечает на запрос [жетрумсреспонсе](https://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) с сообщением [о помещении,](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) которое содержит комнаты в списке помещений.</span><span class="sxs-lookup"><span data-stu-id="e66e9-146">The server responds to the [GetRooms](https://msdn.microsoft.com/library/5501ddc0-3bfa-4da6-8e15-4223ca5499a3%28Office.15%29.aspx) request with a [GetRoomsResponse](https://msdn.microsoft.com/library/a8c85f65-bb63-4e7a-b0ca-7c9a04560a58%28Office.15%29.aspx) message that contains the rooms in the room list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="873" MinorBuildNumber="9" 
                         Version="V2_9" xmlns:h="http://scemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetRoomsResponse ResponseClass="Success" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
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

## <a name="see-also"></a><span data-ttu-id="e66e9-147">См. также</span><span class="sxs-lookup"><span data-stu-id="e66e9-147">See also</span></span>


- [<span data-ttu-id="e66e9-148">Календари и веб-службах Exchange</span><span class="sxs-lookup"><span data-stu-id="e66e9-148">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    
- [<span data-ttu-id="e66e9-149">Получение сведений о доступности с помощью EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e66e9-149">Get free/busy information by using EWS in Exchange</span></span>](how-to-get-free-busy-information-by-using-ews-in-exchange.md)
    
- [<span data-ttu-id="e66e9-150">Создание почтовых ящиков помещения и управление ими</span><span class="sxs-lookup"><span data-stu-id="e66e9-150">Create and Manage Room Mailboxes</span></span>](https://technet.microsoft.com/library/jj215781%28v=exchg.150%29.aspx)
    

