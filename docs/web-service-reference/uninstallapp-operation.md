---
title: Операция UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Найдите сведения о веб-служб Exchange UninstallApp операции.
ms.openlocfilehash: 4f44224651993023336eef5540ec29b7f6a6e32e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840272"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="4e611-103">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="4e611-103">UninstallApp operation</span></span>

<span data-ttu-id="4e611-104">Найдите сведения о **UninstallApp** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4e611-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="4e611-105">Операция **UninstallApp** удаляет почтового приложения для Outlook.</span><span class="sxs-lookup"><span data-stu-id="4e611-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="4e611-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4e611-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="4e611-107">С помощью операции UninstallApp</span><span class="sxs-lookup"><span data-stu-id="4e611-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="4e611-108">Операция **UninstallApp** принимает один аргумент в запросе, идентифицирующее почтового приложения для удаления.</span><span class="sxs-lookup"><span data-stu-id="4e611-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="4e611-109">Заголовки SOAP UninstallApp операции</span><span class="sxs-lookup"><span data-stu-id="4e611-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="4e611-110">Операция **UninstallApp** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4e611-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="4e611-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="4e611-111">**Header name**</span></span>|<span data-ttu-id="4e611-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e611-112">**Element**</span></span>|<span data-ttu-id="4e611-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e611-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4e611-114">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="4e611-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="4e611-115">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4e611-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4e611-116">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="4e611-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="4e611-117">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="4e611-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4e611-118">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="4e611-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="4e611-119">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4e611-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4e611-120">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="4e611-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="4e611-121">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="4e611-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="4e611-122">Пример запроса UninstallApp операции: удаление почтового приложения в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="4e611-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="4e611-123">Приведенный ниже операции **UninstallApp** запроса показано, как для удаления почтового приложения с помощью идентификатора приложения.</span><span class="sxs-lookup"><span data-stu-id="4e611-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="4e611-124">Идентификатор приложения можно найти в манифесте приложения, который возвращается [GetAppManifests операции](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="4e611-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:UninstallApp>
         <m:ID>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</m:ID>
      </m:UninstallApp>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4e611-125">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4e611-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4e611-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="4e611-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="4e611-127">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="4e611-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="4e611-128">Успешные операции ответа UninstallApp</span><span class="sxs-lookup"><span data-stu-id="4e611-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="4e611-129">В следующем примере показано успешного ответа на запрос операции **UninstallApp** для удаления приложения электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4e611-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Success" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4e611-130">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4e611-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4e611-131">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="4e611-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="4e611-132">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4e611-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="4e611-133">Ошибка операции UninstallApp ответа</span><span class="sxs-lookup"><span data-stu-id="4e611-133">UninstallApp operation error response</span></span>

<span data-ttu-id="4e611-134">В следующем примере показано ошибочный ответ на запрос операции **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="4e611-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="4e611-135">Это ответ на запрос для удаления приложения электронной почты, который уже удалено.</span><span class="sxs-lookup"><span data-stu-id="4e611-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
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
      <UninstallAppResponse ResponseClass="Error" 
                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Extension ID 1c50226d-04b5-4ab2-9fcd-42e236b59e4b can't be found.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </UninstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4e611-136">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4e611-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4e611-137">UninstallAppResponse</span><span class="sxs-lookup"><span data-stu-id="4e611-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="4e611-138">MessageText</span><span class="sxs-lookup"><span data-stu-id="4e611-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4e611-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4e611-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4e611-140">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4e611-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="4e611-141">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="4e611-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4e611-142">См. также</span><span class="sxs-lookup"><span data-stu-id="4e611-142">See also</span></span>

- [<span data-ttu-id="4e611-143">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4e611-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="4e611-144">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="4e611-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="4e611-145">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="4e611-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="4e611-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="4e611-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="4e611-147">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="4e611-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

