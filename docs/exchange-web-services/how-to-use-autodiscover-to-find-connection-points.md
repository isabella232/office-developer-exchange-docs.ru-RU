---
title: Использование службы автообнаружения для поиска точек подключения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Узнайте, как использовать службу автообнаружения для направления клиентского приложения к правильному серверу Exchange.
ms.openlocfilehash: 653fcd1c094c23c3e89e903b7194b96720802b51
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761127"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="cb42b-103">Использование службы автообнаружения для поиска точек подключения</span><span class="sxs-lookup"><span data-stu-id="cb42b-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="cb42b-104">Узнайте, как использовать службу автообнаружения для направления клиентского приложения к правильному серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="cb42b-105">Служба автообнаружения Exchange предоставляет клиентского приложения с помощью параметров конфигурации для учетных записей электронной почты, размещенных на Exchange Online, Exchange Online в составе Office 365 или Exchange server, версия Exchange начиная с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="cb42b-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="cb42b-106">Служба автообнаружения — веб-службы, который предоставляет параметры конфигурации.</span><span class="sxs-lookup"><span data-stu-id="cb42b-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="cb42b-107">Служба автообнаружения — веб-службы, который предоставляет сведения о конфигурации сервера Exchange для клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="cb42b-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="cb42b-108">Клиентские приложения используйте службы автообнаружения для определения конечной точки службы автообнаружения для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="cb42b-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="cb42b-109">В этой статье объясняется, как выполнять ответов с сервера Exchange, чтобы найти правильный конечной точки.</span><span class="sxs-lookup"><span data-stu-id="cb42b-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="cb42b-110">Сведения о том, как получить параметры конфигурации адрес электронной почты можно [получить параметры пользователя из Exchange с помощью службы автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и [получить параметры домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="cb42b-111">Процесс поиска правильный конечная точка является частью запроса для пользователя или параметры домена.</span><span class="sxs-lookup"><span data-stu-id="cb42b-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="cb42b-112">Служба автообнаружения использует ряд ответы перенаправления для отправки клиентского приложения к конечной точке правильные адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="cb42b-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="cb42b-113">Можно использовать один из следующих технологиях разработки Exchange для доступа к службе автообнаружения:</span><span class="sxs-lookup"><span data-stu-id="cb42b-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>
  
> [!NOTE]
> <span data-ttu-id="cb42b-114">Дополнительные сведения об этих технологиях разработки Exchange можно [Проводник управляемый API веб-служб Exchange, веб-служб Exchange и веб-служб Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-114">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 
  
- <span data-ttu-id="cb42b-115">Веб-служб Exchange (EWS) управляемого интерфейса API</span><span class="sxs-lookup"><span data-stu-id="cb42b-115">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="cb42b-116">EWS</span><span class="sxs-lookup"><span data-stu-id="cb42b-116">EWS</span></span>
    
    <span data-ttu-id="cb42b-117">При использовании веб-служб Exchange, можно использовать следующие методы для получения параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="cb42b-117">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
  - <span data-ttu-id="cb42b-118">Служба автообнаружения на основе SOAP</span><span class="sxs-lookup"><span data-stu-id="cb42b-118">The SOAP-based Autodiscover service</span></span>
    
  - <span data-ttu-id="cb42b-119">Служба автообнаружения XML (POX)</span><span class="sxs-lookup"><span data-stu-id="cb42b-119">The XML (POX) Autodiscover service</span></span>
    
  - <span data-ttu-id="cb42b-120">Прокси-сервер автоматически созданный, созданный из службы SOAP или автоматического обнаружения XML</span><span class="sxs-lookup"><span data-stu-id="cb42b-120">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
    <span data-ttu-id="cb42b-121">Дополнительные сведения об этих методов можно [автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-121">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>
    
<span data-ttu-id="cb42b-122">Управляемый API веб-служб Exchange предоставляет объектно ориентированный интерфейс для извлечения параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb42b-122">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="cb42b-123">Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-123">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="cb42b-124">Чем обычно автоматически созданный прокси веб-службы для простой объектной модели лучше оптимизированный интерфейс управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-124">The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="cb42b-125">При использовании веб-служб Exchange, рекомендуется использовать службы автообнаружения SOAP, поскольку она поддерживает расширенный набор функциональных возможностей, чем службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="cb42b-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="cb42b-126">Необходимые условия для поиска конечную точку</span><span class="sxs-lookup"><span data-stu-id="cb42b-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="cb42b-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="cb42b-127"></span></span>

<span data-ttu-id="cb42b-128">Перед созданием клиентское приложение, которое использует службу автообнаружения, необходимо иметь доступ к таким компонентам:</span><span class="sxs-lookup"><span data-stu-id="cb42b-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="cb42b-129">Exchange Online или сервера, на котором выполняется версия Exchange о том, начиная с Exchange 2007 с пакетом обновления 1.</span><span class="sxs-lookup"><span data-stu-id="cb42b-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="cb42b-130">При использовании службы автообнаружения на основе SOAP, Exchange Online или версии Exchange, начиная с Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="cb42b-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="cb42b-131">Exchange server, который настроен на прием подключений от клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="cb42b-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="cb42b-132">Сведения о настройке Exchange server в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="cb42b-133">Учетная запись, разрешенных для использования веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="cb42b-134">Сведения о настройке учетной записи в разделе [Управление доступом к клиентского приложения для веб-служб Exchange в Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="cb42b-135">Если используется управляемый API веб-служб Exchange, необходимо предоставить обратного вызова проверки сертификата при определенных обстоятельствах.</span><span class="sxs-lookup"><span data-stu-id="cb42b-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="cb42b-136">Может также потребоваться обратного вызова проверки сертификата с библиотеками некоторые созданного прокси-сервера, например, которые были созданы с помощью Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="cb42b-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="cb42b-137">Дополнительные сведения можно [Проверить сертификат сервера для управляемого интерфейса API веб-служб Exchange](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="cb42b-138">Основные понятия, которые поиска конечную точку</span><span class="sxs-lookup"><span data-stu-id="cb42b-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="cb42b-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="cb42b-139"></span></span>

<span data-ttu-id="cb42b-140">Прежде чем использовать службы автообнаружения для поиска конечную точку, необходимо ознакомиться с понятиями, приведенными в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="cb42b-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="cb42b-141">**Концепция**</span><span class="sxs-lookup"><span data-stu-id="cb42b-141">**Concept**</span></span>|<span data-ttu-id="cb42b-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cb42b-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb42b-143">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="cb42b-144">Обзор работы службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="cb42b-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="cb42b-145">При использовании управляемого интерфейса API веб-служб Exchange, используйте класс [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в пространстве имен [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) для управления подключением к веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="cb42b-146">Чтобы использовать управляемый API EWS примеры кода в этой статье, необходимо ссылаться на следующие пространства имен в коде:</span><span class="sxs-lookup"><span data-stu-id="cb42b-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="cb42b-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="cb42b-147">**System.Net**</span></span>
    
- <span data-ttu-id="cb42b-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="cb42b-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="cb42b-149">Найти правильный конечных точек с помощью управляемого интерфейса API веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="cb42b-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="cb42b-150"></span></span>

<span data-ttu-id="cb42b-151">При использовании управляемого интерфейса API веб-служб Exchange для службы автообнаружения вызовами классом **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="cb42b-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="cb42b-152">Чтобы определить правильное конечной точки для учетной записи электронной почты, вызовите метод **AutodiscoverUrl** объекта **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="cb42b-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="cb42b-153">В следующем примере кода показано, как задать конечную веб-службы веб-служб Exchange для адреса электронной почты Exchange.asmx файла на правильный сервер клиентского доступа с помощью управляемого интерфейса API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="cb42b-154">Найти правильный конечных точек с помощью веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="cb42b-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="cb42b-155"></span></span>

<span data-ttu-id="cb42b-156">Служба автообнаружения SOAP может использовать ряд запросы и ответы для направления приложения правильные конечную точку для веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="cb42b-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="cb42b-157">Сведения о процессе по определению правильный конечных точек для учетной записи электронной почты содержатся в разделе [службы автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="cb42b-158">В следующих примерах XML серии запросов и ответов, которые можно ожидать при выполнении запроса SOAP автообнаружения найти правильный конечную точку.</span><span class="sxs-lookup"><span data-stu-id="cb42b-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="cb42b-159">Запрос конечной точки службы автообнаружения SOAP</span><span class="sxs-lookup"><span data-stu-id="cb42b-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="cb42b-160">В следующем примере показано запрос XML, который отправляется найти правильный конечной точки для службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="cb42b-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://mail.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="cb42b-161">Ответ SOAP автообнаружения в режиме одобрения администратором</span><span class="sxs-lookup"><span data-stu-id="cb42b-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="cb42b-162">Служба автообнаружения может отвечать на запросы с одним из двух ответы перенаправления: на перенаправление HTTP 302 или в режиме одобрения администратором ответа SOAP.</span><span class="sxs-lookup"><span data-stu-id="cb42b-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="cb42b-163">Если ответ от сервера Exchange на перенаправление HTTP 302, клиентское приложение следует проверить, что адрес перенаправления является приемлемым и следуйте ответа в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="cb42b-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [! Примечание по безопасности]<span data-ttu-id="cb42b-164"> критериев для проверки правильности ответа в режиме одобрения администратором, посвященной [автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="cb42b-164"> For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="cb42b-165">Если служба автообнаружения возвращать ответа в режиме одобрения администратором, указанный в параметре элемент [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **ответ пользователя** , клиентское приложение следует использовать элемент **RedirectTarget** для создания нового запроса параметров, то есть Отправить на сервер, указанный в ответ в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="cb42b-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="cb42b-166">В следующем примере показано ответа в режиме одобрения администратором на сервере.</span><span class="sxs-lookup"><span data-stu-id="cb42b-166">The following example shows a redirection response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>682</h:MajorBuildNumber>
      <h:MinorBuildNumber>1</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>RedirectAddress</ErrorCode>
            <ErrorMessage>Redirection address.</ErrorMessage>
            <RedirectTarget>User1@mail.Contoso.com</RedirectTarget>
            <UserSettingErrors />
            <UserSettings />
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="cb42b-167">После перенаправления клиент использует URL-адрес перенаправления для подготовки другой запрос.</span><span class="sxs-lookup"><span data-stu-id="cb42b-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="cb42b-168">Следующий код является примером запроса, создаваемого из ответа в режиме одобрения администратором.</span><span class="sxs-lookup"><span data-stu-id="cb42b-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:wsa="http://www.w3.org/2005/08/addressing" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
        xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2013</a:RequestedServerVersion>
    <wsa:Action>http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://autodiscover.exchange.microsoft.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>User1@mail.Contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>InternalEwsUrl</a:Setting>
          <a:Setting>ExternalEwsUrl</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="cb42b-169">Если клиентское приложение были перенаправлены на правильные конечной точки для службы автообнаружения, сервер отправляет ответ, содержащий элемент [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **ответ пользователя** значение **NoError** и содержащий запрашиваемый параметры пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb42b-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="cb42b-170">Возвращаются только запрошенный параметры пользователя, **InternalEwsUrl** и **ExternalEwsUrl**.</span><span class="sxs-lookup"><span data-stu-id="cb42b-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="cb42b-171">В следующем примере показано ответ от сервера.</span><span class="sxs-lookup"><span data-stu-id="cb42b-171">The following example shows the response from the server.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/" 
        xmlns:a="http://www.w3.org/2005/08/addressing">
  <s:Header>
    <a:Action s:mustUnderstand="1">http://schemas.microsoft.com/exchange/2010/
        Autodiscover/Autodiscover/GetUserSettingsResponse</a:Action>
    <h:ServerVersionInfo xmlns:h="http://schemas.microsoft.com/exchange/2010/Autodiscover" 
        xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
      <h:MajorVersion>15</h:MajorVersion>
      <h:MinorVersion>0</h:MinorVersion>
      <h:MajorBuildNumber>160</h:MajorBuildNumber>
      <h:MinorBuildNumber>4</h:MinorBuildNumber>
      <h:Version>Exchange2013</h:Version>
    </h:ServerVersionInfo>
  </s:Header>
  <s:Body>
    <GetUserSettingsResponseMessage xmlns="http://schemas.microsoft.com/exchange/2010/Autodiscover">
      <Response xmlns:i="http://www.w3.org/2001/XMLSchema-instance">
        <ErrorCode>NoError</ErrorCode>
        <ErrorMessage />
        <UserResponses>
          <UserResponse>
            <ErrorCode>NoError</ErrorCode>
            <ErrorMessage>No error.</ErrorMessage>
            <RedirectTarget i:nil="true" />
            <UserSettingErrors />
            <UserSettings>
              <UserSetting i:type="StringSetting">
                <Name>InternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
              <UserSetting i:type="StringSetting">
                <Name>ExternalEwsUrl</Name>
                <Value>https://server.Contoso.com/ews/exchange.asmx</Value>
              </UserSetting>
            </UserSettings>
          </UserResponse>
        </UserResponses>
      </Response>
    </GetUserSettingsResponseMessage>
  </s:Body>
</s:Envelope>
```

## <a name="next-steps"></a><span data-ttu-id="cb42b-172">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="cb42b-172">Next steps</span></span>
<span data-ttu-id="cb42b-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="cb42b-173"></span></span>

<span data-ttu-id="cb42b-174">Поиск в конечную точку, выполнив процесса автообнаружения возвращает запрошенного домена или параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="cb42b-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="cb42b-175">Сведения о выполнении запроса для определенных параметров см в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="cb42b-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="cb42b-176">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)
    
- [<span data-ttu-id="cb42b-177">Получить параметры пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="cb42b-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="cb42b-178">См. также</span><span class="sxs-lookup"><span data-stu-id="cb42b-178">See also</span></span>


- [<span data-ttu-id="cb42b-179">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)
    
- [<span data-ttu-id="cb42b-180">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)
    
- [<span data-ttu-id="cb42b-181">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)
    
- [<span data-ttu-id="cb42b-182">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="cb42b-182">EWS reference for Exchange</span></span>](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

