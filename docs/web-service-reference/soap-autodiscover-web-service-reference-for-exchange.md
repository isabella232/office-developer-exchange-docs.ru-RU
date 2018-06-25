---
title: SOAP ссылку веб-службы автообнаружения для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Найдите справочные сведения для службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 1cb24a8667c71028f3dead78d9fa533dc9547a64
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835514"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="99f87-103">SOAP ссылку веб-службы автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="99f87-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="99f87-104">Найдите справочные сведения для службы автообнаружения SOAP в Exchange.</span><span class="sxs-lookup"><span data-stu-id="99f87-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="99f87-105">Служба автообнаружения предоставляет сведения о конфигурации, используемые приложением для создания подключения к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="99f87-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="99f87-106">Служба автообнаружения SOAP можно использовать для отправки сообщений между клиентским приложением и Exchange server, чтобы найти параметры приложения будет использоваться для подключения к Exchange.</span><span class="sxs-lookup"><span data-stu-id="99f87-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="99f87-107">В отличие от службы автообнаружения POX служба автообнаружения SOAP обеспечивает пакетных запросах автообнаружения для параметров количество пользователей и более детальный контроль над тем, какие параметры возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="99f87-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="99f87-108">Для клиентов, предназначенных для версии Exchange, начиная с Exchange Server 2010 мы рекомендуем использовать службы автообнаружения SOAP (вместо службы автообнаружения POX).</span><span class="sxs-lookup"><span data-stu-id="99f87-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="99f87-109">Клиенты, предназначенных для Exchange 2007 необходимо использовать службу автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="99f87-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="99f87-110">Мы рекомендуем, что клиентов, использующих .NET Framework использовать управляемый API EWS, так как он содержит надежных и хорошо проверенные клиента автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="99f87-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="99f87-111">Дополнительные сведения о управляемый API EWS можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="99f87-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="99f87-112">В этом разделе приведены сведения об XML-элементы, отправленные между клиентом и сервером во время перенаправления запроса SOAP автообнаружения и параметров пользователя, которые возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="99f87-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="99f87-113">Справочник по элементам XML содержит элементы представления сводки и описание возможных иерархии элементов, которые содержат элемент.</span><span class="sxs-lookup"><span data-stu-id="99f87-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="99f87-114">В статьях этого раздела описывается экземпляры XML, отправленные между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="99f87-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="99f87-115">Схема, описывающая этих элементов можно найти в виртуальном каталоге сервера, на котором размещается служба автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="99f87-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="99f87-116">Операции WSDL, в этом разделе описываются что не обзор операций и примеры операция запроса и ответа.</span><span class="sxs-lookup"><span data-stu-id="99f87-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="99f87-117">Можно использовать сведения о версии, для определения, доступны ли компоненты, которые вы хотите использовать в версию продукта, выполняется.</span><span class="sxs-lookup"><span data-stu-id="99f87-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="99f87-118">Примеров в разделах операции помогут понять структуру XML, который включен в сообщения SOAP, и с сервера.</span><span class="sxs-lookup"><span data-stu-id="99f87-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="99f87-119">В этом разделе также приведены примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="99f87-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="99f87-120">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="99f87-120">In this section</span></span>
<span data-ttu-id="99f87-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="99f87-121"></span></span>

- [<span data-ttu-id="99f87-122">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="99f87-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="99f87-123">Операция GetFederationInformation (SOAP)</span><span class="sxs-lookup"><span data-stu-id="99f87-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="99f87-124">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="99f87-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="99f87-125">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="99f87-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="99f87-126">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="99f87-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="99f87-127">См. также</span><span class="sxs-lookup"><span data-stu-id="99f87-127">See also</span></span>


- [<span data-ttu-id="99f87-128">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="99f87-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="99f87-129">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="99f87-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="99f87-130">Использование службы автообнаружения для поиска точек подключения</span><span class="sxs-lookup"><span data-stu-id="99f87-130">Use Autodiscover to find connection points</span></span>](http://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="99f87-131">Получить параметры пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="99f87-131">Get user settings from Exchange by using Autodiscover</span></span>](http://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="99f87-132">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="99f87-132">Get domain settings from an Exchange server</span></span>](http://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="99f87-133">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="99f87-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

