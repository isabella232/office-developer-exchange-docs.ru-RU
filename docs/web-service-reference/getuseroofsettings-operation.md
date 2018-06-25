---
title: Операция GetUserOofSettings
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserOofSettings
api_type:
- schema
ms.assetid: 153e4440-495b-4972-9811-2fbea740142a
description: Операция GetUserOofSettings получает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика.
ms.openlocfilehash: 75a734999842cc33c213e02dc114f23372ae51fd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833691"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="3d33d-103">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="3d33d-104">Операция **GetUserOofSettings** получает параметры об отсутствии на работе Office (OOF) и сообщения пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="3d33d-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="3d33d-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="3d33d-105">SOAP Headers</span></span>

<span data-ttu-id="3d33d-106">Операция **GetUserOofSettings** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="3d33d-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="3d33d-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="3d33d-107">**Header**</span></span>|<span data-ttu-id="3d33d-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d33d-108">**Element**</span></span>|<span data-ttu-id="3d33d-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d33d-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3d33d-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="3d33d-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="3d33d-111">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3d33d-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3d33d-112">Идентифицирует пользователя, которого олицетворения в клиентском приложении.</span><span class="sxs-lookup"><span data-stu-id="3d33d-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="3d33d-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="3d33d-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="3d33d-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3d33d-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3d33d-115">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="3d33d-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="3d33d-116">С помощью операции GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="3d33d-117">Операция **GetUserOofSettings** предоставляет доступ к параметрам пользователя об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="3d33d-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="3d33d-118">Пользователь идентифицируется адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d33d-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="3d33d-119">Если сообщение об отсутствии на работе имеет значение null и об отсутствии на работе этот параметр включен, сообщения об отсутствии на работе не отправляются.</span><span class="sxs-lookup"><span data-stu-id="3d33d-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="3d33d-120">Если сообщений об отсутствии на работе с MicrosoftOfficeOutlook, эта операция возвращает сообщения об отсутствии на работе в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="3d33d-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="3d33d-121">Пример запроса GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="3d33d-122">Описание</span><span class="sxs-lookup"><span data-stu-id="3d33d-122">Description</span></span>

<span data-ttu-id="3d33d-123">В следующем примере показано **GetUserOofSettings** запрос, который получает сведения об отсутствии на работе одного пользователя.</span><span class="sxs-lookup"><span data-stu-id="3d33d-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="3d33d-124">Программа</span><span class="sxs-lookup"><span data-stu-id="3d33d-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="http://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="3d33d-125">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="3d33d-125">Request elements</span></span>

<span data-ttu-id="3d33d-126">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3d33d-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="3d33d-127">GetUserOofSettingsRequest</span><span class="sxs-lookup"><span data-stu-id="3d33d-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="3d33d-128">Почтовый ящик (доступность)</span><span class="sxs-lookup"><span data-stu-id="3d33d-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="3d33d-129">Адрес (строка)</span><span class="sxs-lookup"><span data-stu-id="3d33d-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="3d33d-130">Пример успешного ответа GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="3d33d-131">Описание</span><span class="sxs-lookup"><span data-stu-id="3d33d-131">Description</span></span>

<span data-ttu-id="3d33d-132">В следующем примере показано отключенном состоянии об отсутствии на работе с сообщениями об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="3d33d-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="3d33d-133">Программа</span><span class="sxs-lookup"><span data-stu-id="3d33d-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Disabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2006-11-03T23:00:00</StartTime>
          <EndTime>2006-11-04T23:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office. This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
      </OofSettings>
      <AllowExternalOof>All</AllowExternalOof>
    </GetUserOofSettingsResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="3d33d-134">Элементы ответов успешно GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="3d33d-135">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3d33d-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="3d33d-136">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3d33d-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="3d33d-137">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3d33d-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="3d33d-138">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3d33d-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="3d33d-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3d33d-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3d33d-140">OofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="3d33d-141">OofState</span><span class="sxs-lookup"><span data-stu-id="3d33d-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="3d33d-142">ExternalAudience</span><span class="sxs-lookup"><span data-stu-id="3d33d-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="3d33d-143">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="3d33d-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="3d33d-144">Время начала</span><span class="sxs-lookup"><span data-stu-id="3d33d-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="3d33d-145">Время окончания</span><span class="sxs-lookup"><span data-stu-id="3d33d-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="3d33d-146">InternalReply</span><span class="sxs-lookup"><span data-stu-id="3d33d-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="3d33d-147">ExternalReply</span><span class="sxs-lookup"><span data-stu-id="3d33d-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="3d33d-148">Message</span><span class="sxs-lookup"><span data-stu-id="3d33d-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="3d33d-149">AllowExternalOof</span><span class="sxs-lookup"><span data-stu-id="3d33d-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="3d33d-150">Пример ответа об ошибке GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="3d33d-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="3d33d-151">Описание</span><span class="sxs-lookup"><span data-stu-id="3d33d-151">Description</span></span>

<span data-ttu-id="3d33d-152">В следующем примере показано возврату ошибки, возникающие при попытке обращения к другому пользователю сведения об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="3d33d-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="3d33d-153">Программа</span><span class="sxs-lookup"><span data-stu-id="3d33d-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="3d33d-154">См. также</span><span class="sxs-lookup"><span data-stu-id="3d33d-154">See also</span></span>



- [<span data-ttu-id="3d33d-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d33d-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

