---
title: Операция Жетфедератионинформатион (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c6666a42-a18f-4e4b-beb6-b25ff62cfcc5
description: Операция Жетфедератионинформатион предоставляет сведения о состоянии Федерации Организации, например целевом URI, используемом при запросе маркеров, предназначенных для данной организации, а также о других доменах, Объединенных в Организации.
ms.openlocfilehash: bf38b2f2b3db3e38b9b0157d1677efe4fc274e1b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762792"
---
# <a name="getfederationinformation-operation-soap"></a><span data-ttu-id="de39b-103">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-103">GetFederationInformation operation (SOAP)</span></span>

<span data-ttu-id="de39b-104">Операция **жетфедератионинформатион** предоставляет сведения о состоянии Федерации Организации, например ЦЕЛЕВом URI, используемом при запросе маркеров, предназначенных для данной организации, а также о других доменах, Объединенных в Организации.</span><span class="sxs-lookup"><span data-stu-id="de39b-104">The **GetFederationInformation** operation provides information about the federation status of the organization, such as the target URI to be used when requesting tokens that are targeted at this organization, and the other domains that the organization has also federated.</span></span> 
  
<span data-ttu-id="de39b-105">Только Федеративные организации могут предоставлять общий доступ к календарю, контактам и сообщениям внешним пользователям.</span><span class="sxs-lookup"><span data-stu-id="de39b-105">Only federated organizations can share calendar, contacts, and messages to external users.</span></span>
  
## <a name="getfederationinformation-request-example"></a><span data-ttu-id="de39b-106">Пример запроса Жетфедератионинформатион</span><span class="sxs-lookup"><span data-stu-id="de39b-106">GetFederationInformation request example</span></span>

### <a name="description"></a><span data-ttu-id="de39b-107">Описание</span><span class="sxs-lookup"><span data-stu-id="de39b-107">Description</span></span>

<span data-ttu-id="de39b-108">В приведенном ниже примере запроса **жетфедератионинформатион** показан запрос сведений о Федерации пользователя.</span><span class="sxs-lookup"><span data-stu-id="de39b-108">The following example of a **GetFederationInformation** request shows a request for a user's federation information.</span></span> <span data-ttu-id="de39b-109">Клиент отправляет этот запрос на сервер.</span><span class="sxs-lookup"><span data-stu-id="de39b-109">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="de39b-110">Код</span><span class="sxs-lookup"><span data-stu-id="de39b-110">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:exm="http://schemas.microsoft.com/exchange/services/2006/messages"
           xmlns:ext="http://schemas.microsoft.com/exchange/services/2006/types"
           xmlns:a="http://www.w3.org/2005/08/addressing"
           xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema"> 
    <soap:Header> 
        <a:MessageID>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:MessageID> 
        <a:Action soap:mustUnderstand="1">http://schemas.microsoft.com/
            exchange/2010/Autodiscover/Autodiscover/GetFederationInformation
        </a:Action> 
        <a:To soap:mustUnderstand="1">https://autodiscover.byfcxu-
            dom.extest.microsoft.com/autodiscover/autodiscover.svc</a:To> 
        <a:ReplyTo>
            <a:Address>http://www.w3.org/2005/08/addressing/anonymous</a:Address> 
        </a:ReplyTo> 
    </soap:Header> 
    <soap:Body> 
        <GetFederationInformationRequestMessage 
            xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Request> 
                <Domain>contoso.com</Domain> 
            </Request> 
        </GetFederationInformationRequestMessage>
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="de39b-111">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="de39b-111">Request elements</span></span>

<span data-ttu-id="de39b-112">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="de39b-112">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="de39b-113">Жетфедератионинформатионрекуестмессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-113">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md)
    
- [<span data-ttu-id="de39b-114">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-114">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="de39b-115">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-115">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="getfederationinformation-response-example"></a><span data-ttu-id="de39b-116">Пример отклика Жетфедератионинформатион</span><span class="sxs-lookup"><span data-stu-id="de39b-116">GetFederationInformation response example</span></span>

### <a name="description"></a><span data-ttu-id="de39b-117">Описание</span><span class="sxs-lookup"><span data-stu-id="de39b-117">Description</span></span>

<span data-ttu-id="de39b-118">В следующем примере показан успешный ответ на запрос **жетфедератионинформатион** , отправляемый сервером клиенту.</span><span class="sxs-lookup"><span data-stu-id="de39b-118">The following example shows a successful response to the **GetFederationInformation** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="de39b-119">Код</span><span class="sxs-lookup"><span data-stu-id="de39b-119">Code</span></span>

```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
xmlns:a="http://www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">
            http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetFederationInformationResponse
        </a:Action> 
        <a:RelatesTo>urn:uuid:6389558d-9e05-465e-ade9-aae14c4bcd10</a:RelatesTo> 
    </s:Header> 
    <s:Body> 
        <GetFederationInformationResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage/> 
                <ApplicationUri>BYFCXU-DOM.EXTEST.MICROSOFT.COM</ApplicationUri> 
                <Domains> 
                    <Domain>contoso.com</Domain> 
                    <Domain>europe.contoso.com</Domain> 
                    <Domain>americas.contoso.com</Domain> 
                    <Domain>contosolive.com</Domain> 
                </Domains> 
            </Response> 
        </GetFederationInformationResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="de39b-120">Элементы Response</span><span class="sxs-lookup"><span data-stu-id="de39b-120">Response elements</span></span>

<span data-ttu-id="de39b-121">В отклике используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="de39b-121">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="de39b-122">Жетфедератионинформатионреспонсемессаже (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-122">GetFederationInformationResponseMessage (SOAP)</span></span>](getfederationinformationresponsemessage-soap.md)
    
- [<span data-ttu-id="de39b-123">Отклик (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-123">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="de39b-124">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-124">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="de39b-125">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-125">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="de39b-126">ApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-126">ApplicationUri (SOAP)</span></span>](applicationuri-soap.md)
    
- [<span data-ttu-id="de39b-127">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-127">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="de39b-128">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-128">Domain (SOAP)</span></span>](domain-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="de39b-129">См. также</span><span class="sxs-lookup"><span data-stu-id="de39b-129">See also</span></span>

- [<span data-ttu-id="de39b-130">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
- [<span data-ttu-id="de39b-131">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="de39b-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

