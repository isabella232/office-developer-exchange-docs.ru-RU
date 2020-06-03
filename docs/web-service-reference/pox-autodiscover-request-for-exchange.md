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
description: Запрос автообнаружения содержит запрос для конфигурации клиентского доступа пользователя.
ms.openlocfilehash: b2138f9813c7b75aef9afb90089b9b874aac7532
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461669"
---
# <a name="pox-autodiscover-request-for-exchange"></a><span data-ttu-id="ccb1c-103">Запрос автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ccb1c-103">POX Autodiscover request for Exchange</span></span>

<span data-ttu-id="ccb1c-104">Запрос автообнаружения содержит запрос для конфигурации клиентского доступа пользователя.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-104">The Autodiscover request contains a query for a user's client access configuration.</span></span>
  
## <a name="autodiscover-request-example"></a><span data-ttu-id="ccb1c-105">Пример запроса автообнаружения</span><span class="sxs-lookup"><span data-stu-id="ccb1c-105">Autodiscover request example</span></span>

### <a name="description"></a><span data-ttu-id="ccb1c-106">Description</span><span class="sxs-lookup"><span data-stu-id="ccb1c-106">Description</span></span>

<span data-ttu-id="ccb1c-107">В приведенном ниже примере XML-кода показан текст запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-107">The following XML example shows an Autodiscover request body.</span></span>
  
### <a name="code"></a><span data-ttu-id="ccb1c-108">Код</span><span class="sxs-lookup"><span data-stu-id="ccb1c-108">Code</span></span>

```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
   <Request>
     <EMailAddress>user@contoso.com</EMailAddress>
     <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
   </Request>
 </Autodiscover>
```

### <a name="request-headers"></a><span data-ttu-id="ccb1c-109">Заголовки запросов</span><span class="sxs-lookup"><span data-stu-id="ccb1c-109">Request Headers</span></span>

<span data-ttu-id="ccb1c-110">Следующие заголовки HTTP необязательны при отправке запросов автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-110">The following HTTP headers are optional when sending Autodiscover requests.</span></span>
  
<span data-ttu-id="ccb1c-111">**Таблица 1. Заголовки HTTP-запросов**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-111">**Table 1. HTTP request headers**</span></span>

|<span data-ttu-id="ccb1c-112">**Header**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-112">**Header**</span></span>|<span data-ttu-id="ccb1c-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ccb1c-114">X — Мапихттпкапабилити</span><span class="sxs-lookup"><span data-stu-id="ccb1c-114">X-MapiHttpCapability</span></span>  <br/> |<span data-ttu-id="ccb1c-115">Если указано значение "1", клиент запрашивает сведения, которые можно использовать для подключения к серверу с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-115">If present and set to "1", indicates that the client is requesting information that can be used to connect to the server by using the MAPI/HTTP protocol.</span></span> <span data-ttu-id="ccb1c-116">Этот заголовок применяется для клиентов, которые реализуют протокол MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-116">This header is applicable to clients that implement the MAPI/HTTP protocol.</span></span>  <br/> |
|<span data-ttu-id="ccb1c-117">X — Клиентканхандле</span><span class="sxs-lookup"><span data-stu-id="ccb1c-117">X-ClientCanHandle</span></span>  <br/> |<span data-ttu-id="ccb1c-118">Этот заголовок содержит разделенный запятыми список возможностей, поддерживаемых клиентом.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-118">This header contains a comma-delimited list of capabilities that the client supports.</span></span> <span data-ttu-id="ccb1c-119">Возможные значения указаны в таблице 2.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-119">The possible values are specified in Table 2.</span></span>  <br/> |
   
<span data-ttu-id="ccb1c-120">**Таблица 2. Значения заголовков X – Клиентканхандле**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-120">**Table 2. X-ClientCanHandle header values**</span></span>

|<span data-ttu-id="ccb1c-121">**Значение X-Клиентканхандле (без учета регистра)**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-121">**X-ClientCanHandle value (case-insensitive)**</span></span>|<span data-ttu-id="ccb1c-122">**Минимальная версия сервера**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-122">**Minimum server version**</span></span>|<span data-ttu-id="ccb1c-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ccb1c-123">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="ccb1c-124">Подключение</span><span class="sxs-lookup"><span data-stu-id="ccb1c-124">Negotiate</span></span>  <br/> |<span data-ttu-id="ccb1c-125">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="ccb1c-125">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="ccb1c-126">Если задано это значение, сервер возвратит значение "Negotiate" в элементе [ауспаккаже (POX)](authpackage-pox.md) , если сервер настроен для приема проверки подлинности согласования.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-126">If this value is present, the server will return a value of "Negotiate" in the [AuthPackage (POX)](authpackage-pox.md) element if the server is configured to accept Negotiate authentication.</span></span> <span data-ttu-id="ccb1c-127">Если это значение отсутствует, сервер не возвратит значение "Negotiate" в элементе **ауспаккаже** .</span><span class="sxs-lookup"><span data-stu-id="ccb1c-127">If this value is not present, the server will not return a value of "Negotiate" in the **AuthPackage** element.</span></span>  <br/> |
|<span data-ttu-id="ccb1c-128">ексхттпинфо</span><span class="sxs-lookup"><span data-stu-id="ccb1c-128">ExHttpInfo</span></span>  <br/> |<span data-ttu-id="ccb1c-129">15.00.0995.014</span><span class="sxs-lookup"><span data-stu-id="ccb1c-129">15.00.0995.014</span></span>  <br/> |<span data-ttu-id="ccb1c-130">Если это значение задано, сервер возвратит элемент [протокола (POX)](protocol-pox.md) с элементом [Type (POX)](type-pox.md) со значением "ексхттп", если сервер НАСТРОЕН для приема подключений RPC/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-130">If this value is present, the server will return a [Protocol (POX)](protocol-pox.md) element with a [Type (POX)](type-pox.md) element set to "EXHTTP" if the server is configured to accept RPC/HTTP connections.</span></span> <span data-ttu-id="ccb1c-131">Если это значение отсутствует, сервер не возвращает элемент **Protocol** , у которого для элемента **Type** задано значение "ексхттп".</span><span class="sxs-lookup"><span data-stu-id="ccb1c-131">If this value is not present, the server will not return a **Protocol** element with a **Type** element set to "EXHTTP".</span></span>  <br/> |
   
### <a name="request-elements"></a><span data-ttu-id="ccb1c-132">Элементы Request</span><span class="sxs-lookup"><span data-stu-id="ccb1c-132">Request elements</span></span>

<span data-ttu-id="ccb1c-133">В тексте запроса используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="ccb1c-133">The following elements are used in the request body:</span></span>
  
- [<span data-ttu-id="ccb1c-134">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="ccb1c-134">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
    
- [<span data-ttu-id="ccb1c-135">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="ccb1c-135">Request (POX)</span></span>](request-pox.md)
    
- [<span data-ttu-id="ccb1c-136">Акцептаблереспонсесчема (POX)</span><span class="sxs-lookup"><span data-stu-id="ccb1c-136">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md)
    
- [<span data-ttu-id="ccb1c-137">EMailAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="ccb1c-137">EMailAddress (POX)</span></span>](emailaddress-pox.md)
    
> [!NOTE]
> <span data-ttu-id="ccb1c-138">Элемент [LegacyDN (POX)](legacydn-pox.md) можно использовать вместо элемента [EMailAddress (POX)](emailaddress-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="ccb1c-138">The [LegacyDN (POX)](legacydn-pox.md) element can be used in place of the [EMailAddress (POX)](emailaddress-pox.md) element.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="ccb1c-139">Различия версий</span><span class="sxs-lookup"><span data-stu-id="ccb1c-139">Version differences</span></span>

<span data-ttu-id="ccb1c-140">Заголовок X-Мапихттпкапабилити доступен в Office 365, Exchange Online и локальных версиях Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1 (SP1)).</span><span class="sxs-lookup"><span data-stu-id="ccb1c-140">The X-MapiHttpCapability header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span>
  
<span data-ttu-id="ccb1c-141">Заголовок X-Клиентканхандле доступен в Office 365, Exchange Online и локальных версиях Exchange, начиная с сборки 15.00.0995.014.</span><span class="sxs-lookup"><span data-stu-id="ccb1c-141">The X-ClientCanHandle header is available in Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="ccb1c-142">См. также</span><span class="sxs-lookup"><span data-stu-id="ccb1c-142">See also</span></span>



[<span data-ttu-id="ccb1c-143">Отклик автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ccb1c-143">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)


[<span data-ttu-id="ccb1c-144">Справочник по веб-службе автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ccb1c-144">POX Autodiscover web service reference for Exchange</span></span>](pox-autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="ccb1c-145">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ccb1c-145">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

