---
title: Операция UninstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7707aa6a-381d-43f7-a454-54f6343ed127
description: Поиск сведений о UninstallAppной операции EWS.
ms.openlocfilehash: 4f44224651993023336eef5540ec29b7f6a6e32e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840272"
---
# <a name="uninstallapp-operation"></a><span data-ttu-id="5e6e4-103">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-103">UninstallApp operation</span></span>

<span data-ttu-id="5e6e4-104">Поиск сведений о **UninstallAppной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-104">Find information about the **UninstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="5e6e4-105">При выполнении операции **UninstallApp** удаляется почтовое приложение для Outlook.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-105">The **UninstallApp** operation uninstalls a mail app for Outlook.</span></span> 
  
<span data-ttu-id="5e6e4-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-uninstallapp-operation"></a><span data-ttu-id="5e6e4-107">Использование операции UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-107">Using the UninstallApp operation</span></span>

<span data-ttu-id="5e6e4-108">Операция **UninstallApp** принимает в запросе один аргумент, идентифицирующий почтовое приложение, которое требуется удалить.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-108">The **UninstallApp** operation takes one argument in the request that identifies the mail app to uninstall.</span></span> 
  
### <a name="uninstallapp-operation-soap-headers"></a><span data-ttu-id="5e6e4-109">Заголовки SOAP операции UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-109">UninstallApp operation SOAP headers</span></span>

<span data-ttu-id="5e6e4-110">Операция **UninstallApp** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-110">The **UninstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="5e6e4-111">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="5e6e4-111">**Header name**</span></span>|<span data-ttu-id="5e6e4-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5e6e4-112">**Element**</span></span>|<span data-ttu-id="5e6e4-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5e6e4-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e6e4-114">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="5e6e4-114">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="5e6e4-115">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="5e6e4-115">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="5e6e4-116">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-116">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="5e6e4-117">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="5e6e4-118">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="5e6e4-118">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="5e6e4-119">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="5e6e4-119">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="5e6e4-120">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-120">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="5e6e4-121">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-121">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="uninstallapp-operation-request-example-uninstall-a-mail-app-in-a-mailbox"></a><span data-ttu-id="5e6e4-122">Пример запроса операции UninstallApp: Удаление почтового приложения в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="5e6e4-122">UninstallApp operation request example: Uninstall a mail app in a mailbox</span></span>

<span data-ttu-id="5e6e4-123">В следующем примере запроса операции **UninstallApp** показано, как удалить почтовое приложение с помощью идентификатора приложения.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-123">The following example of an **UninstallApp** operation request shows how to a uninstall a mail app by using the app identifier.</span></span> <span data-ttu-id="5e6e4-124">Идентификатор приложения можно найти в манифесте приложения, возвращенном [операцией GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e4-124">The app identifier can be found in the app manifest that is returned by the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
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

<span data-ttu-id="5e6e4-125">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5e6e4-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e6e4-126">UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-126">UninstallApp</span></span>](uninstallapp.md)
    
- [<span data-ttu-id="5e6e4-127">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="5e6e4-127">ID (String)</span></span>](id-string.md)
    
## <a name="successful-uninstallapp-operation-response"></a><span data-ttu-id="5e6e4-128">Успешный отклик операции UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-128">Successful UninstallApp operation response</span></span>

<span data-ttu-id="5e6e4-129">В следующем примере показан успешный ответ на запрос операции **UninstallApp** для удаления почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-129">The following example shows a successful response to an **UninstallApp** operation request to uninstall a mail app.</span></span> 
  
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

<span data-ttu-id="5e6e4-130">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5e6e4-130">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e6e4-131">унинсталлаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="5e6e4-131">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="5e6e4-132">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5e6e4-132">ResponseCode</span></span>](responsecode.md)
    
## <a name="uninstallapp-operation-error-response"></a><span data-ttu-id="5e6e4-133">Ответ об ошибке операции UninstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-133">UninstallApp operation error response</span></span>

<span data-ttu-id="5e6e4-134">В следующем примере показан ответ об ошибке для запроса операции **UninstallApp** .</span><span class="sxs-lookup"><span data-stu-id="5e6e4-134">The following example shows an error response to an **UninstallApp** operation request.</span></span> <span data-ttu-id="5e6e4-135">Это ответ на запрос на удаление почтового приложения, которое уже удалено.</span><span class="sxs-lookup"><span data-stu-id="5e6e4-135">This is a response to a request to uninstall a mail app that has already been uninstalled.</span></span> 
  
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

<span data-ttu-id="5e6e4-136">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5e6e4-136">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="5e6e4-137">унинсталлаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="5e6e4-137">UninstallAppResponse</span></span>](uninstallappresponse.md)
    
- [<span data-ttu-id="5e6e4-138">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="5e6e4-138">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="5e6e4-139">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="5e6e4-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5e6e4-140">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="5e6e4-140">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="5e6e4-141">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="5e6e4-141">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="5e6e4-142">См. также</span><span class="sxs-lookup"><span data-stu-id="5e6e4-142">See also</span></span>

- [<span data-ttu-id="5e6e4-143">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="5e6e4-143">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="5e6e4-144">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-144">InstallApp operation</span></span>](installapp-operation.md)
    
- [<span data-ttu-id="5e6e4-145">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="5e6e4-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="5e6e4-146">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="5e6e4-146">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="5e6e4-147">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="5e6e4-147">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

