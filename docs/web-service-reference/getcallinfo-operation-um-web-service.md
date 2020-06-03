---
title: Операция GetCallInfo (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetCallInfo
api_type:
- schema
ms.assetid: 6bccd418-caf7-4eb9-8a6f-410e56a635c3
description: Операция GetCallInfo возвращает состояние исходящего вызова, указанного в параметре CallId (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 6b5664dfe16f9c74cc7175098145141b815a6355
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461242"
---
# <a name="getcallinfo-operation-um-web-service"></a><span data-ttu-id="1575b-103">Операция GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-103">GetCallInfo operation (UM web service)</span></span>

<span data-ttu-id="1575b-104">Операция GetCallInfo возвращает состояние исходящего вызова, указанного в параметре [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="1575b-104">The GetCallInfo operation returns the status of the outbound call that is specified by [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="getcallinfo-request-example"></a><span data-ttu-id="1575b-105">Пример запроса GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="1575b-105">GetCallInfo request example</span></span>

### <a name="description"></a><span data-ttu-id="1575b-106">Description</span><span class="sxs-lookup"><span data-stu-id="1575b-106">Description</span></span>

<span data-ttu-id="1575b-107">В следующем примере запроса GetCallInfo показано, как сформировать запрос для получения сведений об указанном исходящем вызове.</span><span class="sxs-lookup"><span data-stu-id="1575b-107">The following example of a GetCallInfo request shows how to form a request to get information about a specified outbound call.</span></span>
  
### <a name="code"></a><span data-ttu-id="1575b-108">Код</span><span class="sxs-lookup"><span data-stu-id="1575b-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetCallInfo xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </GetCallInfo>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getcallinfo-response-example"></a><span data-ttu-id="1575b-109">Пример успешного ответа GetCallInfo</span><span class="sxs-lookup"><span data-stu-id="1575b-109">Successful GetCallInfo response example</span></span>

### <a name="description"></a><span data-ttu-id="1575b-110">Description</span><span class="sxs-lookup"><span data-stu-id="1575b-110">Description</span></span>

<span data-ttu-id="1575b-111">В приведенном ниже примере ответа GetCallInfo показан ответ на запрос GetCallInfo.</span><span class="sxs-lookup"><span data-stu-id="1575b-111">The following example of a GetCallInfo response shows a response to a GetCallInfo request.</span></span>
  
### <a name="code"></a><span data-ttu-id="1575b-112">Код</span><span class="sxs-lookup"><span data-stu-id="1575b-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetCallInfoResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetCallInfoResponse>
        <CallState>Connected</CallState> 
        <EventCause>None</EventCause> 
      </GetCallInfoResponse>
    </GetCallInfoResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1575b-113">См. также</span><span class="sxs-lookup"><span data-stu-id="1575b-113">See also</span></span>



[<span data-ttu-id="1575b-114">GetCallInfo (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-114">GetCallInfo (UM web service)</span></span>](getcallinfo-um-web-service.md)
  
[<span data-ttu-id="1575b-115">Жеткаллинфореспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-115">GetCallInfoResponse (UM web service)</span></span>](getcallinforesponse-um-web-service.md)
  
[<span data-ttu-id="1575b-116">CallId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-116">CallId (UM web service)</span></span>](callid-um-web-service.md)
  
[<span data-ttu-id="1575b-117">Каллстате (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-117">CallState (UM web service)</span></span>](callstate-um-web-service.md)
  
[<span data-ttu-id="1575b-118">Евенткаусе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="1575b-118">EventCause (UM web service)</span></span>](eventcause-um-web-service.md)

