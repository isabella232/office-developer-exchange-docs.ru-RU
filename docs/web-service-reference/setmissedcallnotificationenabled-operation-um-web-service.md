---
title: Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)
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
ms.openlocfilehash: be9479d6ed2c5238ed19c3d22e028fca62b8deed
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835434"
---
# <a name="setmissedcallnotificationenabled-operation-um-web-service"></a><span data-ttu-id="8ae52-103">Операция SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8ae52-103">SetMissedCallNotificationEnabled operation (UM web service)</span></span>

<span data-ttu-id="8ae52-104">Операция SetMissedCallNotificationEnabled включает или отключает уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="8ae52-104">The SetMissedCallNotificationEnabled operation enables or disables missed call notifications.</span></span>
  
## <a name="setmissedcallnotificationenabled-request-example"></a><span data-ttu-id="8ae52-105">Пример запроса SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="8ae52-105">SetMissedCallNotificationEnabled request example</span></span>

### <a name="description"></a><span data-ttu-id="8ae52-106">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae52-106">Description</span></span>

<span data-ttu-id="8ae52-107">В следующем примере запрос SetMissedCallNotificationEnabled показано, как для формирования запроса, чтобы включить уведомления о пропущенных вызовах.</span><span class="sxs-lookup"><span data-stu-id="8ae52-107">The following example of a SetMissedCallNotificationEnabled request shows how to form a request to enable missed call notifications.</span></span>
  
### <a name="code"></a><span data-ttu-id="8ae52-108">Программа</span><span class="sxs-lookup"><span data-stu-id="8ae52-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetMissedCallNotificationEnabled xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <status>true</status>
    </SetMissedCallNotificationEnabled>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setmissedcallnotificationenabled-response-example"></a><span data-ttu-id="8ae52-109">Пример успешного ответа SetMissedCallNotificationEnabled</span><span class="sxs-lookup"><span data-stu-id="8ae52-109">Successful SetMissedCallNotificationEnabled response example</span></span>

### <a name="description"></a><span data-ttu-id="8ae52-110">Описание</span><span class="sxs-lookup"><span data-stu-id="8ae52-110">Description</span></span>

<span data-ttu-id="8ae52-111">В следующем примере ответа PlayOnPhoneGreeting показано ответа на запрос SetMissedCallNotificationEnabled.</span><span class="sxs-lookup"><span data-stu-id="8ae52-111">The following example of a PlayOnPhoneGreeting response shows a response to the SetMissedCallNotificationEnabled request.</span></span>
  
### <a name="code"></a><span data-ttu-id="8ae52-112">Программа</span><span class="sxs-lookup"><span data-stu-id="8ae52-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetMissedCallNotificationEnabledResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="8ae52-113">См. также</span><span class="sxs-lookup"><span data-stu-id="8ae52-113">See also</span></span>



[<span data-ttu-id="8ae52-114">SetMissedCallNotificationEnabled (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8ae52-114">SetMissedCallNotificationEnabled (UM web service)</span></span>](setmissedcallnotificationenabled-um-web-service.md)
  
[<span data-ttu-id="8ae52-115">SetMissedCallNotificationEnabledResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="8ae52-115">SetMissedCallNotificationEnabledResponse (UM web service)</span></span>](setmissedcallnotificationenabledresponse-um-web-service.md)
  
[<span data-ttu-id="8ae52-116">Состояние (единой системы обмена СООБЩЕНИЯМИ веб-службы - SetMissedCallNotificationEnabled)</span><span class="sxs-lookup"><span data-stu-id="8ae52-116">Status (UM web service - SetMissedCallNotificationEnabled)</span></span>](status-um-web-servicesetmissedcallnotificationenabled.md)

