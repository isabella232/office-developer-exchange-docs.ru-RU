---
title: Операция IsUMEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- IsUMEnabled
api_type:
- schema
ms.assetid: fbe6cd95-f7a5-42b9-8a9d-b6159a269d55
description: Операция IsUMEnabled определяет, включен ли почтовый ящик единой системы обмена сообщениями.
ms.openlocfilehash: 9d94a359d6b11e41762d21aa2fe5501bd9f7b577
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834107"
---
# <a name="isumenabled-operation-um-web-service"></a><span data-ttu-id="fc584-103">Операция IsUMEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="fc584-103">IsUMEnabled operation (UM web service)</span></span>

<span data-ttu-id="fc584-104">Операция IsUMEnabled определяет, включен ли почтовый ящик единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fc584-104">The IsUMEnabled operation determines whether a mailbox is enabled for Unified Messaging.</span></span>
  
## <a name="isumenabled-request-example"></a><span data-ttu-id="fc584-105">Пример запроса IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="fc584-105">IsUMEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="fc584-106">Описание</span><span class="sxs-lookup"><span data-stu-id="fc584-106">Description</span></span>

<span data-ttu-id="fc584-107">В следующем примере запрос IsUMEnabled показано, как для формирования запроса, чтобы определить, включена ли почтовый ящик единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="fc584-107">The following example of an IsUMEnabled request shows how to form a request to determine whether a mailbox is enabled for Unified Messaging.</span></span>
  
### <a name="code"></a><span data-ttu-id="fc584-108">Программа</span><span class="sxs-lookup"><span data-stu-id="fc584-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <IsUMEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-isumenabled-response-example"></a><span data-ttu-id="fc584-109">Пример успешного ответа IsUMEnabled</span><span class="sxs-lookup"><span data-stu-id="fc584-109">Successful IsUMEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="fc584-110">Описание</span><span class="sxs-lookup"><span data-stu-id="fc584-110">Description</span></span>

<span data-ttu-id="fc584-111">В следующем примере показано успешного ответа на запрос IsUMEnabled.</span><span class="sxs-lookup"><span data-stu-id="fc584-111">The following example shows a successful response to an IsUMEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="fc584-112">Программа</span><span class="sxs-lookup"><span data-stu-id="fc584-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <IsUMEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <IsUMEnabledResponse>true</IsUMEnabledResponse> 
    </IsUMEnabledResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="fc584-113">См. также</span><span class="sxs-lookup"><span data-stu-id="fc584-113">See also</span></span>



[<span data-ttu-id="fc584-114">IsUMEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="fc584-114">IsUMEnabled (UM web service)</span></span>](isumenabled-um-web-service.md)
  
[<span data-ttu-id="fc584-115">IsUMEnabledResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="fc584-115">IsUMEnabledResponse (UM web service)</span></span>](isumenabledresponse-um-web-service.md)


[<span data-ttu-id="fc584-116">Единой системы обмена сообщениями веб-службы XML элементов для Exchange</span><span class="sxs-lookup"><span data-stu-id="fc584-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)

