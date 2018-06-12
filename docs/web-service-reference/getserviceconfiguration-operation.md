---
title: Операция GetServiceConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfiguration
api_type:
- schema
ms.assetid: 070cbfe5-325a-4955-8e4a-8230ea0459a7
description: Операция GetServiceConfiguration получает сведения о конфигурации для указанного типа службы. Эта операция может вернуть параметры конфигурации для службы единой системы обмена сообщениями, правила защиты и почтовые подсказки.
ms.openlocfilehash: 7fdc4d8defac3d6d352c121483bf8a4c735d9629
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833667"
---
# <a name="getserviceconfiguration-operation"></a><span data-ttu-id="bdf90-104">Операция GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf90-104">GetServiceConfiguration operation</span></span>

<span data-ttu-id="bdf90-105">Операция **GetServiceConfiguration** получает сведения о конфигурации для указанного типа службы.</span><span class="sxs-lookup"><span data-stu-id="bdf90-105">The **GetServiceConfiguration** operation gets configuration information for the specified type of service.</span></span> <span data-ttu-id="bdf90-106">Эта операция может вернуть параметры конфигурации для службы единой системы обмена сообщениями, правила защиты и почтовые подсказки.</span><span class="sxs-lookup"><span data-stu-id="bdf90-106">This operation can return configuration settings for the Unified Messaging, Protection Rules, and Mail Tips services.</span></span> 
  
## <a name="getserviceconfiguration-request-example"></a><span data-ttu-id="bdf90-107">Пример запроса GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf90-107">GetServiceConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="bdf90-108">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf90-108">Description</span></span>

<span data-ttu-id="bdf90-109">В следующем примере запрос **GetServiceConfiguration** показано, как для формирования запроса для получения сведений о конфигурации службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="bdf90-109">The following example of a **GetServiceConfiguration** request shows how to form a request to get configuration information for the Unified Messaging service.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bdf90-110">Программа</span><span class="sxs-lookup"><span data-stu-id="bdf90-110">Code</span></span>

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
    <m:GetServiceConfiguration>
      <m:RequestedConfiguration>
        <m:ConfigurationName>UnifiedMessagingConfiguration</m:ConfigurationName>
      </m:RequestedConfiguration>
    </m:GetServiceConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getserviceconfiguration-response-example"></a><span data-ttu-id="bdf90-111">Пример ответа GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf90-111">GetServiceConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="bdf90-112">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf90-112">Description</span></span>

<span data-ttu-id="bdf90-113">В следующем примере показано успешного ответа на запрос **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="bdf90-113">The following example shows a successful response to the **GetServiceConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bdf90-114">Программа</span><span class="sxs-lookup"><span data-stu-id="bdf90-114">Code</span></span>

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
    <GetServiceConfigurationResponse ResponseClass="Success" 
                                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <ResponseMessages>
        <ServiceConfigurationResponseMessageType ResponseClass="Success">
          <ResponseCode>NoError</ResponseCode>
          <m:UnifiedMessagingConfiguration xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
            <t:UmEnabled xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">true</t:UmEnabled>
            <t:PlayOnPhoneDialString xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">user@contoso.com</t:PlayOnPhoneDialString>
            <t:PlayOnPhoneEnabled xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">true</t:PlayOnPhoneEnabled>
          </m:UnifiedMessagingConfiguration>
        </ServiceConfigurationResponseMessageType>
      </ResponseMessages>
    </GetServiceConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="getserviceconfiguration-error-response-example"></a><span data-ttu-id="bdf90-115">Пример ответа об ошибке GetServiceConfiguration</span><span class="sxs-lookup"><span data-stu-id="bdf90-115">GetServiceConfiguration Error response example</span></span>

### <a name="description"></a><span data-ttu-id="bdf90-116">Описание</span><span class="sxs-lookup"><span data-stu-id="bdf90-116">Description</span></span>

<span data-ttu-id="bdf90-117">В следующем примере показано ошибочный ответ на запрос **GetServiceConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="bdf90-117">The following example shows an error response to the **GetServiceConfiguration** request.</span></span> <span data-ttu-id="bdf90-118">Эта ошибка была вызвана именем неправильной конфигурации.</span><span class="sxs-lookup"><span data-stu-id="bdf90-118">This error was caused by an incorrect configuration name.</span></span> 
  
### <a name="code"></a><span data-ttu-id="bdf90-119">Программа</span><span class="sxs-lookup"><span data-stu-id="bdf90-119">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Body>
    <s:Fault>
      <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
      <faultstring xml:lang="en-US">The request failed schema validation: 
      The 'http://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
      is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
      datatype 'http://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType' 
      - The Enumeration constraint failed.</faultstring>
      <detail>
        <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
        <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
        <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
          <t:LineNumber>13</t:LineNumber>
          <t:LinePosition>62</t:LinePosition>
          <t:Violation>The 'http://schemas.microsoft.com/exchange/services/2006/messages:ConfigurationName' element 
          is invalid - The value 'UUnifiedMessagingConfiguration' is invalid according to its 
          datatype 'http://schemas.microsoft.com/exchange/services/2006/types:ServiceConfigurationType'
          - The Enumeration constraint failed.</t:Violation>
        </t:MessageXml>
      </detail>
    </s:Fault>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="bdf90-120">См. также</span><span class="sxs-lookup"><span data-stu-id="bdf90-120">See also</span></span>



[<span data-ttu-id="bdf90-121">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bdf90-121">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="bdf90-122">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="bdf90-122">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

