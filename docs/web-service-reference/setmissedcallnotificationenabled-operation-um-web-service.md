---
title: Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetMissedCallNotificationEnabled
api_type:
- schema
ms.assetid: 6693b5db-ac6b-43bc-af83-a9c94fc425bf
description: Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.
ms.openlocfilehash: ca4942942a81bc187e8e18a5e6f003f8587f79d1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467398"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="5a353-103">Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5a353-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="5a353-104">Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="5a353-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="5a353-105">Пример запроса SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="5a353-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="5a353-106">Description</span><span class="sxs-lookup"><span data-stu-id="5a353-106">Description</span></span>

<span data-ttu-id="5a353-107">В следующем примере запроса SetMissedCallNotificationEnabled показано, как сформировать запрос на включение уведомлений о пропущенных звонках.</span><span class="sxs-lookup"><span data-stu-id="5a353-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a353-108">Код</span><span class="sxs-lookup"><span data-stu-id="5a353-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="5a353-109">Пример успешного ответа SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="5a353-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="5a353-110">Description</span><span class="sxs-lookup"><span data-stu-id="5a353-110">Description</span></span>

<span data-ttu-id="5a353-111">В приведенном ниже примере ответа PlayOnPhoneGreeting показан ответ на запрос SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="5a353-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="5a353-112">Код</span><span class="sxs-lookup"><span data-stu-id="5a353-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="5a353-113">См. также</span><span class="sxs-lookup"><span data-stu-id="5a353-113">See also</span></span>



[<span data-ttu-id="5a353-114">SetMissedCallNotificationEnabled (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5a353-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="5a353-115">Сетмисседкаллнотификатионенабледреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="5a353-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="5a353-116">Status (веб-служба единой системы обмена сообщениями — SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="5a353-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

