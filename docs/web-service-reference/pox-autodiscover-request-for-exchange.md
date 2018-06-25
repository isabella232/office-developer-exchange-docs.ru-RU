---
title: Запрос автообнаружения POX для Exchange
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 75671b1d-f35b-497b-8d8c-706f3f2535fd
description: Запрос автообнаружения содержит запросов для настройки доступа пользователя клиента.
ms.openlocfilehash: 48d6c30946e75936ed93a6f4507d8a8d3ae47d40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834865"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="1c258-103">Запрос автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="1c258-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="1c258-104">Запрос автообнаружения содержит запросов для настройки доступа пользователя клиента.</span><span class="sxs-lookup"><span data-stu-id="1c258-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="1c258-105">Пример запроса службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1c258-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="1c258-106">Описание</span><span class="sxs-lookup"><span data-stu-id="1c258-106">Description</span></span>

<span data-ttu-id="1c258-107">В следующем примере XML показано тело запроса службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1c258-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="1c258-108">Программа</span><span class="sxs-lookup"><span data-stu-id="1c258-108">Code</span></span>

```XML
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="1c258-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="1c258-109">Request Headers</span></span>

<span data-ttu-id="1c258-110">Следующие заголовки HTTP не являются обязательными при отправке запросов автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1c258-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="1c258-111">**В таблице 1. Заголовки HTTP-запроса**</span><span class="sxs-lookup"><span data-stu-id="1c258-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="1c258-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="1c258-112">**Header**</span></span>|<span data-ttu-id="1c258-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1c258-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1c258-114">X-MapiHttpCapability</span><span class="sxs-lookup"><span data-stu-id="1c258-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="1c258-115">Если этот параметр указан и задайте значение «1» указывает, что клиент запрашивает сведения, которые можно использовать для подключения к серверу с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1c258-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="1c258-116">Этот заголовок можно применять для клиентов, использующих протокол MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1c258-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="1c258-117">X-ClientCanHandle</span><span class="sxs-lookup"><span data-stu-id="1c258-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="1c258-118">Этот заголовок содержит список разделенных запятой возможности, поддерживаемые клиентом.</span><span class="sxs-lookup"><span data-stu-id="1c258-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="1c258-119">Допустимые значения указаны в таблице 2.</span><span class="sxs-lookup"><span data-stu-id="1c258-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="1c258-120">**В таблице 2. Значения заголовка X-ClientCanHandle**</span><span class="sxs-lookup"><span data-stu-id="1c258-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="1c258-121">**Значение X-ClientCanHandle (без учета регистра)**</span><span class="sxs-lookup"><span data-stu-id="1c258-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="1c258-122">**Минимальная версия**</span><span class="sxs-lookup"><span data-stu-id="1c258-122">**Minimum server version**</span></span>|<span data-ttu-id="1c258-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1c258-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1c258-124">Согласование</span><span class="sxs-lookup"><span data-stu-id="1c258-124">Negotiate</span></span>  <br/> |<span data-ttu-id="1c258-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="1c258-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="1c258-126">Если это значение — этот параметр указан, сервер в элементе [AuthPackage (POX)](authpackage-pox.md) вернет значение «Согласование», если сервер настроен на прием проверки подлинности согласование.</span><span class="sxs-lookup"><span data-stu-id="1c258-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="1c258-127">Если это значение не указан, сервер не будет возвращать значение «Согласование» в элементе **AuthPackage** .</span><span class="sxs-lookup"><span data-stu-id="1c258-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="1c258-128">ExHttpInfo</span><span class="sxs-lookup"><span data-stu-id="1c258-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="1c258-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="1c258-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="1c258-130">Если это значение — этот параметр указан, сервер возвращает элемент [Протокола (POX)](protocol-pox.md) с помощью элемента [Типа (POX)](type-pox.md) значение «EXHTTP», если сервер настроен на прием подключений RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1c258-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="1c258-131">Если это значение не указан, сервер не будет возвращать элемент **протокола** с **типом** элемента, задайте значение «EXHTTP».</span><span class="sxs-lookup"><span data-stu-id="1c258-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="1c258-132">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="1c258-132">Request elements</span></span>

<span data-ttu-id="1c258-133">В тексте запроса используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="1c258-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="1c258-134">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="1c258-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="1c258-135">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="1c258-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="1c258-136">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="1c258-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="1c258-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="1c258-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="1c258-138">Элемент [LegacyDN (POX)](legacydn-pox.md) можно использовать вместо элемента [EMailAddress (POX)](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="1c258-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="1c258-139">Различия версий</span><span class="sxs-lookup"><span data-stu-id="1c258-139">Version differences</span></span>

<span data-ttu-id="1c258-140">Заголовок X-MapiHttpCapability доступна в Office 365 и Exchange Online и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1).</span><span class="sxs-lookup"><span data-stu-id="1c258-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="1c258-141">Заголовок X-ClientCanHandle доступна в Office 365 и Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014.</span><span class="sxs-lookup"><span data-stu-id="1c258-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="1c258-142">См. также</span><span class="sxs-lookup"><span data-stu-id="1c258-142">See also</span></span>



[<span data-ttu-id="1c258-143">POX ответа службы автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="1c258-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="1c258-144">Служба POX автоматического обнаружения веб-ссылки для Exchange</span><span class="sxs-lookup"><span data-stu-id="1c258-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="1c258-145">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="1c258-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

