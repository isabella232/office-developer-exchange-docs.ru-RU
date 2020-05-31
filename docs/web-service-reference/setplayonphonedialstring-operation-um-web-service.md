---
title: Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- SetPlayOnPhoneDialString
api_type:
- schema
ms.assetid: a68479f2-d900-4dd8-a5ce-dbea8247e841
description: Операция SetPlayOnPhoneDialString задает строку набора номера, используемую по умолчанию для операции PlayOnPhone (веб-служба единой системы обмена сообщениями) и операции PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями).
ms.openlocfilehash: 0d1a879784740777e5eab0cbd5f85e59a6479461
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835446"
---
# <a name="setplayonphonedialstring-operation-um-web-service"></a><span data-ttu-id="888d4-103">Операция SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="888d4-103">SetPlayOnPhoneDialString operation (UM web service)</span></span>

<span data-ttu-id="888d4-104">Операция SetPlayOnPhoneDialString задает строку набора номера, используемую по умолчанию для [операции PlayOnPhone (веб-служба единой системы обмена сообщениями)](playonphone-operation-um-web-service.md) и [операции PlayOnPhoneGreeting (веб-служба единой системы обмена сообщениями)](playonphonegreeting-operation-um-web-service.md).</span><span class="sxs-lookup"><span data-stu-id="888d4-104">The SetPlayOnPhoneDialString operation sets the dial string to use as the default for the [PlayOnPhone operation (UM web service)](playonphone-operation-um-web-service.md) and the [PlayOnPhoneGreeting operation (UM web service)](playonphonegreeting-operation-um-web-service.md).</span></span>
  
## <a name="setplayonphonedialstring-request-example"></a><span data-ttu-id="888d4-105">Пример запроса SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="888d4-105">SetPlayOnPhoneDialString request example</span></span>

### <a name="description"></a><span data-ttu-id="888d4-106">Описание</span><span class="sxs-lookup"><span data-stu-id="888d4-106">Description</span></span>

<span data-ttu-id="888d4-107">В следующем примере запроса SetPlayOnPhoneDialString показано, как сформировать запрос на установку строки набора номера по умолчанию для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="888d4-107">The following example of a SetPlayOnPhoneDialString request shows how to form a request to set the default dial string for a mailbox.</span></span>
  
### <a name="code"></a><span data-ttu-id="888d4-108">Код</span><span class="sxs-lookup"><span data-stu-id="888d4-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetPlayOnPhoneDialString xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
        <dialString>12345</dialString>
    </SetPlayOnPhoneDialString>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-setplayonphonedialstring-response-example"></a><span data-ttu-id="888d4-109">Пример успешного ответа SetPlayOnPhoneDialString</span><span class="sxs-lookup"><span data-stu-id="888d4-109">Successful SetPlayOnPhoneDialString response example</span></span>

### <a name="description"></a><span data-ttu-id="888d4-110">Описание</span><span class="sxs-lookup"><span data-stu-id="888d4-110">Description</span></span>

<span data-ttu-id="888d4-111">В приведенном ниже примере ответа Сетплайонефонедиалстринг показан ответ на запрос SetPlayOnPhoneDialString.</span><span class="sxs-lookup"><span data-stu-id="888d4-111">The following example of a SetPlayOnePhoneDialString response shows a response to the SetPlayOnPhoneDialString request.</span></span>
  
### <a name="code"></a><span data-ttu-id="888d4-112">Код</span><span class="sxs-lookup"><span data-stu-id="888d4-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8" ?> 
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Body>
    <SetPlayOnPhoneDialStringResponse xmlns="http://schemas.microsoft.com/exchange/services/2006/messages" /> 
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="888d4-113">См. также</span><span class="sxs-lookup"><span data-stu-id="888d4-113">See also</span></span>



[<span data-ttu-id="888d4-114">SetPlayOnPhoneDialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="888d4-114">SetPlayOnPhoneDialString (UM web service)</span></span>](setplayonphonedialstring-um-web-service.md)
  
[<span data-ttu-id="888d4-115">Сетплайонфонедиалстрингреспонсе (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="888d4-115">SetPlayOnPhoneDialStringResponse (UM web service)</span></span>](setplayonphonedialstringresponse-um-web-service.md)
  
[<span data-ttu-id="888d4-116">dialString (веб-служба единой системы обмена сообщениями)</span><span class="sxs-lookup"><span data-stu-id="888d4-116">dialString (UM web service)</span></span>](dialstring-um-web-service.md)

