---
title: Операция SetOofStatus (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetOofStatus
api_type:
- schema
ms.assetid: 97c271e9-506e-43eb-89cd-46803fc47ee5
description: Операция SetOofStatus задает значение, указывающее, следует ли воспроизводить приветствие "нет на месте" для пользователя, который отправляет запрос.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835445"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="f83d0-103">Операция SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f83d0-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="f83d0-104">Операция SetOofStatus задает значение, указывающее, следует ли воспроизводить приветствие "нет на месте" для пользователя, который отправляет запрос.</span><span class="sxs-lookup"><span data-stu-id="f83d0-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="f83d0-105">Пример запроса SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="f83d0-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="f83d0-106">Описание</span><span class="sxs-lookup"><span data-stu-id="f83d0-106">Description</span></span>

<span data-ttu-id="f83d0-107">В приведенном ниже примере запроса SetOofStatus показано, как сформировать запрос на включение приветствия "нет на месте" для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f83d0-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="f83d0-108">Код</span><span class="sxs-lookup"><span data-stu-id="f83d0-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetOofStatus xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetOofStatus>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="f83d0-109">Пример успешного ответа SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="f83d0-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="f83d0-110">Описание</span><span class="sxs-lookup"><span data-stu-id="f83d0-110">Description</span></span>

<span data-ttu-id="f83d0-111">В приведенном ниже примере ответа SetOofStatus показан ответ на запрос SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="f83d0-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="f83d0-112">Код</span><span class="sxs-lookup"><span data-stu-id="f83d0-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="f83d0-113">См. также</span><span class="sxs-lookup"><span data-stu-id="f83d0-113">See also</span></span>



[<span data-ttu-id="f83d0-114">SetOofStatus (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f83d0-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="f83d0-115">Сетуфстатусреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="f83d0-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="f83d0-116">Status (веб-служба единой системы обмена сообщениями — SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="f83d0-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

