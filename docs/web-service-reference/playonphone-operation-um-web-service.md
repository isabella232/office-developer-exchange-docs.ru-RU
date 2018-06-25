---
title: Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- PlayOnPhone
api_type:
- schema
ms.assetid: 7d55be55-f8b6-4e96-a61e-26fa190217fd
description: Операция PlayOnPhone исходящего звонка и воспроизведения заданным сообщением по телефону, которое задано в элементе DialString.
ms.openlocfilehash: b55bb45d6654f57503879f33e1cd5013ddb69a2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834818"
---
# <a name="playonphone-operation-um-web-service"></a><span data-ttu-id="cc84f-103">Операция PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="cc84f-103">PlayOnPhone operation (UM web service)</span></span>

<span data-ttu-id="cc84f-104">Операция PlayOnPhone исходящего звонка и воспроизведения заданным сообщением по телефону, которое задано в элементе **DialString** .</span><span class="sxs-lookup"><span data-stu-id="cc84f-104">The PlayOnPhone operation makes an outbound call and plays a specified message over the telephone that is specified by the **DialString** element.</span></span> 
  
## <a name="playonphone-request-example"></a><span data-ttu-id="cc84f-105">Пример запроса PlayOnPhone</span><span class="sxs-lookup"><span data-stu-id="cc84f-105">PlayOnPhone request example</span></span>

### <a name="description"></a><span data-ttu-id="cc84f-106">Описание</span><span class="sxs-lookup"><span data-stu-id="cc84f-106">Description</span></span>

<span data-ttu-id="cc84f-107">В следующем примере запрос PlayOnPhone показано, как для формирования запроса на выполнение исходящего звонка и воспроизведение сообщения.</span><span class="sxs-lookup"><span data-stu-id="cc84f-107">The following example of a PlayOnPhone request shows how to form a request to make an outbound call and play a message.</span></span>
  
### <a name="code"></a><span data-ttu-id="cc84f-108">Программа</span><span class="sxs-lookup"><span data-stu-id="cc84f-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <PlayOnPhone xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <entryId>AAAAAGsd2rbQLVtLobUGbrq/9IUHAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAACxVpEl+KVVLl957wp//x6UAGAetcDUAAA==</entryId>
      <DialString>12345</DialString>
    </PlayOnPhone>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-playonphone-response-example"></a><span data-ttu-id="cc84f-109">Пример успешного ответа PlayOnPhone</span><span class="sxs-lookup"><span data-stu-id="cc84f-109">Successful PlayOnPhone response example</span></span>

### <a name="description"></a><span data-ttu-id="cc84f-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cc84f-110">Description</span></span>

<span data-ttu-id="cc84f-111">В следующем примере ответа PlayOnPhone показано ответа на запрос PlayOnPhone.</span><span class="sxs-lookup"><span data-stu-id="cc84f-111">The following example of a PlayOnPhone response shows a response to the PlayOnPhone request.</span></span>
  
### <a name="code"></a><span data-ttu-id="cc84f-112">Программа</span><span class="sxs-lookup"><span data-stu-id="cc84f-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <PlayOnPhoneResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <PlayOnPhoneResponse>NDEzYjEzNmMtZTE2Zi00NTJlLWI3YzctNDhkMTE3MDE3YjlmQGRmLWV1bS0wMS5leGNoYW5nZS5jb3JwLm1pY3Jvc29mdC5jb20=</PlayOnPhoneResponse> 
    </PlayOnPhoneResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="cc84f-113">См. также</span><span class="sxs-lookup"><span data-stu-id="cc84f-113">See also</span></span>



[<span data-ttu-id="cc84f-114">PlayOnPhone (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="cc84f-114">PlayOnPhone (UM web service)</span></span>](playonphone-um-web-service.md)
  
[<span data-ttu-id="cc84f-115">PlayOnPhoneResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="cc84f-115">PlayOnPhoneResponse (UM web service)</span></span>](playonphoneresponse-um-web-service.md)
  
[<span data-ttu-id="cc84f-116">Операция PlayOnPhoneGreeting (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="cc84f-116">PlayOnPhoneGreeting operation (UM web service)</span></span>](playonphonegreeting-operation-um-web-service.md)

