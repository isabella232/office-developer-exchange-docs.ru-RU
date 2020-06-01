---
title: Операция GetAppManifests
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 21a4987c-c24d-4a6e-ace4-e81edcda6303
description: Поиск сведений о GetAppManifestsной операции EWS.
ms.openlocfilehash: 4d4c1d32f14cf144335ddfdf8c9cd4c88a4421d0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463008"
---
# <a name="getappmanifests-operation"></a><span data-ttu-id="82791-103">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-103">GetAppManifests operation</span></span>

<span data-ttu-id="82791-104">Поиск сведений о **GetAppManifestsной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="82791-104">Find information about the **GetAppManifests** EWS operation.</span></span> 
  
<span data-ttu-id="82791-105">Операция **GetAppManifests** получает манифесты приложений.</span><span class="sxs-lookup"><span data-stu-id="82791-105">The **GetAppManifests** operation retrieves app manifests.</span></span> 
  
<span data-ttu-id="82791-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="82791-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmanifests-operation"></a><span data-ttu-id="82791-107">Использование операции GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-107">Using the GetAppManifests operation</span></span>

<span data-ttu-id="82791-108">Операция **GetAppManifests** не имеет аргументов для запроса манифестов приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="82791-108">The **GetAppManifests** operation does not take any arguments to request the app manifests for a mailbox.</span></span> <span data-ttu-id="82791-109">Ответ будет содержать XML-файлы манифеста в кодировке Base64 для каждого приложения, установленного в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="82791-109">The response will contain base64-encoded XML manifest files for each app that is installed in a mailbox.</span></span> 
  
### <a name="getappmanifests-operation-soap-headers"></a><span data-ttu-id="82791-110">Заголовки SOAP операции GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-110">GetAppManifests operation SOAP headers</span></span>

<span data-ttu-id="82791-111">Операция **GetAppManifests** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="82791-111">The **GetAppManifests** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="82791-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="82791-112">**Header name**</span></span>|<span data-ttu-id="82791-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="82791-113">**Element**</span></span>|<span data-ttu-id="82791-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="82791-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="82791-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="82791-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="82791-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="82791-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="82791-117">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="82791-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="82791-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="82791-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="82791-119">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="82791-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="82791-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="82791-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="82791-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="82791-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="82791-122">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="82791-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmanifests-operation-request-example-get-the-app-manifests-for-a-mailbox"></a><span data-ttu-id="82791-123">Пример запроса операции GetAppManifests: получение манифестов приложений для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="82791-123">GetAppManifests operation request example: Get the app manifests for a mailbox</span></span>

<span data-ttu-id="82791-124">В следующем примере запроса операции **GetAppManifests** показано, как получить манифесты приложения для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="82791-124">The following example of a **GetAppManifests** operation request shows how to get the app manifests for a mailbox.</span></span> <span data-ttu-id="82791-125">Элементы [апиверсионсуппортед](apiversionsupported.md) и [счемаверсионсуппортед](schemaversionsupported.md) являются необязательными.</span><span class="sxs-lookup"><span data-stu-id="82791-125">The [ApiVersionSupported](apiversionsupported.md) element and the [SchemaVersionSupported](schemaversionsupported.md) element are optional.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="82791-126">Текст SOAP запроса содержит следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="82791-126">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="82791-127">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-127">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="82791-128">апиверсионсуппортед</span><span class="sxs-lookup"><span data-stu-id="82791-128">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="82791-129">счемаверсионсуппортед</span><span class="sxs-lookup"><span data-stu-id="82791-129">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmanifests-operation-response"></a><span data-ttu-id="82791-130">Успешный отклик операции GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-130">Successful GetAppManifests operation response</span></span>

<span data-ttu-id="82791-131">В следующем примере показан успешный ответ на запрос операции **GetAppManifests** для получения манифестов приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="82791-131">The following example shows a successful response to a **GetAppManifests** operation request to get the app manifests for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="82791-132">Все манифесты приложений Base64 были произвольно усечены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="82791-132">All base64 app manifests have been arbitrarily truncated to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="07" 
                           Version="V2_10" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppManifestsResponse ResponseClass="Success" 
                               xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <m:Apps xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
          <t:App xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
            <t:Manifest>WNlQXBwPg==</t:Manifest>
          </t:App>
         </m:Apps>
      </GetAppManifestsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="82791-133">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="82791-133">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="82791-134">жетаппманифестсреспонсе</span><span class="sxs-lookup"><span data-stu-id="82791-134">GetAppManifestsResponse</span></span>](getappmanifestsresponse.md)
    
- [<span data-ttu-id="82791-135">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="82791-135">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="82791-136">Приложения</span><span class="sxs-lookup"><span data-stu-id="82791-136">Apps</span></span>](apps.md)
    
- [<span data-ttu-id="82791-137">Приложение</span><span class="sxs-lookup"><span data-stu-id="82791-137">App</span></span>](app.md)
    
- [<span data-ttu-id="82791-138">Манифест</span><span class="sxs-lookup"><span data-stu-id="82791-138">Manifest</span></span>](manifest.md)
    
<span data-ttu-id="82791-139">Тело SOAP отклика также может содержать следующий элемент:</span><span class="sxs-lookup"><span data-stu-id="82791-139">The response SOAP body can also contain the following element:</span></span>
  
- [<span data-ttu-id="82791-140">Манифесты</span><span class="sxs-lookup"><span data-stu-id="82791-140">Manifests</span></span>](manifests.md)
    
## <a name="getappmanifests-operation-error-response"></a><span data-ttu-id="82791-141">Ответ об ошибке операции GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="82791-141">GetAppManifests operation error response</span></span>

<span data-ttu-id="82791-142">Ошибки, возвращаемые для этой операции, связаны с недопустимым форматом входных параметров или общими ошибками EWS.</span><span class="sxs-lookup"><span data-stu-id="82791-142">Errors returned for this operation are related to an invalid format of the input parameters or are generic EWS errors.</span></span> <span data-ttu-id="82791-143">Коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="82791-143">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
```
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="07"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetAppManifestsResponse ResponseClass="Error"
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>The apiVersionSupported parameter is invalid. 
                   It should be in the form of major version, minor 
                   version, separated by '.', for example '2.34'.</MessageText>
      <ResponseCode>ErrorInvalidRequest</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetAppManifestsResponse>
  </s:Body>
</s:Envelope>

```

## <a name="see-also"></a><span data-ttu-id="82791-144">См. также</span><span class="sxs-lookup"><span data-stu-id="82791-144">See also</span></span>

- [<span data-ttu-id="82791-145">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="82791-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="82791-146">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="82791-146">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="82791-147">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="82791-147">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="82791-148">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="82791-148">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="82791-149">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="82791-149">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

