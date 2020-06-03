---
title: Операция отключения (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Disconnect
api_type:
- schema
ms.assetid: a987000b-d6e6-49d7-944c-e9c278d0236f
description: Операция отключения завершает вызов, идентифицируемый заданным CallId (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: a1268f9ea3d879f472e019bf1847fc13d65d1819
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529072"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="c55a9-103">Операция отключения (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c55a9-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="c55a9-104">Операция отключения завершает вызов, идентифицируемый заданным [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="c55a9-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="c55a9-105">Пример запроса на отключение</span><span class="sxs-lookup"><span data-stu-id="c55a9-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="c55a9-106">Description</span><span class="sxs-lookup"><span data-stu-id="c55a9-106">Description</span></span>

<span data-ttu-id="c55a9-107">В приведенном ниже примере запроса на отключение показано, как сформировать запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="c55a9-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="c55a9-108">Код</span><span class="sxs-lookup"><span data-stu-id="c55a9-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="c55a9-109">Пример отклика об успешном отключении</span><span class="sxs-lookup"><span data-stu-id="c55a9-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="c55a9-110">Description</span><span class="sxs-lookup"><span data-stu-id="c55a9-110">Description</span></span>

<span data-ttu-id="c55a9-111">В приведенном ниже примере ответа на отключение показан ответ на запрос на отключение.</span><span class="sxs-lookup"><span data-stu-id="c55a9-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="c55a9-112">Код</span><span class="sxs-lookup"><span data-stu-id="c55a9-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="c55a9-113">См. также</span><span class="sxs-lookup"><span data-stu-id="c55a9-113">See also</span></span>

- [<span data-ttu-id="c55a9-114">Отключение (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c55a9-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="c55a9-115">Дисконнектреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c55a9-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="c55a9-116">CallId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="c55a9-116">CallId (UM web service)</span></span>](callid-um-web-service.md)

