---
title: Операция GetUserConfiguration
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfiguration
api_type:
- schema
ms.assetid: 71d50e3c-92bd-435f-8118-b28bb85f8138
description: Операция GetUserConfiguration получает объект конфигурации пользователя из папки.
ms.openlocfilehash: fb28e88d1a47b0ea8f63ed33b1efacae8538e1c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458210"
---
# <a name="getuserconfiguration-operation"></a><span data-ttu-id="80ed7-103">Операция GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="80ed7-103">GetUserConfiguration operation</span></span>

<span data-ttu-id="80ed7-104">Операция **GetUserConfiguration** получает объект конфигурации пользователя из папки.</span><span class="sxs-lookup"><span data-stu-id="80ed7-104">The **GetUserConfiguration** operation gets a user configuration object from a folder.</span></span> 
  
## <a name="getuserconfiguration-request-example"></a><span data-ttu-id="80ed7-105">Пример запроса GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="80ed7-105">GetUserConfiguration request example</span></span>

### <a name="description"></a><span data-ttu-id="80ed7-106">Description</span><span class="sxs-lookup"><span data-stu-id="80ed7-106">Description</span></span>

<span data-ttu-id="80ed7-107">В приведенном ниже примере запроса **GetUserConfiguration** показано, как сформировать запрос на получение объекта конфигурации пользователя в папке "Черновики".</span><span class="sxs-lookup"><span data-stu-id="80ed7-107">The following example of a **GetUserConfiguration** request shows how to form a request to get a user configuration object on the Drafts folder.</span></span> 
  
### <a name="code"></a><span data-ttu-id="80ed7-108">Код</span><span class="sxs-lookup"><span data-stu-id="80ed7-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xs="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010" />
  </soap:Header>
  <soap:Body>
    <m:GetUserConfiguration>
      <m:UserConfigurationName Name="TestConfig">
        <t:DistinguishedFolderId Id="drafts"/>
      </m:UserConfigurationName>
      <m:UserConfigurationProperties>Dictionary</m:UserConfigurationProperties>
    </m:GetUserConfiguration>
  </soap:Body>
</soap:Envelope>
```

## <a name="getuserconfiguration-response-example"></a><span data-ttu-id="80ed7-109">Пример отклика GetUserConfiguration</span><span class="sxs-lookup"><span data-stu-id="80ed7-109">GetUserConfiguration response example</span></span>

### <a name="description"></a><span data-ttu-id="80ed7-110">Description</span><span class="sxs-lookup"><span data-stu-id="80ed7-110">Description</span></span>

<span data-ttu-id="80ed7-111">В следующем примере показан успешный ответ на запрос **GetUserConfiguration** .</span><span class="sxs-lookup"><span data-stu-id="80ed7-111">The following example shows a successful response to the **GetUserConfiguration** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="80ed7-112">Код</span><span class="sxs-lookup"><span data-stu-id="80ed7-112">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="20" 
                         Version="Exchange2010" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetUserConfigurationResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetUserConfigurationResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:UserConfiguration>
            <t:UserConfigurationName Name="TestConfig">
              <t:DistinguishedFolderId Id="drafts">
              </t:DistinguishedFolderId>
            </t:UserConfigurationName>
            <t:Dictionary>
              <t:DictionaryEntry>
                <t:DictionaryKey>
                  <t:Type>String</t:Type>
                  <t:Value>PhoneNumber</t:Value>
                </t:DictionaryKey>
                <t:DictionaryValue>
                  <t:Type>String</t:Type>
                  <t:Value>555-555-1111</t:Value>
                </t:DictionaryValue>
              </t:DictionaryEntry>
            </t:Dictionary>
          </m:UserConfiguration>
        </m:GetUserConfigurationResponseMessage>
      </m:ResponseMessages>
    </m:GetUserConfigurationResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="80ed7-113">См. также</span><span class="sxs-lookup"><span data-stu-id="80ed7-113">See also</span></span>



[<span data-ttu-id="80ed7-114">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="80ed7-114">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="80ed7-115">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="80ed7-115">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

