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
description: SetUserOofSettings веб-метода настраивает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика.
ms.openlocfilehash: 51c2f9488f38a4adb0e291c11adc2ebfe3426f25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835469"
---
# <a name="setuseroofsettings-operation"></a><span data-ttu-id="c703a-103">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c703a-103">SetUserOofSettings operation</span></span>

<span data-ttu-id="c703a-104">Веб-метода **SetUserOofSettings** настраивает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c703a-104">The **SetUserOofSettings** Web method sets a mailbox user's Out of Office (OOF) settings and message.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="c703a-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="c703a-105">SOAP Headers</span></span>

<span data-ttu-id="c703a-106">Операция **SetUserOofSettings** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="c703a-106">The **SetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="c703a-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="c703a-107">**Header**</span></span>|<span data-ttu-id="c703a-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c703a-108">**Element**</span></span>|<span data-ttu-id="c703a-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c703a-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c703a-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="c703a-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="c703a-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c703a-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c703a-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="c703a-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="c703a-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="c703a-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="c703a-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c703a-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c703a-115">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="c703a-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="setuseroofsettings-request-example"></a><span data-ttu-id="c703a-116">Пример запроса SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c703a-116">SetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="c703a-117">Описание</span><span class="sxs-lookup"><span data-stu-id="c703a-117">Description</span></span>

<span data-ttu-id="c703a-118">В следующем примере запрос **SetUserOofSettings** задается параметром об отсутствии на работе для 10 дней.</span><span class="sxs-lookup"><span data-stu-id="c703a-118">The following example of a **SetUserOofSettings** request sets an OOF setting for 10 days.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c703a-119">Программа</span><span class="sxs-lookup"><span data-stu-id="c703a-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>User1</Name>
        <Address>user1@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="request-elements"></a><span data-ttu-id="c703a-120">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="c703a-120">Request elements</span></span>

<span data-ttu-id="c703a-121">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c703a-121">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="c703a-122">SetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="c703a-122">SetUserOofSettingsRequest</span></span>](setuseroofsettingsrequest.md)
    
- [<span data-ttu-id="c703a-123">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="c703a-123">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="c703a-124">Имя (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c703a-124">Name (EmailAddress)</span></span>](name-emailaddress.md)
    
- [<span data-ttu-id="c703a-125">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="c703a-125">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="c703a-126">RoutingType (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="c703a-126">RoutingType (EmailAddress)</span></span>](routingtype-emailaddress.md)
    
- [<span data-ttu-id="c703a-127">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c703a-127">UserOofSettings</span></span>](useroofsettings.md)
    
- [<span data-ttu-id="c703a-128">OofState</span><span class="sxs-lookup"><span data-stu-id="c703a-128">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="c703a-129">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="c703a-129">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="c703a-130">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="c703a-130">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="c703a-131">Время начала</span><span class="sxs-lookup"><span data-stu-id="c703a-131">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="c703a-132">Время окончания</span><span class="sxs-lookup"><span data-stu-id="c703a-132">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="c703a-133">InternalReply</span><span class="sxs-lookup"><span data-stu-id="c703a-133">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="c703a-134">Сообщение (доступность)</span><span class="sxs-lookup"><span data-stu-id="c703a-134">Message (Availability)</span></span>](message-availability.md)
    
- [<span data-ttu-id="c703a-135">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="c703a-135">ExternalReply</span></span>](externalreply.md)
    
## <a name="successful-setuseroofsettings-response-example"></a><span data-ttu-id="c703a-136">Пример успешного ответа SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="c703a-136">Successful SetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="c703a-137">Описание</span><span class="sxs-lookup"><span data-stu-id="c703a-137">Description</span></span>

<span data-ttu-id="c703a-138">В следующем примере показано успешного ответа на запрос **SetUserOofSettings** .</span><span class="sxs-lookup"><span data-stu-id="c703a-138">The following example shows a successful response to the **SetUserOofSettings** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="c703a-139">Программа</span><span class="sxs-lookup"><span data-stu-id="c703a-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" /> 
  </soap:Header>
  <soap:Body>
    <SetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode> 
      </ResponseMessage>
    </SetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="c703a-140">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="c703a-140">Successful response elements</span></span>

<span data-ttu-id="c703a-141">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="c703a-141">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="c703a-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c703a-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="c703a-143">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="c703a-143">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md)
    
- [<span data-ttu-id="c703a-144">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c703a-144">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="c703a-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c703a-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="see-also"></a><span data-ttu-id="c703a-146">См. также</span><span class="sxs-lookup"><span data-stu-id="c703a-146">See also</span></span>



- [<span data-ttu-id="c703a-147">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="c703a-147">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

