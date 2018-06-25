---
title: Операция GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Найдите сведения о веб-служб Exchange GetAppMarketplaceUrl операции.
ms.openlocfilehash: 616e7f571ba5283a773e51d611cd18bb37b5bc8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762689"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="1ada9-103">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ada9-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="1ada9-104">Найдите сведения о **GetAppMarketplaceUrl** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ada9-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="1ada9-105">Операция **GetAppMarketplaceUrl** получает URL-адрес на рынке приложения, которые можно воспользоваться клиента для получения приложения для установки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="1ada9-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="1ada9-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="1ada9-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="1ada9-107">С помощью операции GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ada9-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="1ada9-108">Операция **GetAppMarketplaceUrl** не имеет аргументов, чтобы запросить URL-адрес для marketplace, из которого клиент может устанавливать приложения.</span><span class="sxs-lookup"><span data-stu-id="1ada9-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="1ada9-109">Ответ будет содержать URL-адрес приложения партнеров.</span><span class="sxs-lookup"><span data-stu-id="1ada9-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="1ada9-110">Заголовки SOAP GetAppMarketplaceUrl операции</span><span class="sxs-lookup"><span data-stu-id="1ada9-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="1ada9-111">Операция **GetAppMarketplaceUrl** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="1ada9-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="1ada9-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="1ada9-112">**Header name**</span></span>|<span data-ttu-id="1ada9-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1ada9-113">**Element**</span></span>|<span data-ttu-id="1ada9-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1ada9-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1ada9-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1ada9-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1ada9-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1ada9-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1ada9-117">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="1ada9-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1ada9-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="1ada9-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1ada9-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1ada9-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1ada9-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1ada9-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1ada9-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="1ada9-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1ada9-122">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="1ada9-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="1ada9-123">Пример запроса GetAppMarketplaceUrl операции: Получение URL-адрес приложения marketplace для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="1ada9-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="1ada9-124">Приведенный ниже запрос операции **GetAppMarketplaceUrl** показано, как получить URL-адрес приложения marketplace для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ada9-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
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
      <m:GetAppMarketplaceUrl>
        <m:ApiVersionSupported>1.0</m:ApiVersionSupported>
        <m:SchemaVersionSupported>1.0</m:SchemaVersionSupported>
      </m:GetAppMarketplaceUrl>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="1ada9-125">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1ada9-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1ada9-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ada9-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="1ada9-127">ApiVersionSupported</span><span class="sxs-lookup"><span data-stu-id="1ada9-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="1ada9-128">SchemaVersionSupported</span><span class="sxs-lookup"><span data-stu-id="1ada9-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="1ada9-129">Успешные операции ответа GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ada9-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="1ada9-130">В следующем примере показано успешного ответа на запрос операции **GetAppMarketplaceUrl** , чтобы получить URL-адрес приложения marketplace для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="1ada9-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="1ada9-131">URL-адрес приложения marketplace был изменен, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="1ada9-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Success" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <AppMarketplaceUrl>http://marketplace.contoso.com</AppMarketplaceUrl>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="1ada9-132">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1ada9-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1ada9-133">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="1ada9-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="1ada9-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1ada9-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1ada9-135">AppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="1ada9-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="1ada9-136">Ошибка операции GetAppMarketPlaceUrl ответа</span><span class="sxs-lookup"><span data-stu-id="1ada9-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="1ada9-137">Ошибок, возвращаемых для этой операции либо связанные с настройкой неправильные службы или универсальные ошибок веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="1ada9-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="1ada9-138">Коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="1ada9-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="1ada9-139">В следующем примере показано возврату ошибки, который возвращается при внешних панели управления Exchange (ECP) не настроен.</span><span class="sxs-lookup"><span data-stu-id="1ada9-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="918" 
                           MinorBuildNumber="7" 
                           Version="V2_10" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetAppMarketplaceUrlResponse ResponseClass="Error" 
                                    xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Cannot get external ECP URL. This might happen if external ECP URL isn't configured.</MessageText>
         <ResponseCode>ErrorCannotGetExternalEcpUrl</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetAppMarketplaceUrlResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1ada9-140">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1ada9-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1ada9-141">GetAppMarketplaceUrlResponse</span><span class="sxs-lookup"><span data-stu-id="1ada9-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="1ada9-142">MessageText</span><span class="sxs-lookup"><span data-stu-id="1ada9-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="1ada9-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1ada9-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1ada9-144">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1ada9-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="1ada9-145">См. также</span><span class="sxs-lookup"><span data-stu-id="1ada9-145">See also</span></span>

- [<span data-ttu-id="1ada9-146">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="1ada9-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="1ada9-147">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="1ada9-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="1ada9-148">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="1ada9-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="1ada9-149">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="1ada9-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="1ada9-150">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="1ada9-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

