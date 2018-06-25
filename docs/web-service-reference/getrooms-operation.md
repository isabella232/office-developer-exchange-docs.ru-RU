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
description: Операция GetRooms получает комнат в список помещений указанного.
ms.openlocfilehash: 3718c476881ae8aa538646464e7c61845d849562
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762908"
---
# <a name="getrooms-operation"></a><span data-ttu-id="a095c-103">Операция GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-103">GetRooms operation</span></span>

<span data-ttu-id="a095c-104">Операция **GetRooms** получает комнат в список помещений указанного.</span><span class="sxs-lookup"><span data-stu-id="a095c-104">The **GetRooms** operation gets the rooms within the specified room list.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="a095c-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="a095c-105">SOAP Headers</span></span>

<span data-ttu-id="a095c-106">Операция **GetRooms** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a095c-106">The **GetRooms** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a095c-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="a095c-107">**Header**</span></span>|<span data-ttu-id="a095c-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a095c-108">**Element**</span></span>|<span data-ttu-id="a095c-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a095c-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a095c-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="a095c-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="a095c-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a095c-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a095c-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="a095c-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="a095c-113">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a095c-113">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="a095c-114">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a095c-114">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a095c-115">Идентифицирует культуры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="a095c-115">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a095c-116">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="a095c-116">RequestVersion</span></span>  <br/> |[<span data-ttu-id="a095c-117">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a095c-117">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a095c-118">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="a095c-118">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="a095c-119">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="a095c-119">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a095c-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a095c-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a095c-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="a095c-121">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getrooms-request-example"></a><span data-ttu-id="a095c-122">Пример запроса GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-122">GetRooms request example</span></span>

### <a name="description"></a><span data-ttu-id="a095c-123">Описание</span><span class="sxs-lookup"><span data-stu-id="a095c-123">Description</span></span>

<span data-ttu-id="a095c-124">Ниже приведен пример **GetRooms** запрос, который получает комнат, связанных с почтового ящика помещения.</span><span class="sxs-lookup"><span data-stu-id="a095c-124">The following is an example of a **GetRooms** request that gets the rooms that are associated with a room list.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a095c-125">Программа</span><span class="sxs-lookup"><span data-stu-id="a095c-125">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="request-elements"></a><span data-ttu-id="a095c-126">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="a095c-126">Request elements</span></span>

<span data-ttu-id="a095c-127">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a095c-127">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a095c-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a095c-128">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="a095c-129">GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-129">GetRooms</span></span>](getrooms.md)
    
- [<span data-ttu-id="a095c-130">RoomList</span><span class="sxs-lookup"><span data-stu-id="a095c-130">RoomList</span></span>](roomlist.md)
    
- [<span data-ttu-id="a095c-131">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a095c-131">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
## <a name="successful-getrooms-response-example"></a><span data-ttu-id="a095c-132">Пример успешного ответа GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-132">Successful GetRooms response example</span></span>

### <a name="description"></a><span data-ttu-id="a095c-133">Описание</span><span class="sxs-lookup"><span data-stu-id="a095c-133">Description</span></span>

<span data-ttu-id="a095c-134">Приведенный ниже ответ показывает информации адреса электронной почты для комнат, связанных с список помещений.</span><span class="sxs-lookup"><span data-stu-id="a095c-134">The following response shows the email address information for the rooms that are associated with the room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="a095c-135">Программа</span><span class="sxs-lookup"><span data-stu-id="a095c-135">Code</span></span>

```xml
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Success" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <m:Rooms xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:Id>
            <t:Name>Room01</t:Name>
            <t:EmailAddress>Room01@contoso.com</t:EmailAddress>
            <t:RoutingType>SMTP</t:RoutingType>
            <t:MailboxType>Mailbox</t:MailboxType>
          </t:Id>
        </t:Room>
        <t:Room xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="successful-getrooms-response-elements"></a><span data-ttu-id="a095c-136">Элементы ответов успешно GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-136">Successful GetRooms response elements</span></span>

<span data-ttu-id="a095c-137">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a095c-137">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a095c-138">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a095c-138">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a095c-139">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="a095c-139">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="a095c-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a095c-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a095c-141">Комнат</span><span class="sxs-lookup"><span data-stu-id="a095c-141">Rooms</span></span>](rooms.md)
    
- [<span data-ttu-id="a095c-142">Комнаты</span><span class="sxs-lookup"><span data-stu-id="a095c-142">Room</span></span>](room.md)
    
- [<span data-ttu-id="a095c-143">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a095c-143">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="a095c-144">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="a095c-144">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="a095c-145">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a095c-145">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="a095c-146">MailboxType</span><span class="sxs-lookup"><span data-stu-id="a095c-146">MailboxType</span></span>](mailboxtype.md)
    
## <a name="getrooms-error-response-example"></a><span data-ttu-id="a095c-147">Пример ответа об ошибке GetRooms</span><span class="sxs-lookup"><span data-stu-id="a095c-147">GetRooms Error response example</span></span>

### <a name="description"></a><span data-ttu-id="a095c-148">Описание</span><span class="sxs-lookup"><span data-stu-id="a095c-148">Description</span></span>

<span data-ttu-id="a095c-149">В следующем примере показано возврату ошибки, возникающие при попытке получить сведения о комнаты для почтового ящика несуществующий помещения.</span><span class="sxs-lookup"><span data-stu-id="a095c-149">The following example shows an error response caused by an attempt to get room information for a nonexistent room list.</span></span>
  
### <a name="code"></a><span data-ttu-id="a095c-150">Программа</span><span class="sxs-lookup"><span data-stu-id="a095c-150">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" MinorVersion="1" MajorBuildNumber="164" MinorBuildNumber="0" Version="Exchange2010_SP1" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRoomsResponse ResponseClass="Error" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>No results were found.</MessageText>
      <ResponseCode>ErrorNameResolutionNoResults</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRoomsResponse>
  </s:Body>
</s:Envelope>
```

### <a name="getrooms-error-response-elements"></a><span data-ttu-id="a095c-151">Ошибка GetRooms элементы ответа</span><span class="sxs-lookup"><span data-stu-id="a095c-151">GetRooms Error response elements</span></span>

<span data-ttu-id="a095c-152">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a095c-152">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a095c-153">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a095c-153">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a095c-154">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="a095c-154">GetRoomsResponse</span></span>](getroomsresponse.md)
    
- [<span data-ttu-id="a095c-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="a095c-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="a095c-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a095c-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a095c-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a095c-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="a095c-158">См. также</span><span class="sxs-lookup"><span data-stu-id="a095c-158">See also</span></span>

- [<span data-ttu-id="a095c-159">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="a095c-159">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="a095c-160">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a095c-160">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

