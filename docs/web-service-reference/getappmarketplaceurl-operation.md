---
title: Операция GetAppMarketplaceUrl
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2c016fc3-0e13-4624-9a5b-d3e84577a860
description: Поиск сведений о GetAppMarketplaceUrlной операции EWS.
ms.openlocfilehash: 616e7f571ba5283a773e51d611cd18bb37b5bc8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762689"
---
# <a name="getappmarketplaceurl-operation"></a><span data-ttu-id="d8925-103">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-103">GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="d8925-104">Поиск сведений о **GetAppMarketplaceUrlной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="d8925-104">Find information about the **GetAppMarketplaceUrl** EWS operation.</span></span> 
  
<span data-ttu-id="d8925-105">Операция **GetAppMarketplaceUrl** извлекает URL-адрес магазина приложений, который клиент может посетить для получения приложений для установки в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="d8925-105">The **GetAppMarketplaceUrl** operation retrieves the URL for the app marketplace that a client can visit to acquire apps to install in a mailbox.</span></span> 
  
<span data-ttu-id="d8925-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="d8925-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getappmarketplaceurl-operation"></a><span data-ttu-id="d8925-107">Использование операции GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-107">Using the GetAppMarketplaceUrl operation</span></span>

<span data-ttu-id="d8925-108">Операция **GetAppMarketplaceUrl** не имеет аргументов для запроса URL-адреса Marketplace, с которого клиент может устанавливать приложения.</span><span class="sxs-lookup"><span data-stu-id="d8925-108">The **GetAppMarketplaceUrl** operation does not take any arguments to request the URL for the marketplace from which a client can install apps.</span></span> <span data-ttu-id="d8925-109">Ответ будет содержать URL-адрес Marketplace для приложения.</span><span class="sxs-lookup"><span data-stu-id="d8925-109">The response will contain a URL to the app marketplace.</span></span> 
  
### <a name="getappmarketplaceurl-operation-soap-headers"></a><span data-ttu-id="d8925-110">Заголовки SOAP операции GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-110">GetAppMarketplaceUrl operation SOAP headers</span></span>

<span data-ttu-id="d8925-111">Операция **GetAppMarketplaceUrl** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="d8925-111">The **GetAppMarketplaceUrl** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d8925-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="d8925-112">**Header name**</span></span>|<span data-ttu-id="d8925-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d8925-113">**Element**</span></span>|<span data-ttu-id="d8925-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d8925-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d8925-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="d8925-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d8925-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="d8925-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d8925-117">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="d8925-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d8925-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="d8925-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d8925-119">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="d8925-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d8925-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="d8925-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d8925-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="d8925-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d8925-122">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="d8925-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getappmarketplaceurl-operation-request-example-get-the-app-marketplace-url-for-a-mailbox"></a><span data-ttu-id="d8925-123">Пример запроса операции GetAppMarketplaceUrl: получение URL-адреса магазина приложений для почтового ящика</span><span class="sxs-lookup"><span data-stu-id="d8925-123">GetAppMarketplaceUrl operation request example: Get the app marketplace URL for a mailbox</span></span>

<span data-ttu-id="d8925-124">В следующем примере запроса операции **GetAppMarketplaceUrl** показано, как получить URL-адрес рынка приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d8925-124">The following example of a **GetAppMarketplaceUrl** operation request shows how to get the app marketplace URL for a mailbox.</span></span> 
  
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

<span data-ttu-id="d8925-125">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d8925-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d8925-126">GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-126">GetAppMarketplaceUrl</span></span>](getappmarketplaceurl.md)
    
- [<span data-ttu-id="d8925-127">апиверсионсуппортед</span><span class="sxs-lookup"><span data-stu-id="d8925-127">ApiVersionSupported</span></span>](apiversionsupported.md)
    
- [<span data-ttu-id="d8925-128">счемаверсионсуппортед</span><span class="sxs-lookup"><span data-stu-id="d8925-128">SchemaVersionSupported</span></span>](schemaversionsupported.md)
    
## <a name="successful-getappmarketplaceurl-operation-response"></a><span data-ttu-id="d8925-129">Успешный отклик операции GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-129">Successful GetAppMarketplaceUrl operation response</span></span>

<span data-ttu-id="d8925-130">В следующем примере показан успешный ответ на запрос операции **GetAppMarketplaceUrl** для получения URL-адреса рынка приложений для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d8925-130">The following example shows a successful response to a **GetAppMarketplaceUrl** operation request to get the app marketplace URL for a mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d8925-131">URL-адрес магазина приложений изменен в целях сохранения читаемости.</span><span class="sxs-lookup"><span data-stu-id="d8925-131">The app marketplace URL has been altered to preserve readability.</span></span> 
  
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

<span data-ttu-id="d8925-132">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d8925-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d8925-133">жетаппмаркетплацеурлреспонсе</span><span class="sxs-lookup"><span data-stu-id="d8925-133">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="d8925-134">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d8925-134">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d8925-135">аппмаркетплацеурл</span><span class="sxs-lookup"><span data-stu-id="d8925-135">AppMarketplaceUrl</span></span>](appmarketplaceurl.md)
    
## <a name="getappmarketplaceurl-operation-error-response"></a><span data-ttu-id="d8925-136">Ответ об ошибке операции GetAppMarketPlaceUrl</span><span class="sxs-lookup"><span data-stu-id="d8925-136">GetAppMarketPlaceUrl operation error response</span></span>

<span data-ttu-id="d8925-137">Ошибки, возвращаемые для этой операции, связаны с неправильной конфигурацией службы или общими ошибками EWS.</span><span class="sxs-lookup"><span data-stu-id="d8925-137">Errors returned for this operation are either related to an incorrect service configuration or are generic EWS errors.</span></span> <span data-ttu-id="d8925-138">Коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="d8925-138">For error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span> 
  
<span data-ttu-id="d8925-139">В следующем примере показан ответ об ошибке, который возвращается, если внешняя панель управления Exchange (ECP) не настроена.</span><span class="sxs-lookup"><span data-stu-id="d8925-139">The following example shows an error response that is returned when external Exchange Control Panel (ECP) is not configured.</span></span>
  
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

<span data-ttu-id="d8925-140">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="d8925-140">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d8925-141">жетаппмаркетплацеурлреспонсе</span><span class="sxs-lookup"><span data-stu-id="d8925-141">GetAppMarketplaceUrlResponse</span></span>](getappmarketplaceurlresponse.md)
    
- [<span data-ttu-id="d8925-142">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="d8925-142">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="d8925-143">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="d8925-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="d8925-144">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="d8925-144">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="d8925-145">См. также</span><span class="sxs-lookup"><span data-stu-id="d8925-145">See also</span></span>

- [<span data-ttu-id="d8925-146">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="d8925-146">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="d8925-147">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="d8925-147">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="d8925-148">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="d8925-148">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="d8925-149">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="d8925-149">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="d8925-150">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="d8925-150">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    

