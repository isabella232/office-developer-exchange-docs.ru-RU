---
title: Операция GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Найдите сведения о веб-служб Exchange GetAppManifests операции.
ms.openlocfilehash: 9c919bac9ac0042890d1c439454b37e6b7c60876
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762683"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="6b152-103">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6b152-103">GetAppManifests operation</span></span>

<span data-ttu-id="6b152-104">Найдите сведения о операции **GetAppManifests** веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b152-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="6b152-105">Операция **GetAppManifests** извлекает манифестов приложений.</span><span class="sxs-lookup"><span data-stu-id="6b152-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="6b152-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="6b152-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="6b152-107">С помощью операции GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6b152-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="6b152-108">Операция **GetAppManifests** не имеет аргументов, чтобы запросить манифестов приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6b152-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="6b152-109">Ответ будет содержать кодировки Base64 XML-файлах манифестов для каждого приложения, которая устанавливается в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="6b152-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="6b152-110">Заголовки SOAP GetAppManifests операции</span><span class="sxs-lookup"><span data-stu-id="6b152-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="6b152-111">Операция **GetAppManifests** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="6b152-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="6b152-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="6b152-112">**Header name**</span></span>|<span data-ttu-id="6b152-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6b152-113">**Element**</span></span>|<span data-ttu-id="6b152-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6b152-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6b152-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="6b152-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="6b152-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="6b152-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="6b152-117">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="6b152-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="6b152-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="6b152-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="6b152-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="6b152-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="6b152-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="6b152-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="6b152-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="6b152-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="6b152-122">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="6b152-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="6b152-123">Пример запроса GetAppManifests операции: получение манифестов приложений для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="6b152-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="6b152-124">В следующем примере запрос операции **GetAppManifests** показано, как получить манифестов приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6b152-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="6b152-125">Элемент [ApiVersionSupported](apiversionsupported.md) и элемент [SchemaVersionSupported](schemaversionsupported.md) являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="6b152-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013_SP1" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:GetAppManifests>
        <m:ApiVersionSupported>1.1</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.1</m:SchemaVersionSupported>
      </m:GetAppManifests>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="6b152-126">Запрос SOAP body содержит следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="6b152-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="6b152-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6b152-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="6b152-128">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="6b152-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="6b152-129">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="6b152-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="6b152-130">Успешные операции ответа GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="6b152-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="6b152-131">В следующем примере показано успешного ответа на запрос **GetAppManifests** операции для получения манифестов приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="6b152-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="6b152-132">Все манифесты приложений base64 произвольно усечен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="6b152-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="6b152-133">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="6b152-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="6b152-134">GetAppManifestsResponse</span><span class="sxs-lookup"><span data-stu-id="6b152-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="6b152-135">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6b152-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="6b152-136">Приложения</span><span class="sxs-lookup"><span data-stu-id="6b152-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="6b152-137">Приложения</span><span class="sxs-lookup"><span data-stu-id="6b152-137">App</span></span>](app.md)
    
- [<span data-ttu-id="6b152-138">Манифест</span><span class="sxs-lookup"><span data-stu-id="6b152-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="6b152-139">Ответ SOAP body также может содержать следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="6b152-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="6b152-140">Манифесты</span><span class="sxs-lookup"><span data-stu-id="6b152-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="6b152-141">Ошибка операции GetAppManifests ответа</span><span class="sxs-lookup"><span data-stu-id="6b152-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="6b152-142">Сообщений об ошибках, возвращаемых для этой операции связаны с недопустимый формат входных параметров или универсальные ошибок веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="6b152-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="6b152-143">Коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="6b152-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="6b152-144">См. также</span><span class="sxs-lookup"><span data-stu-id="6b152-144">See also</span></span>

- [<span data-ttu-id="6b152-145">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="6b152-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="6b152-146">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="6b152-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="6b152-147">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="6b152-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="6b152-148">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="6b152-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="6b152-149">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="6b152-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

