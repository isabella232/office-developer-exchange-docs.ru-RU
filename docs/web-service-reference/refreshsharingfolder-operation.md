---
title: Операция RefreshSharingFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolder
api_type:
- schema
ms.assetid: 1b047e34-40f0-459f-ac9e-e9f8e7349479
description: Операция RefreshSharingFolder обновляет указанного локальную папку с использованием последних данных из папки "Общий".
ms.openlocfilehash: 0037de28f0720b97cd51c58a6ee7e3c06e84d642
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835041"
---
# <a name="refreshsharingfolder-operation"></a><span data-ttu-id="eb42c-103">Операция RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="eb42c-103">RefreshSharingFolder operation</span></span>

<span data-ttu-id="eb42c-104">Операция **RefreshSharingFolder** обновляет указанного локальную папку с использованием последних данных из папки "Общий".</span><span class="sxs-lookup"><span data-stu-id="eb42c-104">The **RefreshSharingFolder** operation refreshes the specified local folder with the latest data from the folder that is being shared.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="eb42c-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="eb42c-105">SOAP Headers</span></span>

<span data-ttu-id="eb42c-106">Операция **RefreshSharingFolder** можно использовать заголовки SOAP, которые перечислены и описаны в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="eb42c-106">The **RefreshSharingFolder** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="eb42c-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="eb42c-107">**Header**</span></span>|<span data-ttu-id="eb42c-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="eb42c-108">**Element**</span></span>|<span data-ttu-id="eb42c-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="eb42c-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="eb42c-110">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="eb42c-110">RequestVersion</span></span>  <br/> |[<span data-ttu-id="eb42c-111">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="eb42c-111">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="eb42c-112">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="eb42c-112">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="eb42c-113">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="eb42c-113">ServerVersion</span></span>  <br/> |[<span data-ttu-id="eb42c-114">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eb42c-114">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="eb42c-115">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="eb42c-115">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="refreshsharingfolder-request-example"></a><span data-ttu-id="eb42c-116">Пример запроса RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="eb42c-116">RefreshSharingFolder request example</span></span>

### <a name="description"></a><span data-ttu-id="eb42c-117">Описание</span><span class="sxs-lookup"><span data-stu-id="eb42c-117">Description</span></span>

<span data-ttu-id="eb42c-118">Следующем примере показано, как для формирования запроса для обновления указанного локальную папку с использованием последних данных из папки "Общий".</span><span class="sxs-lookup"><span data-stu-id="eb42c-118">The following example shows how to form a request to refresh the specified local folder with the latest data from the folder that is being shared.</span></span> <span data-ttu-id="eb42c-119">Элемент [SharingFolderId](sharingfolderid.md) указывает идентификатор локальной папки необходимо обновить.</span><span class="sxs-lookup"><span data-stu-id="eb42c-119">The [SharingFolderId](sharingfolderid.md) element specifies the identifier of the local folder to be refreshed.</span></span> 
  
### <a name="code"></a><span data-ttu-id="eb42c-120">Программа</span><span class="sxs-lookup"><span data-stu-id="eb42c-120">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolder xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:SharingFolderId Id="AAMkAD=" ChangeKey="AwAAA=" />
    </RefreshSharingFolder>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="eb42c-121">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="eb42c-121">Request elements</span></span>

<span data-ttu-id="eb42c-122">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eb42c-122">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="eb42c-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="eb42c-123">RequestServerVersion</span></span>](requestserverversion.md)
    
- [<span data-ttu-id="eb42c-124">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="eb42c-124">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
    
- [<span data-ttu-id="eb42c-125">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="eb42c-125">SharingFolderId</span></span>](sharingfolderid.md)
    
## <a name="successful-refreshsharingfolder-response"></a><span data-ttu-id="eb42c-126">Успешного ответа RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="eb42c-126">Successful RefreshSharingFolder Response</span></span>

### <a name="description"></a><span data-ttu-id="eb42c-127">Описание</span><span class="sxs-lookup"><span data-stu-id="eb42c-127">Description</span></span>

<span data-ttu-id="eb42c-128">В следующем примере показано успешного ответа на запрос **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="eb42c-128">The following example shows a successful response to a **RefreshSharingFolder** request.</span></span> 
  
### <a name="code"></a><span data-ttu-id="eb42c-129">Программа</span><span class="sxs-lookup"><span data-stu-id="eb42c-129">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Success"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseCode>NoError</m:ResponseCode>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a><span data-ttu-id="eb42c-130">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="eb42c-130">Successful response elements</span></span>

<span data-ttu-id="eb42c-131">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eb42c-131">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="eb42c-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eb42c-132">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eb42c-133">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb42c-133">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="eb42c-134">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eb42c-134">ResponseCode</span></span>](responsecode.md)
    
## <a name="refreshsharingfolder-error-response"></a><span data-ttu-id="eb42c-135">Ошибка RefreshSharingFolder ответа</span><span class="sxs-lookup"><span data-stu-id="eb42c-135">RefreshSharingFolder error response</span></span>

### <a name="description"></a><span data-ttu-id="eb42c-136">Описание</span><span class="sxs-lookup"><span data-stu-id="eb42c-136">Description</span></span>

<span data-ttu-id="eb42c-137">В следующем примере показано ошибочный ответ на запрос **RefreshSharingFolder** .</span><span class="sxs-lookup"><span data-stu-id="eb42c-137">The following example shows an error response to a **RefreshSharingFolder** request.</span></span> <span data-ttu-id="eb42c-138">В этом примере **RefreshSharingFolder** не удалось выполнить запрос, поскольку не найден подписки, соответствующий указанной локальной папке.</span><span class="sxs-lookup"><span data-stu-id="eb42c-138">In this example, the **RefreshSharingFolder** request failed because a subscription that corresponds to the specified local folder was not found.</span></span> 
  
### <a name="code"></a><span data-ttu-id="eb42c-139">Программа</span><span class="sxs-lookup"><span data-stu-id="eb42c-139">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <RefreshSharingFolderResponseMessage ResponseClass="Error"
                                xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:MessageText>Failed to synchronize the sharing folder.</m:MessageText>
      <m:ResponseCode>ErrorSharingSynchronizationFailed</m:ResponseCode>
      <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
      <m:MessageXml>
        <t:Value Name="ErrorDetails">Microsoft.Exchange.InfoWorker.Common.Sharing.SubscriptionNotFoundException: The subscription wasn't found.;</t:Value>
      </m:MessageXml>
    </RefreshSharingFolderResponseMessage>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a><span data-ttu-id="eb42c-140">Элементы ответа об ошибках</span><span class="sxs-lookup"><span data-stu-id="eb42c-140">Error response elements</span></span>

<span data-ttu-id="eb42c-141">В ответ на ошибку используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="eb42c-141">The following elements are used in the error response:</span></span>
  
- [<span data-ttu-id="eb42c-142">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="eb42c-142">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="eb42c-143">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb42c-143">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
    
- [<span data-ttu-id="eb42c-144">MessageText</span><span class="sxs-lookup"><span data-stu-id="eb42c-144">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="eb42c-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eb42c-145">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="eb42c-146">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="eb42c-146">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="eb42c-147">MessageXml</span><span class="sxs-lookup"><span data-stu-id="eb42c-147">MessageXml</span></span>](messagexml.md)
    
## <a name="see-also"></a><span data-ttu-id="eb42c-148">См. также</span><span class="sxs-lookup"><span data-stu-id="eb42c-148">See also</span></span>



[<span data-ttu-id="eb42c-149">RefreshSharingFolder</span><span class="sxs-lookup"><span data-stu-id="eb42c-149">RefreshSharingFolder</span></span>](refreshsharingfolder.md)
  
[<span data-ttu-id="eb42c-150">RefreshSharingFolderType</span><span class="sxs-lookup"><span data-stu-id="eb42c-150">RefreshSharingFolderType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderType.aspx)
  
[<span data-ttu-id="eb42c-151">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb42c-151">RefreshSharingFolderResponseMessage</span></span>](refreshsharingfolderresponsemessage.md)
  
[<span data-ttu-id="eb42c-152">RefreshSharingFolderResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="eb42c-152">RefreshSharingFolderResponseMessageType</span></span>](https://msdn.microsoft.com/library/ExchangeWebServices.RefreshSharingFolderResponseMessageType.aspx)


[<span data-ttu-id="eb42c-153">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="eb42c-153">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="eb42c-154">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="eb42c-154">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

