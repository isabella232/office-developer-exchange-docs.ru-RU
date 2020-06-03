---
title: Операция InstallApp
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 596eae95-3e78-489a-8bb2-d2dd4a026405
description: Поиск сведений о InstallAppной операции EWS.
ms.openlocfilehash: ae6aab7f7176aa827bafa9abf1aa67d458d309d2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465690"
---
# <a name="installapp-operation"></a><span data-ttu-id="3d428-103">Операция InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-103">InstallApp operation</span></span>

<span data-ttu-id="3d428-104">Поиск сведений о **InstallAppной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="3d428-104">Find information about the **InstallApp** EWS operation.</span></span> 
  
<span data-ttu-id="3d428-105">Операция **InstallAPP** устанавливает почтовое приложение для Outlook в почтовом ящике.</span><span class="sxs-lookup"><span data-stu-id="3d428-105">The **InstallApp** operation installs a mail app for Outlook in a mailbox.</span></span> 
  
<span data-ttu-id="3d428-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="3d428-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-installapp-operation"></a><span data-ttu-id="3d428-107">Использование операции InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-107">Using the InstallApp operation</span></span>

<span data-ttu-id="3d428-108">Операция **InstallAPP** принимает в качестве аргумента один аргумент, определяющий устанавливаемое почтовое приложение.</span><span class="sxs-lookup"><span data-stu-id="3d428-108">The **InstallApp** operation takes a single argument that identifies a mail app to install.</span></span> <span data-ttu-id="3d428-109">Аргумент содержит манифест с кодировкой base64 для почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="3d428-109">The argument contains the base64-encoded manifest for a mail app.</span></span> 
  
### <a name="installapp-operation-soap-headers"></a><span data-ttu-id="3d428-110">Заголовки SOAP операции InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-110">InstallApp operation SOAP headers</span></span>

<span data-ttu-id="3d428-111">Операция **InstallAPP** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="3d428-111">The **InstallApp** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="3d428-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="3d428-112">**Header name**</span></span>|<span data-ttu-id="3d428-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3d428-113">**Element**</span></span>|<span data-ttu-id="3d428-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3d428-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3d428-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="3d428-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3d428-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="3d428-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3d428-117">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="3d428-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3d428-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="3d428-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3d428-119">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="3d428-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3d428-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="3d428-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3d428-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="3d428-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3d428-122">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="3d428-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="installapp-operation-request-example-install-a-mail-app-in-a-mailbox"></a><span data-ttu-id="3d428-123">Пример запроса операции InstallApp: Установка почтового приложения в почтовом ящике</span><span class="sxs-lookup"><span data-stu-id="3d428-123">InstallApp operation request example: Install a mail app in a mailbox</span></span>

<span data-ttu-id="3d428-124">В следующем примере запроса операции **InstallAPP** показано, как установить почтовое приложение для Outlook.</span><span class="sxs-lookup"><span data-stu-id="3d428-124">The following example of an **InstallApp** operation request shows how to install a mail app for Outlook.</span></span> <span data-ttu-id="3d428-125">Манифест приложения можно найти с помощью [операции GetAppManifests](getappmanifests-operation.md).</span><span class="sxs-lookup"><span data-stu-id="3d428-125">The app manifest can be found by using the [GetAppManifests operation](getappmanifests-operation.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="3d428-126">Манифест приложения в кодировке Base64 произвольно усечен, чтобы сохранить удобочитаемость и не представляет допустимый манифест.</span><span class="sxs-lookup"><span data-stu-id="3d428-126">The base64-encoded app manifest has been arbitrarily truncated to preserve readability and does not represent a valid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="3d428-127">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3d428-127">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3d428-128">InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-128">InstallApp</span></span>](installapp.md)
    
- [<span data-ttu-id="3d428-129">Манифест</span><span class="sxs-lookup"><span data-stu-id="3d428-129">Manifest</span></span>](manifest.md)
    
## <a name="successful-installapp-operation-response"></a><span data-ttu-id="3d428-130">Успешный отклик операции InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-130">Successful InstallApp operation response</span></span>

<span data-ttu-id="3d428-131">В следующем примере показан успешный ответ на запрос операции **InstallAPP** для установки почтового приложения.</span><span class="sxs-lookup"><span data-stu-id="3d428-131">The following example shows a successful response to an **InstallApp** operation request to install a mail app.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3d428-132">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3d428-132">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3d428-133">инсталлаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="3d428-133">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="3d428-134">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3d428-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="installapp-operation-error-response"></a><span data-ttu-id="3d428-135">Ответ об ошибке операции InstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-135">InstallApp operation error response</span></span>

<span data-ttu-id="3d428-136">В следующем примере показан ответ об ошибке для запроса операции **InstallAPP** .</span><span class="sxs-lookup"><span data-stu-id="3d428-136">The following example shows an error response to an **InstallApp** operation request.</span></span> <span data-ttu-id="3d428-137">Это ответ на запрос, который содержит недопустимый манифест.</span><span class="sxs-lookup"><span data-stu-id="3d428-137">This is a response to a request that contains an invalid manifest.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="14" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <InstallAppResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>This app can't be installed. Missing OfficeApp element.</MessageText>
         <ResponseCode>ErrorInternalServerError</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </InstallAppResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="3d428-138">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="3d428-138">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3d428-139">инсталлаппреспонсе</span><span class="sxs-lookup"><span data-stu-id="3d428-139">InstallAppResponse</span></span>](installappresponse.md)
    
- [<span data-ttu-id="3d428-140">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="3d428-140">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="3d428-141">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="3d428-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3d428-142">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="3d428-142">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="3d428-143">См. также</span><span class="sxs-lookup"><span data-stu-id="3d428-143">See also</span></span>

- [<span data-ttu-id="3d428-144">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="3d428-144">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="3d428-145">Операция DisableApp</span><span class="sxs-lookup"><span data-stu-id="3d428-145">DisableApp operation</span></span>](disableapp-operation.md)
    
- [<span data-ttu-id="3d428-146">Операция UninstallApp</span><span class="sxs-lookup"><span data-stu-id="3d428-146">UninstallApp operation</span></span>](uninstallapp-operation.md)
    
- [<span data-ttu-id="3d428-147">GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="3d428-147">GetAppManifests</span></span>](getappmanifests.md)
    
- [<span data-ttu-id="3d428-148">Операция GetAppMarketplaceUrl</span><span class="sxs-lookup"><span data-stu-id="3d428-148">GetAppMarketplaceUrl operation</span></span>](getappmarketplaceurl-operation.md)
    

