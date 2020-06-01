---
title: Операция GetClientAccessToken
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 086876cc-e22c-4e89-89f9-19e78af51217
description: Поиск сведений о GetClientAccessTokenной операции EWS.
ms.openlocfilehash: 2d49d675fcedb0e7e8312a9715f095c47fcf3d77
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462040"
---
# <a name="getclientaccesstoken-operation"></a><span data-ttu-id="bb57c-103">Операция GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-103">GetClientAccessToken operation</span></span>

<span data-ttu-id="bb57c-104">Поиск сведений о **GetClientAccessTokenной** операции EWS.</span><span class="sxs-lookup"><span data-stu-id="bb57c-104">Find information about the **GetClientAccessToken** EWS operation.</span></span> 
  
<span data-ttu-id="bb57c-105">Операция **GetClientAccessToken** получает маркер клиентского доступа для почтового приложения для Outlook.</span><span class="sxs-lookup"><span data-stu-id="bb57c-105">The **GetClientAccessToken** operation gets a client access token for a mail app for Outlook.</span></span> 
  
<span data-ttu-id="bb57c-106">Эта операция появилась в Exchange Server 2013.</span><span class="sxs-lookup"><span data-stu-id="bb57c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getclientaccesstoken-operation"></a><span data-ttu-id="bb57c-107">Использование операции GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-107">Using the GetClientAccessToken operation</span></span>

<span data-ttu-id="bb57c-108">Запрос операции **GetClientAccessToken** принимает два обязательных аргумента: идентификатор приложения и тип маркера.</span><span class="sxs-lookup"><span data-stu-id="bb57c-108">The **GetClientAccessToken** operation request takes two required arguments: the identifier of the app, and the token type.</span></span> <span data-ttu-id="bb57c-109">Для запроса идентификатора приложения можно использовать [операцию GetAppManifests](getappmanifests-operation.md) .</span><span class="sxs-lookup"><span data-stu-id="bb57c-109">You can use the [GetAppManifests operation](getappmanifests-operation.md) to request the app identifier.</span></span> 
  
### <a name="getclientaccesstoken-operation-soap-headers"></a><span data-ttu-id="bb57c-110">Заголовки SOAP операции GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-110">GetClientAccessToken operation SOAP headers</span></span>

<span data-ttu-id="bb57c-111">Операция **GetClientAccessToken** может использовать заголовки SOAP, указанные в приведенной ниже таблице.</span><span class="sxs-lookup"><span data-stu-id="bb57c-111">The **GetClientAccessToken** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="bb57c-112">**Имя заголовка**</span><span class="sxs-lookup"><span data-stu-id="bb57c-112">**Header name**</span></span>|<span data-ttu-id="bb57c-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bb57c-113">**Element**</span></span>|<span data-ttu-id="bb57c-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bb57c-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bb57c-115">**рекуестверсион**</span><span class="sxs-lookup"><span data-stu-id="bb57c-115">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="bb57c-116">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="bb57c-116">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="bb57c-117">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="bb57c-117">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="bb57c-118">Этот заголовок является применимым для запроса.</span><span class="sxs-lookup"><span data-stu-id="bb57c-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="bb57c-119">**серверверсион**</span><span class="sxs-lookup"><span data-stu-id="bb57c-119">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="bb57c-120">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="bb57c-120">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="bb57c-121">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="bb57c-121">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="bb57c-122">Этот заголовок является применимым для отклика.</span><span class="sxs-lookup"><span data-stu-id="bb57c-122">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getclientaccesstoken-operation-request-example-get-a-caller-identity-token"></a><span data-ttu-id="bb57c-123">Пример запроса операции GetClientAccessToken: получение маркера удостоверения звонящего</span><span class="sxs-lookup"><span data-stu-id="bb57c-123">GetClientAccessToken operation request example: Get a caller identity token</span></span>

<span data-ttu-id="bb57c-124">В следующем примере запроса операции **GetClientAccessToken** показано, как получить маркер удостоверения звонящего для приложения.</span><span class="sxs-lookup"><span data-stu-id="bb57c-124">The following example of a **GetClientAccessToken** operation request shows how to get a caller identity token for an app.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="bb57c-125">Текст SOAP Request содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bb57c-125">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb57c-126">GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-126">GetClientAccessToken</span></span>](getclientaccesstoken.md)
    
- [<span data-ttu-id="bb57c-127">токенрекуестс</span><span class="sxs-lookup"><span data-stu-id="bb57c-127">TokenRequests</span></span>](tokenrequests.md)
    
- [<span data-ttu-id="bb57c-128">токенрекуест</span><span class="sxs-lookup"><span data-stu-id="bb57c-128">TokenRequest</span></span>](tokenrequest.md)
    
- [<span data-ttu-id="bb57c-129">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="bb57c-129">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="bb57c-130">токентипе</span><span class="sxs-lookup"><span data-stu-id="bb57c-130">TokenType</span></span>](tokentype.md)
    
## <a name="successful-getclientaccesstoken-operation-response"></a><span data-ttu-id="bb57c-131">Успешный отклик операции GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-131">Successful GetClientAccessToken operation response</span></span>

<span data-ttu-id="bb57c-132">В следующем примере показан успешный ответ на запрос операции **GetClientAccessToken** для получения маркера удостоверения вызывающего абонента для приложения.</span><span class="sxs-lookup"><span data-stu-id="bb57c-132">The following example shows a successful response to a **GetClientAccessToken** operation request to get a caller identity token for an app.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="bb57c-133">Значения маркеров, приведенные в этой статье, были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="bb57c-133">The token values in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="bb57c-134">Тело SOAP отклика содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bb57c-134">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb57c-135">жетклиентакцесстокенреспонсе</span><span class="sxs-lookup"><span data-stu-id="bb57c-135">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="bb57c-136">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bb57c-136">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bb57c-137">жетклиентакцесстокенреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bb57c-137">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="bb57c-138">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bb57c-138">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bb57c-139">Маркер (Клиентакцесстокентипе)</span><span class="sxs-lookup"><span data-stu-id="bb57c-139">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md)
    
- [<span data-ttu-id="bb57c-140">ID (строка)</span><span class="sxs-lookup"><span data-stu-id="bb57c-140">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="bb57c-141">Токентипе (Клиентакцесстокентипе)</span><span class="sxs-lookup"><span data-stu-id="bb57c-141">TokenType (ClientAccessTokenType)</span></span>](tokentype-clientaccesstokentype.md)
    
- [<span data-ttu-id="bb57c-142">токенвалуе</span><span class="sxs-lookup"><span data-stu-id="bb57c-142">TokenValue</span></span>](tokenvalue.md)
    
- [<span data-ttu-id="bb57c-143">TTL (Клиентакцесстокентипетипе)</span><span class="sxs-lookup"><span data-stu-id="bb57c-143">TTL (ClientAccessTokenTypeType)</span></span>](ttl-clientaccesstokentypetype.md)
    
## <a name="getclientaccesstoken-operation-error-response"></a><span data-ttu-id="bb57c-144">Ответ об ошибке операции GetClientAccessToken</span><span class="sxs-lookup"><span data-stu-id="bb57c-144">GetClientAccessToken operation error response</span></span>

<span data-ttu-id="bb57c-145">В следующем примере показан ответ об ошибке для запроса операции **GetClientAccessToken** .</span><span class="sxs-lookup"><span data-stu-id="bb57c-145">The following example shows an error response to a **GetClientAccessToken** operation request.</span></span> <span data-ttu-id="bb57c-146">Это ответ на запрос на получение маркера обратного вызова расширения без соответствующих разрешений.</span><span class="sxs-lookup"><span data-stu-id="bb57c-146">This is a response to a request to get an extension callback token without the appropriate permissions.</span></span> 
  
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
      <m:GetClientAccessTokenResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="bb57c-147">Основной текст сообщения об ошибке SOAP содержит следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="bb57c-147">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="bb57c-148">жетклиентакцесстокенреспонсе</span><span class="sxs-lookup"><span data-stu-id="bb57c-148">GetClientAccessTokenResponse</span></span>](getclientaccesstokenresponse.md)
    
- [<span data-ttu-id="bb57c-149">респонсемессажес</span><span class="sxs-lookup"><span data-stu-id="bb57c-149">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="bb57c-150">жетклиентакцесстокенреспонсемессаже</span><span class="sxs-lookup"><span data-stu-id="bb57c-150">GetClientAccessTokenResponseMessage</span></span>](getclientaccesstokenresponsemessage.md)
    
- [<span data-ttu-id="bb57c-151">мессажетекст</span><span class="sxs-lookup"><span data-stu-id="bb57c-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="bb57c-152">респонсекоде</span><span class="sxs-lookup"><span data-stu-id="bb57c-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="bb57c-153">дескриптивелинккэй</span><span class="sxs-lookup"><span data-stu-id="bb57c-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="bb57c-154">Дополнительные коды ошибок, которые являются общими для EWS и специфичными для этой операции, можно найти в разделе [респонсекоде](responsecode.md).</span><span class="sxs-lookup"><span data-stu-id="bb57c-154">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="bb57c-155">См. также</span><span class="sxs-lookup"><span data-stu-id="bb57c-155">See also</span></span>

- [<span data-ttu-id="bb57c-156">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="bb57c-156">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="bb57c-157">Операция GetAppManifests</span><span class="sxs-lookup"><span data-stu-id="bb57c-157">GetAppManifests operation</span></span>](getappmanifests-operation.md)
    
- [<span data-ttu-id="bb57c-158">Надстройки Outlook</span><span class="sxs-lookup"><span data-stu-id="bb57c-158">Outlook add-ins</span></span>](https://msdn.microsoft.com/library/71e64bc9-e347-4f5d-8948-0a47b5dd93e6%28Office.15%29.aspx)
    

