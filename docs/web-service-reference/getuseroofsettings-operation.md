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
description: Операция GetUserOofSettings Возвращает параметры и сообщения пользователя почтового ящика "нет на месте" (отсутствие на работе).
ms.openlocfilehash: 622faa622b0ea231a6331ff62631885d4252c1f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457699"
---
# <a name="getuseroofsettings-operation"></a><span data-ttu-id="6135c-103">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-103">GetUserOofSettings operation</span></span>

<span data-ttu-id="6135c-104">Операция **GetUserOofSettings** Возвращает параметры и сообщения пользователя почтового ящика "нет на месте" (отсутствие на работе).</span><span class="sxs-lookup"><span data-stu-id="6135c-104">The **GetUserOofSettings** operation gets a mailbox user's Out of Office (OOF) settings and messages.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="6135c-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="6135c-105">SOAP Headers</span></span>

<span data-ttu-id="6135c-106">Операция **GetUserOofSettings** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="6135c-106">The **GetUserOofSettings** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="6135c-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="6135c-107">**Header**</span></span>|<span data-ttu-id="6135c-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6135c-108">**Element**</span></span>|<span data-ttu-id="6135c-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6135c-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6135c-110">Олицетворение</span><span class="sxs-lookup"><span data-stu-id="6135c-110">Impersonation</span></span>  <br/> |[<span data-ttu-id="6135c-111">ексчанжеимперсонатион</span><span class="sxs-lookup"><span data-stu-id="6135c-111">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="6135c-112">Идентифицирует пользователя, который олицетворяет клиентское приложение.</span><span class="sxs-lookup"><span data-stu-id="6135c-112">Identifies the user whom the client application is impersonating.</span></span>  <br/> |
|<span data-ttu-id="6135c-113">серверверсион</span><span class="sxs-lookup"><span data-stu-id="6135c-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="6135c-114">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6135c-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6135c-115">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="6135c-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="using-the-getuseroofsettings-operation"></a><span data-ttu-id="6135c-116">Использование операции GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-116">Using the GetUserOofSettings Operation</span></span>

<span data-ttu-id="6135c-117">Операция **GetUserOofSettings** предоставляет доступ к параметрам отсутствия на работе пользователя.</span><span class="sxs-lookup"><span data-stu-id="6135c-117">The **GetUserOofSettings** operation provides access to a user's OOF settings.</span></span> <span data-ttu-id="6135c-118">Пользователь идентифицируется по адресу электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="6135c-118">A user is identified by the user's email address.</span></span> <span data-ttu-id="6135c-119">Если сообщение об отсутствии на работе имеет значение NULL и включено отсутствие на работе, сообщение об отсутствии на месте не отправляется.</span><span class="sxs-lookup"><span data-stu-id="6135c-119">If the OOF message is null and OOF is enabled, no OOF message is sent.</span></span> 
  
> [!IMPORTANT]
> <span data-ttu-id="6135c-120">Если сообщения об отсутствии на работе задаются Майкрософтofficeoutlook, эта операция возвратит сообщения об отсутствии на работе в формате HTML.</span><span class="sxs-lookup"><span data-stu-id="6135c-120">If the OOF messages are set by MicrosoftOfficeOutlook, this operation will return the OOF messages in HTML format.</span></span> 
  
## <a name="getuseroofsettings-request-example"></a><span data-ttu-id="6135c-121">Пример запроса GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-121">GetUserOofSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="6135c-122">Description</span><span class="sxs-lookup"><span data-stu-id="6135c-122">Description</span></span>

<span data-ttu-id="6135c-123">В приведенном ниже примере показан запрос **GetUserOofSettings** , который получает сведения об отсутствии на работе отдельных пользователей.</span><span class="sxs-lookup"><span data-stu-id="6135c-123">The following example shows a **GetUserOofSettings** request that gets a single user's OOF information.</span></span> 
  
### <a name="code"></a><span data-ttu-id="6135c-124">Код</span><span class="sxs-lookup"><span data-stu-id="6135c-124">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns ="https://schemas.microsoft.com/exchange/services/2006/types">
        <Address>User1@example.com</Address>
      </Mailbox>
    </GetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="6135c-125">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="6135c-125">Request elements</span></span>

<span data-ttu-id="6135c-126">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6135c-126">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="6135c-127">жетусеруфсеттингсрекуест</span><span class="sxs-lookup"><span data-stu-id="6135c-127">GetUserOofSettingsRequest</span></span>](getuseroofsettingsrequest.md)
    
- [<span data-ttu-id="6135c-128">Mailbox (доступность)</span><span class="sxs-lookup"><span data-stu-id="6135c-128">Mailbox (Availability)</span></span>](mailbox-availability.md)
    
- [<span data-ttu-id="6135c-129">Address (строка)</span><span class="sxs-lookup"><span data-stu-id="6135c-129">Address (string)</span></span>](address-string.md)
    
## <a name="successful-getuseroofsettings-response-example"></a><span data-ttu-id="6135c-130">Пример успешного ответа GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-130">Successful GetUserOofSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="6135c-131">Description</span><span class="sxs-lookup"><span data-stu-id="6135c-131">Description</span></span>

<span data-ttu-id="6135c-132">В следующем примере показано отключенное состояние отсутствия на работе с сообщениями об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="6135c-132">The following example shows a disabled OOF state with the OOF messages.</span></span>
  
### <a name="code"></a><span data-ttu-id="6135c-133">Код</span><span class="sxs-lookup"><span data-stu-id="6135c-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetUserOofSettingsResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseMessage ResponseClass="Success">
        <ResponseCode>NoError</ResponseCode>
      </ResponseMessage>
      <OofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="successful-getuseroofsettings-response-elements"></a><span data-ttu-id="6135c-134">Успешные элементы ответа GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-134">Successful GetUserOofSettings response elements</span></span>

<span data-ttu-id="6135c-135">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6135c-135">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="6135c-136">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="6135c-136">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="6135c-137">жетусеруфсеттингсреспонсе</span><span class="sxs-lookup"><span data-stu-id="6135c-137">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md)
    
- [<span data-ttu-id="6135c-138">респонсемессаже</span><span class="sxs-lookup"><span data-stu-id="6135c-138">ResponseMessage</span></span>](responsemessage.md)
    
- [<span data-ttu-id="6135c-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="6135c-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6135c-140">уфсеттингс</span><span class="sxs-lookup"><span data-stu-id="6135c-140">OofSettings</span></span>](oofsettings.md)
    
- [<span data-ttu-id="6135c-141">уфстате</span><span class="sxs-lookup"><span data-stu-id="6135c-141">OofState</span></span>](oofstate.md)
    
- [<span data-ttu-id="6135c-142">екстерналаудиенце</span><span class="sxs-lookup"><span data-stu-id="6135c-142">ExternalAudience</span></span>](externalaudience.md)
    
- [<span data-ttu-id="6135c-143">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="6135c-143">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md)
    
- [<span data-ttu-id="6135c-144">StartTime</span><span class="sxs-lookup"><span data-stu-id="6135c-144">StartTime</span></span>](starttime.md)
    
- [<span data-ttu-id="6135c-145">EndTime</span><span class="sxs-lookup"><span data-stu-id="6135c-145">EndTime</span></span>](endtime.md)
    
- [<span data-ttu-id="6135c-146">интерналрепли</span><span class="sxs-lookup"><span data-stu-id="6135c-146">InternalReply</span></span>](internalreply.md)
    
- [<span data-ttu-id="6135c-147">екстерналрепли</span><span class="sxs-lookup"><span data-stu-id="6135c-147">ExternalReply</span></span>](externalreply.md)
    
- [<span data-ttu-id="6135c-148">Сообщение</span><span class="sxs-lookup"><span data-stu-id="6135c-148">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="6135c-149">алловекстерналуф</span><span class="sxs-lookup"><span data-stu-id="6135c-149">AllowExternalOof</span></span>](allowexternaloof.md)
    
## <a name="getuseroofsettings-error-response-example"></a><span data-ttu-id="6135c-150">Пример ответа на сообщение об ошибке GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="6135c-150">GetUserOofSettings Error response example</span></span>

### <a name="description"></a><span data-ttu-id="6135c-151">Description</span><span class="sxs-lookup"><span data-stu-id="6135c-151">Description</span></span>

<span data-ttu-id="6135c-152">В следующем примере показан ответ об ошибке, вызванный попыткой доступа к сведениям об отсутствии на работе другого пользователя.</span><span class="sxs-lookup"><span data-stu-id="6135c-152">The following example shows an error response caused by an attempt to access another user's OOF information.</span></span>
  
### <a name="code"></a><span data-ttu-id="6135c-153">Код</span><span class="sxs-lookup"><span data-stu-id="6135c-153">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="685" MinorBuildNumber="8" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <soap:Fault>
      <faultcode>soap:Client</faultcode>
      <faultstring>Microsoft.Exchange.Data.Storage.AccessDeniedException: User is not mailbox owner. User = S-1-5-21-3642464542-282065186-3871681729-1155, MailboxGuid = S-1-5-21-3642464542-282065186-3871681729-1156 ---> User is not mailbox owner. </faultstring>
      <faultactor>https://CAS01.example.com/EWS/Exchange.asmx</faultactor>
      <detail>
        <ErrorCode xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">-2146233088</ErrorCode>
      </detail>
    </soap:Fault>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="6135c-154">См. также</span><span class="sxs-lookup"><span data-stu-id="6135c-154">See also</span></span>



- [<span data-ttu-id="6135c-155">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="6135c-155">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

