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
ms.openlocfilehash: 42176d9cd0288af6515aeea616a4f216a419410c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462474"
---
# <a name="getumproperties-operation-um-web-service"></a><span data-ttu-id="cbb0e-103">Операция GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="cbb0e-103">GetUMProperties operation (UM web service)</span></span>

<span data-ttu-id="cbb0e-104">Операция GetUMProperties получает все свойства единой системы обмена сообщениями для почтового ящика пользователя, сделавшего запрос.</span><span class="sxs-lookup"><span data-stu-id="cbb0e-104">The GetUMProperties operation gets all the Unified Messaging properties for the mailbox of the user who is making the request.</span></span>
  
## <a name="getumproperties-request-example"></a><span data-ttu-id="cbb0e-105">Пример запроса GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="cbb0e-105">GetUMProperties request example</span></span>

### <a name="description"></a><span data-ttu-id="cbb0e-106">Описание</span><span class="sxs-lookup"><span data-stu-id="cbb0e-106">Description</span></span>

<span data-ttu-id="cbb0e-107">В приведенном ниже примере запроса GetUMProperties показано, как сформировать запрос на получение свойств единой системы обмена сообщениями почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="cbb0e-107">The following example of a GetUMProperties request shows how to form a request to get the Unified Messaging properties of a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="cbb0e-108">Код</span><span class="sxs-lookup"><span data-stu-id="cbb0e-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUMProperties xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" />
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-getumproperties-response-example"></a><span data-ttu-id="cbb0e-109">Пример успешного ответа GetUMProperties</span><span class="sxs-lookup"><span data-stu-id="cbb0e-109">Successful GetUMProperties response example</span></span>

### <a name="description"></a><span data-ttu-id="cbb0e-110">Описание</span><span class="sxs-lookup"><span data-stu-id="cbb0e-110">Description</span></span>

<span data-ttu-id="cbb0e-111">В приведенном ниже примере ответа GetUMProperties показан ответ на запрос GetUMProperties.</span><span class="sxs-lookup"><span data-stu-id="cbb0e-111">The following example of a GetUMProperties response shows a response to the GetUMProperties request.</span></span>
  
### <a name="code"></a><span data-ttu-id="cbb0e-112">Код</span><span class="sxs-lookup"><span data-stu-id="cbb0e-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <GetUMPropertiesResponse xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a><span data-ttu-id="cbb0e-113">См. также</span><span class="sxs-lookup"><span data-stu-id="cbb0e-113">See also</span></span>



[<span data-ttu-id="cbb0e-114">GetUMProperties (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="cbb0e-114">GetUMProperties (UM web service)</span></span>](getumproperties-um-web-service.md)
  
[<span data-ttu-id="cbb0e-115">Жетумпропертиесреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="cbb0e-115">GetUMPropertiesResponse (UM web service)</span></span>](getumpropertiesresponse-um-web-service.md)

