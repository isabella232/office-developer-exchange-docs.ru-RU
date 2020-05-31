---
title: Операция GetUMProperties (веб-служба единой системы обмена сообщениями)
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
description: Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, сделавшего запрос.
ms.openlocfilehash: 8878099bbd907fe0648f7d64dde3cd9600c2c45f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833678"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="51bea-103">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="51bea-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="51bea-104">Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, сделавшего запрос.</span><span class="sxs-lookup"><span data-stu-id="51bea-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="51bea-105">Пример запроса GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="51bea-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="51bea-106">Описание</span><span class="sxs-lookup"><span data-stu-id="51bea-106">Description</span></span>

<span data-ttu-id="51bea-107">В приведенном ниже примере запроса GetUMProperties показано, как сформировать запрос на получение свойств единой системы обмена сообщениями почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="51bea-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="51bea-108">Код</span><span class="sxs-lookup"><span data-stu-id="51bea-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="51bea-109">Пример успешного ответа GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="51bea-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="51bea-110">Описание</span><span class="sxs-lookup"><span data-stu-id="51bea-110">Description</span></span>

<span data-ttu-id="51bea-111">В приведенном ниже примере ответа GetUMProperties показан ответ на запрос GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="51bea-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="51bea-112">Код</span><span class="sxs-lookup"><span data-stu-id="51bea-112">Code</span></span>

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

## <a name="see-also"></a><span data-ttu-id="51bea-113">См. также</span><span class="sxs-lookup"><span data-stu-id="51bea-113">See also</span></span>



[<span data-ttu-id="51bea-114">GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="51bea-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="51bea-115">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="51bea-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

