---
title: Поиск точек соединения с помощью службы автообнаружения
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 03896542-549b-4c45-973c-98f9025ea26c
description: Узнайте, как использовать службу автообнаружения для направления клиентского приложения на соответствующий сервер Exchange.
ms.openlocfilehash: eb3fb3664e5789638c097a43cf48f757bb0713ae
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353982"
---
# <a name="use-autodiscover-to-find-connection-points"></a><span data-ttu-id="a16b6-103">Поиск точек соединения с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a16b6-103">Use Autodiscover to find connection points</span></span>

<span data-ttu-id="a16b6-104">Узнайте, как использовать службу автообнаружения для направления клиентского приложения на соответствующий сервер Exchange.</span><span class="sxs-lookup"><span data-stu-id="a16b6-104">Find out how to use the Autodiscover service to direct your client application to the correct Exchange server.</span></span>
  
<span data-ttu-id="a16b6-105">Служба автообнаружения Exchange предоставляет клиентским приложениям параметры конфигурации для учетных записей электронной почты, размещенных в Exchange Online, Exchange Online в составе Office 365, или на сервере Exchange Server с Exchange 2013.</span><span class="sxs-lookup"><span data-stu-id="a16b6-105">The Exchange Autodiscover service provides your client application with configuration settings for email accounts that are hosted on Exchange Online, Exchange Online as part of Office 365, or an Exchange server running a version of Exchange starting with Exchange 2013.</span></span> <span data-ttu-id="a16b6-106">Служба автообнаружения — это веб-служба, предоставляющая параметры конфигурации.</span><span class="sxs-lookup"><span data-stu-id="a16b6-106">The Autodiscover service is a web service that provides configuration settings.</span></span> <span data-ttu-id="a16b6-107">Служба автообнаружения — это веб-служба, которая предоставляет клиентским приложениям сведения о конфигурации Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="a16b6-107">The Autodiscover service is a web service that provides Exchange server configuration information to your client application.</span></span> <span data-ttu-id="a16b6-108">Клиентские приложения используют службу автообнаружения для определения конечной точки службы автообнаружения для определенного почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a16b6-108">Client applications use Autodiscover to determine the endpoint of the Autodiscover service for a specific mailbox.</span></span> <span data-ttu-id="a16b6-109">В этой статье объясняется, как выполнять ответы от сервера Exchange Server, чтобы найти правильную конечную точку.</span><span class="sxs-lookup"><span data-stu-id="a16b6-109">This article explains how to follow the responses from an Exchange server to find the correct endpoint.</span></span> 
  
<span data-ttu-id="a16b6-110">Сведения о получении параметров конфигурации адресов электронной почты приведены в статье [Получение параметров пользователя из Exchange с помощью автообнаружения](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) и [Получение параметров домена с сервера Exchange](how-to-get-domain-settings-from-an-exchange-server.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-110">For information about how to get email address configuration settings, see [Get user settings from Exchange by using Autodiscover](how-to-get-user-settings-from-exchange-by-using-autodiscover.md) and [Get domain settings from an Exchange server](how-to-get-domain-settings-from-an-exchange-server.md).</span></span>
  
> [!NOTE]
> <span data-ttu-id="a16b6-111">Процесс поиска правильной конечной точки является частью запроса параметров пользователя или домена.</span><span class="sxs-lookup"><span data-stu-id="a16b6-111">The process for finding the correct endpoint is part of the request for user or domain settings.</span></span> <span data-ttu-id="a16b6-112">Служба автообнаружения использует серию ответов перенаправления для отправки клиентского приложения в правильную конечную точку для адреса электронной почты.</span><span class="sxs-lookup"><span data-stu-id="a16b6-112">The Autodiscover service uses a series of redirect responses to send the client application to the correct endpoint for an email address.</span></span> 
  
<span data-ttu-id="a16b6-113">Для доступа к службе автообнаружения можно использовать одну из следующих технологий разработки Exchange:</span><span class="sxs-lookup"><span data-stu-id="a16b6-113">You can use one of the following Exchange development technologies to access the Autodiscover service:</span></span>

- <span data-ttu-id="a16b6-114">Управляемый API веб-служб Exchange (EWS)</span><span class="sxs-lookup"><span data-stu-id="a16b6-114">The Exchange Web Services (EWS) Managed API</span></span>
    
- <span data-ttu-id="a16b6-115">EWS</span><span class="sxs-lookup"><span data-stu-id="a16b6-115">EWS</span></span>
    
<span data-ttu-id="a16b6-116">Если вы используете EWS, вы можете использовать следующие методы для получения параметров пользователя:</span><span class="sxs-lookup"><span data-stu-id="a16b6-116">If you are using EWS, you can use the following methods to retrieve user settings:</span></span>
    
- <span data-ttu-id="a16b6-117">Служба автообнаружения на основе SOAP</span><span class="sxs-lookup"><span data-stu-id="a16b6-117">The SOAP-based Autodiscover service</span></span>
    
- <span data-ttu-id="a16b6-118">Служба автообнаружения XML (POX)</span><span class="sxs-lookup"><span data-stu-id="a16b6-118">The XML (POX) Autodiscover service</span></span>
    
- <span data-ttu-id="a16b6-119">Автоматически созданный прокси-сервер, созданный службой автообнаружения SOAP или XML</span><span class="sxs-lookup"><span data-stu-id="a16b6-119">An autogenerated proxy generated from the SOAP or XML Autodiscover service</span></span>
    
<span data-ttu-id="a16b6-120">Дополнительные сведения об этих методах см. в разделе [автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-120">For more information about these methods, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span>

<span data-ttu-id="a16b6-121">Дополнительные сведения об этих технологиях разработки Exchange можно найти [в статье Обзор управляемого API EWS, EWS и веб-служб в Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-121">For more information about these Exchange development technologies, see [Explore the EWS Managed API, EWS, and web services in Exchange](explore-the-ews-managed-api-ews-and-web-services-in-exchange.md).</span></span> 

<span data-ttu-id="a16b6-122">Управляемый API EWS предоставляет интерфейс на основе объектов для получения параметров пользователя.</span><span class="sxs-lookup"><span data-stu-id="a16b6-122">The EWS Managed API provides an object-based interface for retrieving user settings.</span></span> <span data-ttu-id="a16b6-123">Если клиентское приложение использует управляемый код, мы рекомендуем использовать управляемый API EWS.</span><span class="sxs-lookup"><span data-stu-id="a16b6-123">If your client application uses managed code, we recommend that you use the EWS Managed API.</span></span> <span data-ttu-id="a16b6-124">Интерфейс управляемого API EWS лучше оптимизирован для простой объектной модели по сравнению с обычным автоматически созданным прокси-сервером веб-службы.</span><span class="sxs-lookup"><span data-stu-id="a16b6-124">The EWS Managed API interface is better optimized for a simple object model than the typical autogenerated web service proxy.</span></span> 
  
<span data-ttu-id="a16b6-125">Если вы используете EWS, мы рекомендуем использовать службу автообнаружения SOAP, так как она поддерживает более широкий набор функций, чем служба автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="a16b6-125">If you are using EWS, we suggest that you use the SOAP Autodiscover service, because it supports a richer set of features than the POX Autodiscover service.</span></span>
  
## <a name="prerequisites-for-finding-an-endpoint"></a><span data-ttu-id="a16b6-126">Необходимые условия для поиска конечной точки</span><span class="sxs-lookup"><span data-stu-id="a16b6-126">Prerequisites for finding an endpoint</span></span>
<span data-ttu-id="a16b6-127"><a name="bk_Prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="a16b6-127"><a name="bk_Prereq"> </a></span></span>

<span data-ttu-id="a16b6-128">Прежде чем можно будет создать клиентское приложение, использующее службу автообнаружения, необходимо иметь доступ к следующим параметрам:</span><span class="sxs-lookup"><span data-stu-id="a16b6-128">Before you can create a client application that uses the Autodiscover service, you need to have access to the following:</span></span>
  
- <span data-ttu-id="a16b6-129">Exchange Online или сервер, на котором работает версия Exchange начиная с Exchange 2007 с пакетом обновления 1 (SP1).</span><span class="sxs-lookup"><span data-stu-id="a16b6-129">Exchange Online or a server that is running a version of Exchange starting with Exchange 2007 SP1.</span></span> <span data-ttu-id="a16b6-130">Если вы используете службу автообнаружения на основе SOAP, Exchange Online или версию Exchange, начиная с Exchange 2010.</span><span class="sxs-lookup"><span data-stu-id="a16b6-130">If you are using the SOAP-based Autodiscover service, Exchange Online or a version of Exchange starting with Exchange 2010.</span></span>
    
- <span data-ttu-id="a16b6-131">Сервер Exchange, настроенный для приема подключений из клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="a16b6-131">An Exchange server that is configured to accept connections from your client application.</span></span> <span data-ttu-id="a16b6-132">Сведения о настройке сервера Exchange Server можно найти [в статье Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-132">For information about how to configure your Exchange server, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
- <span data-ttu-id="a16b6-133">Учетная запись, которая авторизована для использования EWS.</span><span class="sxs-lookup"><span data-stu-id="a16b6-133">An account that is authorized to use EWS.</span></span> <span data-ttu-id="a16b6-134">Сведения о настройке учетной записи см [в разделе Управление доступом клиентского приложения к EWS в Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-134">For information about how to configure an account, see [Controlling client application access to EWS in Exchange](controlling-client-application-access-to-ews-in-exchange.md).</span></span>
    
> [!NOTE]
> <span data-ttu-id="a16b6-135">Если вы используете управляемый API EWS, в некоторых обстоятельствах необходимо предоставить обратный вызов проверки сертификата.</span><span class="sxs-lookup"><span data-stu-id="a16b6-135">If you are using the EWS Managed API, you must provide a certificate validation callback in some circumstances.</span></span> <span data-ttu-id="a16b6-136">Кроме того, вам может потребоваться обратный вызов проверки сертификата со всеми созданными библиотеками прокси, например, созданными Visual Studio.</span><span class="sxs-lookup"><span data-stu-id="a16b6-136">You may also need a certificate validation callback with some generated proxy libraries, such as those created by Visual Studio.</span></span> <span data-ttu-id="a16b6-137">Дополнительные сведения см. [в статье Проверка сертификата сервера для управляемого API EWS](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-137">For more information, see [Validate a server certificate for the EWS Managed API](how-to-validate-a-server-certificate-for-the-ews-managed-api.md).</span></span> 
  
### <a name="core-concepts-for-finding-an-endpoint"></a><span data-ttu-id="a16b6-138">Основные понятия, связанные с поиском конечной точки</span><span class="sxs-lookup"><span data-stu-id="a16b6-138">Core concepts for finding an endpoint</span></span>
<span data-ttu-id="a16b6-139"><a name="bk_Core"> </a></span><span class="sxs-lookup"><span data-stu-id="a16b6-139"><a name="bk_Core"> </a></span></span>

<span data-ttu-id="a16b6-140">Прежде чем использовать службу автообнаружения для поиска конечной точки, необходимо ознакомиться с концепциями, приведенными в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="a16b6-140">Before you use Autodiscover to find an endpoint, you should be familiar with the concepts listed in the following table.</span></span>
  
|<span data-ttu-id="a16b6-141">**Концепция**</span><span class="sxs-lookup"><span data-stu-id="a16b6-141">**Concept**</span></span>|<span data-ttu-id="a16b6-142">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a16b6-142">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a16b6-143">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-143">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md) <br/> |<span data-ttu-id="a16b6-144">Предоставляет общие сведения о работе службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="a16b6-144">Provides an overview of how the Autodiscover service works.</span></span>  <br/> |
   
<span data-ttu-id="a16b6-145">Если вы используете управляемый API EWS, вы используете класс [Microsoft. Exchange. WebServices. Data. ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) в пространстве имен [Microsoft. Exchange. WebServices. Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) для управления подключением к EWS.</span><span class="sxs-lookup"><span data-stu-id="a16b6-145">If you are using the EWS Managed API, you use the [Microsoft.Exchange.WebServices.Data.ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) class in the [Microsoft.Exchange.WebServices.Data](http://msdn.microsoft.com/en-us/library/dd633907%28v=exchg.80%29.aspx) namespace to manage your connection to EWS.</span></span> <span data-ttu-id="a16b6-146">Чтобы использовать примеры кода управляемого API EWS, приведенные в этой статье, необходимо сослаться на следующие пространства имен в коде:</span><span class="sxs-lookup"><span data-stu-id="a16b6-146">To use the EWS Managed API code samples in this article, you need to reference the following namespaces in your code:</span></span> 
  
- <span data-ttu-id="a16b6-147">**System.Net**</span><span class="sxs-lookup"><span data-stu-id="a16b6-147">**System.Net**</span></span>
    
- <span data-ttu-id="a16b6-148">**Microsoft. Exchange. WebServices. Data. ExchangeService**</span><span class="sxs-lookup"><span data-stu-id="a16b6-148">**Microsoft.Exchange.WebServices.Data.ExchangeService**</span></span>
    
## <a name="find-the-correct-endpoint-by-using-the-ews-managed-api"></a><span data-ttu-id="a16b6-149">Поиск правильной конечной точки с помощью управляемого API EWS</span><span class="sxs-lookup"><span data-stu-id="a16b6-149">Find the correct endpoint by using the EWS Managed API</span></span>
<span data-ttu-id="a16b6-150"><a name="bk_Managed"> </a></span><span class="sxs-lookup"><span data-stu-id="a16b6-150"><a name="bk_Managed"> </a></span></span>

<span data-ttu-id="a16b6-151">Если вы используете управляемый API EWS, вызовы службы автообнаружения обрабатываются классом **ExchangeService** .</span><span class="sxs-lookup"><span data-stu-id="a16b6-151">If you are using the EWS Managed API, calls to the Autodiscover service are handled by the **ExchangeService** class.</span></span> <span data-ttu-id="a16b6-152">Чтобы определить правильную конечную точку для учетной записи электронной почты, необходимо вызвать метод **AutodiscoverUrl** для объекта **[ExchangeService]** .</span><span class="sxs-lookup"><span data-stu-id="a16b6-152">To determine the correct endpoint for an email account, you call the **AutodiscoverUrl** method on an **[ExchangeService]** object.</span></span> <span data-ttu-id="a16b6-153">В следующем примере кода показано, как установить конечную точку веб-службы EWS для адреса электронной почты в файл Exchange. asmx на правильном сервере клиентского доступа с помощью управляемого API EWS.</span><span class="sxs-lookup"><span data-stu-id="a16b6-153">The following code example shows how to set the EWS web service endpoint for an email address to the Exchange.asmx file on the correct Client Access server by using the EWS Managed API.</span></span> 
  
```cs
NetworkCredential credentials = new NetworkCredential(securelyStoredEmail, securelyStoredPassword);
ExchangeService service = new ExchangeService(ExchangeVersion.Exchange2013);
service.Credentials = credentials;
service.AutodiscoverUrl("User1@contoso.com");
```

## <a name="find-the-correct-endpoint-by-using-ews"></a><span data-ttu-id="a16b6-154">Поиск правильной конечной точки с помощью EWS</span><span class="sxs-lookup"><span data-stu-id="a16b6-154">Find the correct endpoint by using EWS</span></span>
<span data-ttu-id="a16b6-155"><a name="bk_SOAP"> </a></span><span class="sxs-lookup"><span data-stu-id="a16b6-155"><a name="bk_SOAP"> </a></span></span>

<span data-ttu-id="a16b6-156">Служба автообнаружения SOAP может использовать серию запросов и ответов для направления приложения в правильную конечную точку для EWS.</span><span class="sxs-lookup"><span data-stu-id="a16b6-156">The SOAP Autodiscover service may use a series of requests and responses to direct your application to the correct endpoint for EWS.</span></span> <span data-ttu-id="a16b6-157">Сведения о том, как определить правильную конечную точку для учетной записи электронной почты, можно найти в разделе Служба [автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-157">For information about the process for determining the correct endpoint for an email account, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> <span data-ttu-id="a16b6-158">В следующих примерах XML-кода показан ряд запросов и ответов, которые можно ожидать при выполнении запроса автообнаружения SOAP для поиска нужной конечной точки.</span><span class="sxs-lookup"><span data-stu-id="a16b6-158">The following XML examples show the series of requests and responses that you can expect when making a SOAP Autodiscover request to find the correct endpoint.</span></span>
  
### <a name="soap-autodiscover-endpoint-request"></a><span data-ttu-id="a16b6-159">Запрос конечной точки автообнаружения SOAP</span><span class="sxs-lookup"><span data-stu-id="a16b6-159">SOAP Autodiscover endpoint request</span></span>

<span data-ttu-id="a16b6-160">В следующем примере показан XML-запрос, который отправляется в службу автообнаружения, чтобы найти правильную конечную точку.</span><span class="sxs-lookup"><span data-stu-id="a16b6-160">The following example shows an XML request that is sent to the Autodiscover service to find the correct endpoint.</span></span>
  
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

### <a name="soap-autodiscover-redirection-response"></a><span data-ttu-id="a16b6-161">Ответ на перенаправление автообнаружения SOAP</span><span class="sxs-lookup"><span data-stu-id="a16b6-161">SOAP Autodiscover redirection response</span></span>

<span data-ttu-id="a16b6-162">Служба автообнаружения может отвечать на один из двух ответов перенаправления: HTTP 302 Redirect или ответ на перенаправление SOAP.</span><span class="sxs-lookup"><span data-stu-id="a16b6-162">The Autodiscover service may respond with one of two redirection responses: an HTTP 302 redirect, or a SOAP redirection response.</span></span> <span data-ttu-id="a16b6-163">Если ответ сервера Exchange Server является перенаправлением HTTP 302, клиентское приложение должно проверить, является ли адрес перенаправления допустимым, а затем следовать ответу перенаправления.</span><span class="sxs-lookup"><span data-stu-id="a16b6-163">If the response from the Exchange server is an HTTP 302 redirect, the client application should validate that the redirection address is acceptable and then follow the redirection response.</span></span>
  
> [!IMPORTANT]
> <span data-ttu-id="a16b6-164">Условия проверки отклика перенаправления содержатся в разделе Служба [автообнаружения для Exchange](autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="a16b6-164">For criteria for validating a redirection response, see [Autodiscover for Exchange](autodiscover-for-exchange.md).</span></span> 
  
<span data-ttu-id="a16b6-165">Если служба автообнаружения возвращает ответ на перенаправление, который указывается элементом [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **усерреспонсе** , клиентское приложение должно использовать элемент **редиректтаржет** для создания нового запроса на параметры, который отправляется на сервер, указанный в ответе на перенаправление.</span><span class="sxs-lookup"><span data-stu-id="a16b6-165">If the Autodiscover service returns a redirection response, indicated by the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element, your client application should use the **RedirectTarget** element to construct a new settings request that is sent to the server specified in the redirection response.</span></span> <span data-ttu-id="a16b6-166">В следующем примере показан ответ перенаправления от сервера.</span><span class="sxs-lookup"><span data-stu-id="a16b6-166">The following example shows a redirection response from the server.</span></span> 
  
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

<span data-ttu-id="a16b6-167">После перенаправления клиент использует URL-адрес перенаправления, чтобы подготовить еще один запрос.</span><span class="sxs-lookup"><span data-stu-id="a16b6-167">After a redirection, the client uses the redirection URL to prepare another request.</span></span> <span data-ttu-id="a16b6-168">В приведенном ниже коде показан пример запроса, созданного на основе ответа на перенаправление.</span><span class="sxs-lookup"><span data-stu-id="a16b6-168">The following code shows an example of the request that you create from the redirection response.</span></span>
  
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

<span data-ttu-id="a16b6-169">Когда клиентское приложение направляется в правильную конечную точку для службы автообнаружения, сервер отправит ответ с элементом [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) элемента **усерреспонсе** , установленным в значение " **Ошибка** ", и содержащий запрошенные параметры пользователя.</span><span class="sxs-lookup"><span data-stu-id="a16b6-169">When the client application has been directed to the correct endpoint for the Autodiscover service, the server will send a response with the [ErrorCode](http://msdn.microsoft.com/library/0bb00cee-c66b-4f34-b99d-355458f5e83b%28Office.15%29.aspx) element of the **UserResponse** element set to **NoError** and containing the requested user settings.</span></span> <span data-ttu-id="a16b6-170">Возвращаются только запрошенные параметры пользователя, **интерналевсурл** и **екстерналевсурл**.</span><span class="sxs-lookup"><span data-stu-id="a16b6-170">Only the requested user settings, **InternalEwsUrl** and **ExternalEwsUrl**, are returned.</span></span> <span data-ttu-id="a16b6-171">В следующем примере показан ответ от сервера.</span><span class="sxs-lookup"><span data-stu-id="a16b6-171">The following example shows the response from the server.</span></span> 
  
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

## <a name="next-steps"></a><span data-ttu-id="a16b6-172">Дальнейшие действия</span><span class="sxs-lookup"><span data-stu-id="a16b6-172">Next steps</span></span>
<span data-ttu-id="a16b6-173"><a name="bk_Next"> </a></span><span class="sxs-lookup"><span data-stu-id="a16b6-173"><a name="bk_Next"> </a></span></span>

<span data-ttu-id="a16b6-174">Поиск конечной точки с помощью процесса автообнаружения возвращает запрошенный домен или параметры пользователя.</span><span class="sxs-lookup"><span data-stu-id="a16b6-174">Finding the endpoint by following the Autodiscover process returns the requested domain or user settings.</span></span> <span data-ttu-id="a16b6-175">Сведения о том, как сделать запрос на определенные параметры, можно найти в следующих статьях:</span><span class="sxs-lookup"><span data-stu-id="a16b6-175">For information about making a request for specific settings, see the following articles:</span></span>
  
- [<span data-ttu-id="a16b6-176">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-176">Get domain settings from an Exchange server</span></span>](how-to-get-domain-settings-from-an-exchange-server.md)    
- [<span data-ttu-id="a16b6-177">Получение параметров пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a16b6-177">Get user settings from Exchange by using Autodiscover</span></span>](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    
## <a name="see-also"></a><span data-ttu-id="a16b6-178">См. также</span><span class="sxs-lookup"><span data-stu-id="a16b6-178">See also</span></span>

- [<span data-ttu-id="a16b6-179">Настройка приложения веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-179">Setting up your EWS application</span></span>](setting-up-your-ews-application.md)   
- [<span data-ttu-id="a16b6-180">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-180">Autodiscover for Exchange</span></span>](autodiscover-for-exchange.md)    
- [<span data-ttu-id="a16b6-181">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-181">Autodiscover web service reference for Exchange</span></span>](http://msdn.microsoft.com/library/a01124a8-a8cf-4b80-8625-d7ee05690bca%28Office.15%29.aspx)    
- [<span data-ttu-id="a16b6-182">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="a16b6-182">EWS reference for Exchange</span></span>](http://msdn.microsoft.com/library/2a873474-1bb2-4cb1-a556-40e8c4159f4a%28Office.15%29.aspx)
    

