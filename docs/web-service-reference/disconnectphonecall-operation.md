---
title: Операция DisconnectPhoneCall
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DisconnectPhoneCall
api_type:
- schema
ms.assetid: b42fb512-2ae4-4072-906a-ccebb85edb84
description: Операция DisconnectPhoneCall завершение работы телефонный звонок.
ms.openlocfilehash: 4bd68dd40f831794072263b487255330ea31d7bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762139"
---
# <a name="disconnectphonecall-operation"></a><span data-ttu-id="cfdef-103">Операция DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="cfdef-103">DisconnectPhoneCall operation</span></span>

<span data-ttu-id="cfdef-104">Операция **DisconnectPhoneCall** завершение работы телефонный звонок.</span><span class="sxs-lookup"><span data-stu-id="cfdef-104">The **DisconnectPhoneCall** operation terminates the telephone call.</span></span> 
  
## <a name="disconnectphonecall-request-example"></a><span data-ttu-id="cfdef-105">Пример запроса DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="cfdef-105">DisconnectPhoneCall request example</span></span>

### <a name="description"></a><span data-ttu-id="cfdef-106">Описание</span><span class="sxs-lookup"><span data-stu-id="cfdef-106">Description</span></span>

<span data-ttu-id="cfdef-107">В следующем примере запрос **DisconnectPhoneCall** показано, как для формирования запроса для отключения телефонные звонки.</span><span class="sxs-lookup"><span data-stu-id="cfdef-107">The following example of a **DisconnectPhoneCall** request shows how to form a request to disconnect a telephone call.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cfdef-108">Программа</span><span class="sxs-lookup"><span data-stu-id="cfdef-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:DisconnectPhoneCall>
      <m:PhoneCallId Id="OWVl4NWb3N29t"/>
    </m:DisconnectPhoneCall>
  </soap:Body>
</soap:Envelope>
```

## <a name="disconnectphonecall-response-example"></a><span data-ttu-id="cfdef-109">Пример ответа DisconnectPhoneCall</span><span class="sxs-lookup"><span data-stu-id="cfdef-109">DisconnectPhoneCall response example</span></span>

### <a name="description"></a><span data-ttu-id="cfdef-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cfdef-110">Description</span></span>

<span data-ttu-id="cfdef-111">В следующем примере показано успешного ответа на запрос **DisconnectPhoneCall** .</span><span class="sxs-lookup"><span data-stu-id="cfdef-111">The following example shows a successful response to the **DisconnectPhoneCall** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="cfdef-112">Программа</span><span class="sxs-lookup"><span data-stu-id="cfdef-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <DisconnectPhoneCallResponse ResponseClass="Success" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
    </DisconnectPhoneCallResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="cfdef-113">См. также</span><span class="sxs-lookup"><span data-stu-id="cfdef-113">See also</span></span>

- [<span data-ttu-id="cfdef-114">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="cfdef-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="cfdef-115">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="cfdef-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

