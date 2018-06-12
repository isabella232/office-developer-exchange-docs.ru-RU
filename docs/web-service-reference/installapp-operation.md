---
title: Операция InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Найдите сведения о веб-служб Exchange InstallApp операции.
ms.openlocfilehash: ccc5d2dde949070bae905ff1ebb182c892f07fcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833951"
---
# <a name="installapp-operation"></a><span data-ttu-id="7ed47-103">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-103">InstallApp operation</span></span>

<span data-ttu-id="7ed47-104">Найдите сведения о **InstallApp** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="7ed47-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="7ed47-105">Операция **InstallApp** устанавливает почтовое приложение для Outlook в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="7ed47-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="7ed47-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="7ed47-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="7ed47-107">С помощью операции InstallApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-107">Using the InstallApp operation</span></span>

<span data-ttu-id="7ed47-108">Операция **InstallApp** принимает один аргумент, определяющий почтового приложения для установки.</span><span class="sxs-lookup"><span data-stu-id="7ed47-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="7ed47-109">Аргумент содержит кодировки Base64 манифеста для почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="7ed47-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="7ed47-110">Заголовки SOAP InstallApp операции</span><span class="sxs-lookup"><span data-stu-id="7ed47-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="7ed47-111">Операция **InstallApp** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="7ed47-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7ed47-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="7ed47-112">**Header name**</span></span>|<span data-ttu-id="7ed47-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7ed47-113">**Element**</span></span>|<span data-ttu-id="7ed47-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7ed47-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ed47-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7ed47-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7ed47-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7ed47-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7ed47-117">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="7ed47-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7ed47-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="7ed47-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ed47-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7ed47-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7ed47-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7ed47-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7ed47-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="7ed47-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7ed47-122">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="7ed47-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="7ed47-123">Пример запроса InstallApp операции: установки почтового приложения в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="7ed47-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="7ed47-124">В следующем примере запрос операции **InstallApp** показано, как установить почтовое приложение для Outlook.</span><span class="sxs-lookup"><span data-stu-id="7ed47-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="7ed47-125">Манифест приложения можно найти с помощью [операции GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="7ed47-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="7ed47-126">Манифест приложения в кодировке base64 произвольно усечен, чтобы сохранить возможность чтения и не представляет допустимое манифеста.</span><span class="sxs-lookup"><span data-stu-id="7ed47-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:InstallApp>
         <m:Manifest>TUwiIC8+CiAgPC9SdWxlPgo8L09mZmljZUFwcD4=</m:Manifest>
      </m:InstallApp>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="7ed47-127">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7ed47-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ed47-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="7ed47-129">Манифест</span><span class="sxs-lookup"><span data-stu-id="7ed47-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="7ed47-130">Успешные операции ответа InstallApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="7ed47-131">В следующем примере показано успешного ответа на запрос операции **InstallApp** для установки почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="7ed47-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7ed47-132">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7ed47-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ed47-133">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7ed47-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="7ed47-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ed47-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="7ed47-135">Ошибка операции InstallApp ответа</span><span class="sxs-lookup"><span data-stu-id="7ed47-135">InstallApp operation error response</span></span>

<span data-ttu-id="7ed47-136">В следующем примере показано ошибочный ответ на запрос операции **InstallApp** .</span><span class="sxs-lookup"><span data-stu-id="7ed47-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="7ed47-137">Это ответ на запрос, который содержит недопустимый манифест.</span><span class="sxs-lookup"><span data-stu-id="7ed47-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="7ed47-138">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="7ed47-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ed47-139">InstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="7ed47-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="7ed47-140">MessageText</span><span class="sxs-lookup"><span data-stu-id="7ed47-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7ed47-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ed47-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7ed47-142">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7ed47-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7ed47-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7ed47-143">See also</span></span>

- [<span data-ttu-id="7ed47-144">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="7ed47-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7ed47-145">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="7ed47-146">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="7ed47-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="7ed47-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="7ed47-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="7ed47-148">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="7ed47-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

