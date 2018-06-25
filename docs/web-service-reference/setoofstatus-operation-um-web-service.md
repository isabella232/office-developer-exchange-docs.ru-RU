---
title: Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
description: Операция SetOofStatus задает значение, указывающее, следует ли воспроизводиться приветствие об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.
ms.openlocfilehash: 2bb1deeec8ddb5be56979bfb2fae3396672298a3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835445"
---
# <a name="setoofstatus-operation-um-web-service"></a><span data-ttu-id="93266-103">Операция SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="93266-103">SetOofStatus operation (UM web service)</span></span>

<span data-ttu-id="93266-104">Операция SetOofStatus задает значение, указывающее, следует ли воспроизводиться приветствие об отсутствии на работе Office (OOF) для пользователя, который выполняет запрос.</span><span class="sxs-lookup"><span data-stu-id="93266-104">The SetOofStatus operation sets a value that indicates whether the Out of Office (OOF) greeting should be played for the user who makes the request.</span></span>
  
## <a name="setoofstatus-request-example"></a><span data-ttu-id="93266-105">Пример запроса SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="93266-105">SetOofStatus request example</span></span>

### <a name="description"></a><span data-ttu-id="93266-106">Описание</span><span class="sxs-lookup"><span data-stu-id="93266-106">Description</span></span>

<span data-ttu-id="93266-107">В следующем примере запрос SetOofStatus показано, как для формирования запроса, чтобы включить приветствие об отсутствии на работе для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="93266-107">The following example of a SetOofStatus request shows how to form a request to enable the Out of Office greeting for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="93266-108">Программа</span><span class="sxs-lookup"><span data-stu-id="93266-108">Code</span></span>

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

## <a name="successful-setoofstatus-response-example"></a><span data-ttu-id="93266-109">Пример успешного ответа SetOofStatus</span><span class="sxs-lookup"><span data-stu-id="93266-109">Successful SetOofStatus response example</span></span>

### <a name="description"></a><span data-ttu-id="93266-110">Описание</span><span class="sxs-lookup"><span data-stu-id="93266-110">Description</span></span>

<span data-ttu-id="93266-111">В следующем примере ответа SetOofStatus показано ответа на запрос SetOofStatus.</span><span class="sxs-lookup"><span data-stu-id="93266-111">The following example of a SetOofStatus response shows a response to the SetOofStatus request.</span></span>
  
### <a name="code"></a><span data-ttu-id="93266-112">Программа</span><span class="sxs-lookup"><span data-stu-id="93266-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetOofStatusResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="93266-113">См. также</span><span class="sxs-lookup"><span data-stu-id="93266-113">See also</span></span>



[<span data-ttu-id="93266-114">SetOofStatus (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="93266-114">SetOofStatus (UM web service)</span></span>](setoofstatus-um-web-service.md)
  
[<span data-ttu-id="93266-115">SetOofStatusResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="93266-115">SetOofStatusResponse (UM web service)</span></span>](setoofstatusresponse-um-web-service.md)
  
[<span data-ttu-id="93266-116">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetOofStatus)</span><span class="sxs-lookup"><span data-stu-id="93266-116">Status (UM web service - SetOofStatus)</span></span>](status-um-web-servicesetoofstatus.md)

