---
title: Операция SetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SetUserOofSettings
api_type:
- schema
ms.assetid: 36277ef0-18ee-4b35-9e6e-8c321d8f5433
description: Веб-метод SetUserOofSettings устанавливает параметры и сообщение "нет на месте" для пользователя почтового ящика.
ms.openlocfilehash: 88b5475dd2f0fe6d334bad51a0fe8d0beb767634
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463155"
---
# <a name="setuseroofsettings-operation"></a><span data-ttu-id="a1aa1-103">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a1aa1-103">SetUserOofSettings operation</span></span>

<span data-ttu-id="a1aa1-104">Веб-метод **SetUserOofSettings** устанавливает параметры и сообщение "нет на месте" для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-104">The **SetUserOofSettings** Web method sets a mailbox user's Out of Office (OOF) settings and message.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="a1aa1-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="a1aa1-105">SOAP Headers</span></span>

<span data-ttu-id="a1aa1-106">Операция **SetUserOofSettings** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-106">The **SetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a1aa1-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="a1aa1-107">**Header**</span></span>|<span data-ttu-id="a1aa1-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1aa1-108">**Element**</span></span>|<span data-ttu-id="a1aa1-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1aa1-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a1aa1-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="a1aa1-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="a1aa1-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="a1aa1-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a1aa1-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="a1aa1-113">серверверсион</span><span class="sxs-lookup"><span data-stu-id="a1aa1-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a1aa1-114">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a1aa1-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a1aa1-115">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="setuseroofsettings-request-example"></a><span data-ttu-id="a1aa1-116">Пример запроса SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a1aa1-116">SetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="a1aa1-117">Описание</span><span class="sxs-lookup"><span data-stu-id="a1aa1-117">Description</span></span>

<span data-ttu-id="a1aa1-118">В следующем примере запроса **SetUserOofSettings** задается значение параметра "отсутствие на работе" в течение 10 дней.</span><span class="sxs-lookup"><span data-stu-id="a1aa1-118">The following example of a **SetUserOofSettings** request sets an OOF setting for 10 days.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a1aa1-119">Код</span><span class="sxs-lookup"><span data-stu-id="a1aa1-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-10-05T00:00:00</StartTime>
          <EndTime>2006-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="a1aa1-120">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="a1aa1-120">Request elements</span></span>

<span data-ttu-id="a1aa1-121">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a1aa1-121">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="a1aa1-122">сетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="a1aa1-122">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
    
- [<span data-ttu-id="a1aa1-123">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-123">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="a1aa1-124">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-124">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="a1aa1-125">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-125">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="a1aa1-126">Раутингтипе (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-126">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="a1aa1-127">усеруфсеттингс</span><span class="sxs-lookup"><span data-stu-id="a1aa1-127">UserOofSettings</span></span>](useroofsettings.md)
    
- [<span data-ttu-id="a1aa1-128">уфстате</span><span class="sxs-lookup"><span data-stu-id="a1aa1-128">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="a1aa1-129">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="a1aa1-129">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="a1aa1-130">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-130">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="a1aa1-131">StartTime</span><span class="sxs-lookup"><span data-stu-id="a1aa1-131">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="a1aa1-132">EndTime</span><span class="sxs-lookup"><span data-stu-id="a1aa1-132">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="a1aa1-133">интерналрепли</span><span class="sxs-lookup"><span data-stu-id="a1aa1-133">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="a1aa1-134">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="a1aa1-134">Message (Availability)</span></span>](message-availability.md)
    
- [<span data-ttu-id="a1aa1-135">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="a1aa1-135">ExternalReply</span></span>](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a><span data-ttu-id="a1aa1-136">Пример успешного ответа SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="a1aa1-136">Successful SetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="a1aa1-137">Описание</span><span class="sxs-lookup"><span data-stu-id="a1aa1-137">Description</span></span>

<span data-ttu-id="a1aa1-138">В следующем примере показан успешный ответ на запрос **SetUserOofSettings** .</span><span class="sxs-lookup"><span data-stu-id="a1aa1-138">The following example shows a successful response to the **SetUserOofSettings** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="a1aa1-139">Код</span><span class="sxs-lookup"><span data-stu-id="a1aa1-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="a1aa1-140">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="a1aa1-140">Successful response elements</span></span>

<span data-ttu-id="a1aa1-141">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="a1aa1-141">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="a1aa1-142">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="a1aa1-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="a1aa1-143">сетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1aa1-143">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md)
    
- [<span data-ttu-id="a1aa1-144">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="a1aa1-144">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="a1aa1-145">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="a1aa1-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="a1aa1-146">См. также</span><span class="sxs-lookup"><span data-stu-id="a1aa1-146">See also</span></span>



- [<span data-ttu-id="a1aa1-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="a1aa1-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

