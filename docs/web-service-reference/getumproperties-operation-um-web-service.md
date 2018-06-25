---
title: Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- GetUMProperties
api_type:
- schema
ms.assetid: 301fb9a3-67df-44c4-8ffe-0600237fc344
description: Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, отправившего запрос.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833678"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="b9a4e-103">Операция GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9a4e-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="b9a4e-104">Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, отправившего запрос.</span><span class="sxs-lookup"><span data-stu-id="b9a4e-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="b9a4e-105">Пример запроса GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="b9a4e-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="b9a4e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a4e-106">Description</span></span>

<span data-ttu-id="b9a4e-107">В следующем примере запрос GetUMProperties показано, как для формирования запроса для получения свойства почтового ящика единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="b9a4e-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="b9a4e-108">Программа</span><span class="sxs-lookup"><span data-stu-id="b9a4e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="b9a4e-109">Пример успешного ответа GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="b9a4e-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="b9a4e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="b9a4e-110">Description</span></span>

<span data-ttu-id="b9a4e-111">В следующем примере ответа GetUMProperties показано ответа на запрос GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="b9a4e-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="b9a4e-112">Программа</span><span class="sxs-lookup"><span data-stu-id="b9a4e-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetUMPropertiesResponse>
        <OofStatus>false</OofStatus> 
        <MissedCallNotificationEnabled>true</MissedCallNotificationEnabled> 
        <PlayOnPhoneDialString>12345</PlayOnPhoneDialString> 
        <TelephoneAccessNumbers>54321</TelephoneAccessNumbers> 
        <TelephoneAccessFolderEmail>AAAAAGsd2rbQLVtLobUGbrq/9IUBAEX2ikn/L8JJtI5WHI0FAW8AAAFXHhsAAA==</TelephoneAccessFolderEmail> 
      </GetUMPropertiesResponse>
    </GetUMPropertiesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="b9a4e-113">См. также</span><span class="sxs-lookup"><span data-stu-id="b9a4e-113">See also</span></span>



[<span data-ttu-id="b9a4e-114">GetUMProperties (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9a4e-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="b9a4e-115">GetUMPropertiesResponse (веб-служба единой системы обмена СООБЩЕНИЯМИ)</span><span class="sxs-lookup"><span data-stu-id="b9a4e-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

