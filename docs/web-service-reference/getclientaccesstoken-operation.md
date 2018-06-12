---
title: Операция GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Найдите сведения о веб-служб Exchange GetClientAccessToken операции.
ms.openlocfilehash: afa9a315a8421f31c345c9547a5d80bed41e9fbc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762713"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="4afd5-103">Операция GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="4afd5-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="4afd5-104">Найдите сведения о **GetClientAccessToken** операции веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="4afd5-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="4afd5-105">Операция **GetClientAccessToken** получает клиентского доступа маркер для почтового приложения для Outlook.</span><span class="sxs-lookup"><span data-stu-id="4afd5-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="4afd5-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="4afd5-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="4afd5-107">С помощью операции GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="4afd5-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="4afd5-108">Запрос операции **GetClientAccessToken** использует два обязательных аргумента: идентификатор приложения и тип маркера.</span><span class="sxs-lookup"><span data-stu-id="4afd5-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="4afd5-109">[Операция GetAppManifests](getappmanifests-operation.md) можно использовать для запроса идентификатор приложения.</span><span class="sxs-lookup"><span data-stu-id="4afd5-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="4afd5-110">Заголовки SOAP GetClientAccessToken операции</span><span class="sxs-lookup"><span data-stu-id="4afd5-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="4afd5-111">Операция **GetClientAccessToken** можно использовать заголовки SOAP, которые перечислены в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="4afd5-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="4afd5-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="4afd5-112">**Header name**</span></span>|<span data-ttu-id="4afd5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4afd5-113">**Element**</span></span>|<span data-ttu-id="4afd5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4afd5-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4afd5-115">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="4afd5-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="4afd5-116">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4afd5-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4afd5-117">Определяет версию схемы для операции запроса.</span><span class="sxs-lookup"><span data-stu-id="4afd5-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="4afd5-118">Этот заголовок можно применять к запросу.</span><span class="sxs-lookup"><span data-stu-id="4afd5-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4afd5-119">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="4afd5-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="4afd5-120">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4afd5-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4afd5-121">Определяет версию сервера, ответившего на запрос.</span><span class="sxs-lookup"><span data-stu-id="4afd5-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="4afd5-122">Этот заголовок можно применять, чтобы получить ответ.</span><span class="sxs-lookup"><span data-stu-id="4afd5-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="4afd5-123">Пример запроса GetClientAccessToken операции: получение маркера удостоверения вызывающей стороны</span><span class="sxs-lookup"><span data-stu-id="4afd5-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="4afd5-124">Приведенный ниже запрос операции **GetClientAccessToken** показано, как получить маркер удостоверения вызывающей стороны для приложения.</span><span class="sxs-lookup"><span data-stu-id="4afd5-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:GetClientAccessToken>
         <m:TokenRequests>
            <t:TokenRequest>
               <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
               <t:TokenType>CallerIdentity</t:TokenType>
            </t:TokenRequest>
         </m:TokenRequests>
      </m:GetClientAccessToken>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="4afd5-125">Запрос SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4afd5-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4afd5-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="4afd5-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="4afd5-127">TokenRequests</span><span class="sxs-lookup"><span data-stu-id="4afd5-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="4afd5-128">TokenRequest</span><span class="sxs-lookup"><span data-stu-id="4afd5-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="4afd5-129">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="4afd5-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="4afd5-130">TokenType</span><span class="sxs-lookup"><span data-stu-id="4afd5-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="4afd5-131">Успешные операции ответа GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="4afd5-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="4afd5-132">В следующем примере показано успешного ответа на запрос операции **GetClientAccessToken** для получения маркера удостоверения вызывающей стороны для приложения.</span><span class="sxs-lookup"><span data-stu-id="4afd5-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4afd5-133">Для сохранения удобочитаемость URL были сокращены значения маркера в этой статье.</span><span class="sxs-lookup"><span data-stu-id="4afd5-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Token>
                  <t:Id>1C50226D-04B5-4AB2-9FCD-42E236B59E4B</t:Id>
                  <t:TokenType>CallerIdentity</t:TokenType>
                  <t:TokenValue>eyJ0eXAmv0QitaJg</t:TokenValue>
                  <t:TTL>479</t:TTL>
               </m:Token>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="4afd5-134">Ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4afd5-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4afd5-135">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="4afd5-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="4afd5-136">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4afd5-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4afd5-137">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4afd5-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="4afd5-138">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4afd5-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4afd5-139">Маркер (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="4afd5-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="4afd5-140">Идентификатор (строка)</span><span class="sxs-lookup"><span data-stu-id="4afd5-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="4afd5-141">TokenType (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="4afd5-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="4afd5-142">TokenValue</span><span class="sxs-lookup"><span data-stu-id="4afd5-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="4afd5-143">TTL (ClientAccessTokenTypeType)</span><span class="sxs-lookup"><span data-stu-id="4afd5-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="4afd5-144">Ошибка операции GetClientAccessToken ответа</span><span class="sxs-lookup"><span data-stu-id="4afd5-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="4afd5-145">В следующем примере показано ошибочный ответ на запрос операции **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="4afd5-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="4afd5-146">Это ответ на запрос для получения обратного вызова расширение маркеров без соответствующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="4afd5-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetClientAccessTokenResponseMessage ResponseClass="Error">
               <m:MessageText>The caller does not have enough permission for this token request.</m:MessageText>
               <m:ResponseCode>ErrorInvalidClientAccessTokenRequest</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:GetClientAccessTokenResponseMessage>
         </m:ResponseMessages>
      </m:GetClientAccessTokenResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4afd5-147">Ошибка ответ SOAP body содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="4afd5-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4afd5-148">GetClientAccessTokenResponse</span><span class="sxs-lookup"><span data-stu-id="4afd5-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="4afd5-149">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4afd5-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="4afd5-150">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4afd5-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="4afd5-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="4afd5-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="4afd5-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4afd5-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4afd5-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4afd5-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="4afd5-154">Дополнительные коды ошибок, которые являются общими для веб-служб Exchange и специально для этой операции в разделе [ResponseCode](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="4afd5-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="4afd5-155">См. также</span><span class="sxs-lookup"><span data-stu-id="4afd5-155">See also</span></span>

- [<span data-ttu-id="4afd5-156">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="4afd5-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="4afd5-157">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="4afd5-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="4afd5-158">Надстройки Outlook</span><span class="sxs-lookup"><span data-stu-id="4afd5-158">Outlook add-ins</span></span>](http://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

