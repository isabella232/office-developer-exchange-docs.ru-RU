---
title: Операция GetRooms
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRooms
api_type:
- schema
ms.assetid: 5501ddc0-3bfa-4da6-8e15-4223ca5499a3
description: Операция "высвободить" получает комнаты в указанном списке помещений.
ms.openlocfilehash: 4cb124b96637b9fcdca15595faebb2ce4d304de0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460549"
---
# <a name="getrooms-operation"></a><span data-ttu-id="ee36f-103">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="ee36f-103">GetRooms operation</span></span>

<span data-ttu-id="ee36f-104">Операция " **высвободить** " получает комнаты в указанном списке помещений.</span><span class="sxs-lookup"><span data-stu-id="ee36f-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="ee36f-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="ee36f-105">SOAP Headers</span></span>

<span data-ttu-id="ee36f-106">Операция " **высвободить** " может использовать заголовки SOAP, приведенные в следующей таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="ee36f-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="ee36f-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="ee36f-107">**Header**</span></span>|<span data-ttu-id="ee36f-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ee36f-108">**Element**</span></span>|<span data-ttu-id="ee36f-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ee36f-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ee36f-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="ee36f-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="ee36f-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="ee36f-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="ee36f-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="ee36f-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="ee36f-113">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="ee36f-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="ee36f-114">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="ee36f-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="ee36f-115">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="ee36f-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="ee36f-116">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="ee36f-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="ee36f-117">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="ee36f-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="ee36f-118">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="ee36f-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="ee36f-119">серверверсион</span><span class="sxs-lookup"><span data-stu-id="ee36f-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="ee36f-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ee36f-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="ee36f-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="ee36f-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="ee36f-122">Пример запроса на получение помещений</span><span class="sxs-lookup"><span data-stu-id="ee36f-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="ee36f-123">Описание</span><span class="sxs-lookup"><span data-stu-id="ee36f-123">Description</span></span>

<span data-ttu-id="ee36f-124">Ниже приведен **Пример запроса на получение комнат,** которые связаны со списком помещений.</span><span class="sxs-lookup"><span data-stu-id="ee36f-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="ee36f-125">Код</span><span class="sxs-lookup"><span data-stu-id="ee36f-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version ="Exchange2010_SP1"/>
  </soap:Header>
  <soap:Body>
    <m:GetRooms>
      <m:RoomList>
        <t:EmailAddress>RoomList@contoso.com</t:EmailAddress>
      </m:RoomList>
    </m:GetRooms>
  </soap:Body>

```

### <a name="request-elements"></a><span data-ttu-id="ee36f-126">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="ee36f-126">Request elements</span></span>

<span data-ttu-id="ee36f-127">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ee36f-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="ee36f-128">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="ee36f-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="ee36f-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="ee36f-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="ee36f-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="ee36f-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="ee36f-131">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="ee36f-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="ee36f-132">Пример ответа на успешные помещения</span><span class="sxs-lookup"><span data-stu-id="ee36f-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="ee36f-133">Описание</span><span class="sxs-lookup"><span data-stu-id="ee36f-133">Description</span></span>

<span data-ttu-id="ee36f-134">В следующем ответе показаны сведения об адресе электронной почты для комнат, связанных с списком помещений.</span><span class="sxs-lookup"><span data-stu-id="ee36f-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="ee36f-135">Код</span><span class="sxs-lookup"><span data-stu-id="ee36f-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room02</t:Name>
            <t:EmailAddress>Room02@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
      </m:Rooms>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="ee36f-136">Элементы ответа на успешные помещения</span><span class="sxs-lookup"><span data-stu-id="ee36f-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="ee36f-137">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ee36f-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ee36f-138">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ee36f-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ee36f-139">жетрумсреспонсе</span><span class="sxs-lookup"><span data-stu-id="ee36f-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="ee36f-140">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ee36f-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ee36f-141">Комната</span><span class="sxs-lookup"><span data-stu-id="ee36f-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="ee36f-142">Комната</span><span class="sxs-lookup"><span data-stu-id="ee36f-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="ee36f-143">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ee36f-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="ee36f-144">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="ee36f-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="ee36f-145">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="ee36f-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="ee36f-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="ee36f-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="ee36f-147">Пример ответа на сообщение об ошибке при возникновении ошибок</span><span class="sxs-lookup"><span data-stu-id="ee36f-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="ee36f-148">Описание</span><span class="sxs-lookup"><span data-stu-id="ee36f-148">Description</span></span>

<span data-ttu-id="ee36f-149">В следующем примере показан ответ об ошибке, вызванный попыткой получения сведений о помещении для несуществующего списка помещений.</span><span class="sxs-lookup"><span data-stu-id="ee36f-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="ee36f-150">Код</span><span class="sxs-lookup"><span data-stu-id="ee36f-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="ee36f-151">Элементы ответа с ошибками во всех местах</span><span class="sxs-lookup"><span data-stu-id="ee36f-151">GetRooms Error response elements</span></span>

<span data-ttu-id="ee36f-152">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ee36f-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="ee36f-153">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="ee36f-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="ee36f-154">жетрумсреспонсе</span><span class="sxs-lookup"><span data-stu-id="ee36f-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="ee36f-155">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="ee36f-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="ee36f-156">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="ee36f-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="ee36f-157">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="ee36f-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="ee36f-158">См. также</span><span class="sxs-lookup"><span data-stu-id="ee36f-158">See also</span></span>

- [<span data-ttu-id="ee36f-159">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee36f-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="ee36f-160">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="ee36f-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

