---
title: Операция GetDomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a6f4a53d-d7f6-4ad1-8afb-78745c500eaa
description: Операция GetDomainSettings извлекает заданных параметров домена для пользователя. Автообнаружение возвращает домены, которые для обнаружения и требуемые настройки эти домены.
ms.openlocfilehash: 09b1d610cd415d2d9d7d0098354521ece86f5184
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762765"
---
# <a name="getdomainsettings-operation-soap"></a><span data-ttu-id="8dbcb-104">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-104">GetDomainSettings operation (SOAP)</span></span>

<span data-ttu-id="8dbcb-105">Операция **GetDomainSettings** извлекает заданных параметров домена для пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dbcb-105">The **GetDomainSettings** operation retrieves the specified settings of the domain for the user.</span></span> <span data-ttu-id="8dbcb-106">Автообнаружение возвращает домены, которые для обнаружения и требуемые настройки эти домены.</span><span class="sxs-lookup"><span data-stu-id="8dbcb-106">Autodiscover returns the domains that are to be discovered and the requested settings of those domains.</span></span> 
  
## <a name="getdomainsettings-request-example"></a><span data-ttu-id="8dbcb-107">Пример запроса GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="8dbcb-107">GetDomainSettings request example</span></span>

### <a name="description"></a><span data-ttu-id="8dbcb-108">Описание</span><span class="sxs-lookup"><span data-stu-id="8dbcb-108">Description</span></span>

<span data-ttu-id="8dbcb-109">В следующем примере запрос **GetDomainSettings** показано запроса для настройки домена **ExternalEWSUrl** пользователя.</span><span class="sxs-lookup"><span data-stu-id="8dbcb-109">The following example of a **GetDomainSettings** request shows a request for a user's **ExternalEWSUrl** domain settings.</span></span> <span data-ttu-id="8dbcb-110">Клиент отправляет запрос на сервер.</span><span class="sxs-lookup"><span data-stu-id="8dbcb-110">The client sends this request to the server.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8dbcb-111">Программа</span><span class="sxs-lookup"><span data-stu-id="8dbcb-111">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?> 
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"> 
    <soap:Header> 
        <a:RequestedServerVersion>Exchange2010</a:RequestedServerVersion>
        <wsa:Action>http://schemas.microsoft.com/exchange/2010/
            Autodiscover/Autodiscover/GetDomainSettings</wsa:Action>
        <wsa:To>
            https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc
        </wsa:To>
    </soap:Header> 
    <soap:Body> 
        <a:GetDomainSettingsRequestMessage xmlns:a="http://schemas.microsoft.com
            /exchange/2010/Autodiscover"> 
            <a:Request> 
                <a:Domains> 
                    <a:Domain>contoso.com<</a:Domain> 
                </a:Domains> 
                <a:RequestedSettings> 
                    <a:Setting>ExternalEwsUrl</a:Setting> 
                </a:RequestedSettings> 
            </a:Request> 
        </a:GetDomainSettingsRequestMessage> 
    </soap:Body> 
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="8dbcb-112">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="8dbcb-112">Request elements</span></span>

<span data-ttu-id="8dbcb-113">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8dbcb-113">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="8dbcb-114">GetDomainSettingsRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-114">GetDomainSettingsRequestMessage (SOAP)</span></span>](getdomainsettingsrequestmessage-soap.md)
    
- [<span data-ttu-id="8dbcb-115">Запрос (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-115">Request (SOAP)</span></span>](request-soap.md)
    
- [<span data-ttu-id="8dbcb-116">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-116">Domains (SOAP)</span></span>](domains-soap.md)
    
- [<span data-ttu-id="8dbcb-117">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-117">Domain (SOAP)</span></span>](domain-soap.md)
    
- [<span data-ttu-id="8dbcb-118">RequestedSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-118">RequestedSettings (SOAP)</span></span>](requestedsettings-soap.md)
    
- [<span data-ttu-id="8dbcb-119">Параметр (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-119">Setting (SOAP)</span></span>](setting-soap.md)
    
## <a name="getdomainsettings-response-example"></a><span data-ttu-id="8dbcb-120">Пример ответа GetDomainSettings</span><span class="sxs-lookup"><span data-stu-id="8dbcb-120">GetDomainSettings response example</span></span>

### <a name="description"></a><span data-ttu-id="8dbcb-121">Описание</span><span class="sxs-lookup"><span data-stu-id="8dbcb-121">Description</span></span>

<span data-ttu-id="8dbcb-122">В следующем примере показано успешного ответа на запрос **GetDomainSettings** , сервер отправляет клиенту.</span><span class="sxs-lookup"><span data-stu-id="8dbcb-122">The following example shows a successful response to the **GetDomainSettings** request that the server sends to the client.</span></span> 
  
### <a name="code"></a><span data-ttu-id="8dbcb-123">Программа</span><span class="sxs-lookup"><span data-stu-id="8dbcb-123">Code</span></span>

```XML
//www.w3.org/2005/08/addressing"> 
    <s:Header> 
        <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/ 
            Autodiscover/Autodiscover/GetDomainSettingsResponse
        </a:Action> 
        <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
            xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
        <h:MajorVersion>14</h:MajorVersion> 
        <h:MinorVersion>0</h:MinorVersion> 
        <h:MajorBuildNumber>639</h:MajorBuildNumber> 
        <h:MinorBuildNumber>20</h:MinorBuildNumber> 
        <h:Version>Exchange2010</h:Version> 
        </h:ServerVersionInfo>
    </s:Header> 
    <s:Body> 
        <GetDomainSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover"> 
            <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance"> 
                <ErrorCode>NoError</ErrorCode> 
                <ErrorMessage /> 
                <DomainResponses> 
                    <DomainResponse> 
                        <ErrorCode>NoError</ErrorCode> 
                        <ErrorMessage>No error.</ErrorMessage> 
                        <DomainSettingErrors /> 
                        <DomainSettings> 
                            <DomainSetting i:type="DomainStringSetting"> 
                                <Name>ExternalEwsUrl</Name> 
                                <Value>https://emea.mail.microsoft.com/EWS/Exchange.asmx</Value> 
                            </DomainSetting> 
                        </DomainSettings> 
                        <RedirectTarget i:nil="true" /> 
                    </DomainResponse> 
                </DomainResponses> 
            </Response> 
        </GetDomainSettingsResponseMessage> 
    </s:Body> 
</s:Envelope>
```

### <a name="response-elements"></a><span data-ttu-id="8dbcb-124">Элементы ответа</span><span class="sxs-lookup"><span data-stu-id="8dbcb-124">Response elements</span></span>

<span data-ttu-id="8dbcb-125">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="8dbcb-125">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="8dbcb-126">GetDomainSettingsResponseMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-126">GetDomainSettingsResponseMessage (SOAP)</span></span>](getdomainsettingsresponsemessage-soap.md)
    
- [<span data-ttu-id="8dbcb-127">Ответ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-127">Response (SOAP)</span></span>](response-soap.md)
    
- [<span data-ttu-id="8dbcb-128">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-128">ErrorCode (SOAP)</span></span>](errorcode-soap.md)
    
- [<span data-ttu-id="8dbcb-129">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-129">ErrorMessage (SOAP)</span></span>](errormessage-soap.md)
    
- [<span data-ttu-id="8dbcb-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md)
    
- [<span data-ttu-id="8dbcb-131">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-131">DomainResponse (SOAP)</span></span>](domainresponse-soap.md)
    
- [<span data-ttu-id="8dbcb-132">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-132">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md)
    
- [<span data-ttu-id="8dbcb-133">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-133">DomainSettings (SOAP)</span></span>](domainsettings-soap.md)
    
- [<span data-ttu-id="8dbcb-134">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-134">DomainSetting (SOAP)</span></span>](domainsetting-soap.md)
    
- [<span data-ttu-id="8dbcb-135">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-135">Name (SOAP)</span></span>](name-soap.md)
    
- [<span data-ttu-id="8dbcb-136">Значение (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-136">Value (SOAP)</span></span>](value-soap.md)
    
- [<span data-ttu-id="8dbcb-137">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-137">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md)
    
## <a name="see-also"></a><span data-ttu-id="8dbcb-138">См. также</span><span class="sxs-lookup"><span data-stu-id="8dbcb-138">See also</span></span>



[<span data-ttu-id="8dbcb-139">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-139">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="8dbcb-140">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8dbcb-140">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

