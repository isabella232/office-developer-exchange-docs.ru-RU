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
ms.openlocfilehash: 1e04e65fa1951a6aa46e2c8b6dd5fe524c84a8fc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762134"
---
# <a name="disconnect-operation-um-web-service"></a><span data-ttu-id="5fee8-103">Операция отключения (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5fee8-103">Disconnect operation (UM web service)</span></span>

<span data-ttu-id="5fee8-104">Операция отключения завершает вызов, идентифицируемый заданным [CallId (веб-служба единой системы обмена сообщениями)](callid-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="5fee8-104">The Disconnect operation terminates the call that is identified by the specified [CallId (UM web service)](callid-um-web-service.md).</span></span>
  
## <a name="disconnect-request-example"></a><span data-ttu-id="5fee8-105">Пример запроса на отключение</span><span class="sxs-lookup"><span data-stu-id="5fee8-105">Disconnect request example</span></span>

### <a name="description"></a><span data-ttu-id="5fee8-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5fee8-106">Description</span></span>

<span data-ttu-id="5fee8-107">В приведенном ниже примере запроса на отключение показано, как сформировать запрос на отключение вызова.</span><span class="sxs-lookup"><span data-stu-id="5fee8-107">The following example of a Disconnect request shows how to form a request to disconnect a call.</span></span>
  
### <a name="code"></a><span data-ttu-id="5fee8-108">Код</span><span class="sxs-lookup"><span data-stu-id="5fee8-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <Disconnect xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <CallId>MDlkZjllZGMtNGUyMy00NzA5LWJkYWYtN2JlMjBjYjBhZTU2QGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</CallId>
    </Disconnect>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-disconnect-response-example"></a><span data-ttu-id="5fee8-109">Пример отклика об успешном отключении</span><span class="sxs-lookup"><span data-stu-id="5fee8-109">Successful Disconnect response example</span></span>

### <a name="description"></a><span data-ttu-id="5fee8-110">Описание</span><span class="sxs-lookup"><span data-stu-id="5fee8-110">Description</span></span>

<span data-ttu-id="5fee8-111">В приведенном ниже примере ответа на отключение показан ответ на запрос на отключение.</span><span class="sxs-lookup"><span data-stu-id="5fee8-111">The following example of a Disconnect response shows a response to the Disconnect request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5fee8-112">Код</span><span class="sxs-lookup"><span data-stu-id="5fee8-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <DisconnectResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5fee8-113">См. также</span><span class="sxs-lookup"><span data-stu-id="5fee8-113">See also</span></span>

- [<span data-ttu-id="5fee8-114">Отключение (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5fee8-114">Disconnect (UM web service)</span></span>](disconnect-um-web-service.md) 
- [<span data-ttu-id="5fee8-115">Дисконнектреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5fee8-115">DisconnectResponse (UM web service)</span></span>](disconnectresponse-um-web-service.md) 
- [<span data-ttu-id="5fee8-116">CallId (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5fee8-116">CallId (UM web service)</span></span>](callid-um-web-service.md)

