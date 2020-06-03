---
title: Справочник по веб-службе автообнаружения SOAP для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 61c21ea9-7fea-4f56-8ada-bf80e1e6b074
description: Найдите справочные сведения о службе автообнаружения SOAP в Exchange.
ms.openlocfilehash: bfca8e8e260a6262d12542bd6834894a2375453f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468427"
---
# <a name="soap-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="9789c-103">Справочник по веб-службе автообнаружения SOAP для Exchange</span><span class="sxs-lookup"><span data-stu-id="9789c-103">SOAP Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="9789c-104">Найдите справочные сведения о службе автообнаружения SOAP в Exchange.</span><span class="sxs-lookup"><span data-stu-id="9789c-104">Find reference information for the SOAP Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="9789c-105">Служба автообнаружения предоставляет сведения о конфигурации, которые приложение использует для создания подключения к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="9789c-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="9789c-106">Службу автообнаружения SOAP можно использовать для отправки сообщений между клиентским приложением и сервером Exchange Server для обнаружения параметров, которые приложение будет использовать для подключения к Exchange.</span><span class="sxs-lookup"><span data-stu-id="9789c-106">You can use the SOAP Autodiscover service to send messages between the client application and the Exchange server to locate the settings the application will use to connect to Exchange.</span></span> <span data-ttu-id="9789c-107">В отличие от службы автообнаружения POX служба автообнаружения SOAP позволяет пакетным запросам на обнаружение для множества параметров пользователей и более детально контролировать, какие параметры возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="9789c-107">Unlike the POX Autodiscover service, the SOAP Autodiscover service allows for batched Autodiscover requests for many users' settings and more granular control over which settings are returned in the response.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9789c-108">Для клиентов, использующих версии Exchange, начиная с Exchange Server 2010, рекомендуется использовать службу автообнаружения SOAP (вместо службы автообнаружения POX).</span><span class="sxs-lookup"><span data-stu-id="9789c-108">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service (instead of the POX Autodiscover service).</span></span> <span data-ttu-id="9789c-109">Клиентам, которые нацелены на Exchange 2007, необходимо использовать службу автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="9789c-109">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="9789c-110">Мы рекомендуем использовать для клиентов, использующих платформу .NET Framework, управляемый API EWS, так как он содержит надежный и хорошо протестированный клиент автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="9789c-110">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested SOAP Autodiscover client.</span></span> <span data-ttu-id="9789c-111">Дополнительные сведения об управляемом API EWS можно найти в статье Начало [работы с клиентскими приложениями для управляемого API EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9789c-111">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="9789c-112">В этом разделе представлены сведения об элементах XML, которые передаются между клиентом и сервером во время перенаправления запросов автообнаружения SOAP, и пользовательских параметров, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="9789c-112">This section provides information about the XML elements that are sent between the client and server during SOAP Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="9789c-113">Справочник по XML-элементам содержит сводки элементов, которые представляют элементы, и описание потенциальных иерархий элементов, содержащих элемент.</span><span class="sxs-lookup"><span data-stu-id="9789c-113">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that contain the element.</span></span> 
  
<span data-ttu-id="9789c-114">В статьях этого раздела описываются экземпляры XML, которые передаются между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="9789c-114">The articles in this section describe the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="9789c-115">Схема, описывающая эти элементы, можно найти в виртуальном каталоге сервера, на котором размещается служба автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="9789c-115">The schema that describes these elements can be found in the virtual directory of the server that hosts the SOAP Autodiscover service.</span></span>
  
<span data-ttu-id="9789c-116">В разделах, посвященных операциям WSDL, представлены общие сведения о действиях, выполняемых операцией и примерах запросов операций и ответов.</span><span class="sxs-lookup"><span data-stu-id="9789c-116">The WSDL operation topics in this section provide an overview of what the operation does and operation request and response examples.</span></span> <span data-ttu-id="9789c-117">Вы можете использовать сведения о версии, чтобы определить, доступны ли функции, которые вы хотите использовать, в используемой версии продукта.</span><span class="sxs-lookup"><span data-stu-id="9789c-117">You can use the version information provided to determine whether the features that you want to use are available in the product version that you are running.</span></span> <span data-ttu-id="9789c-118">Примеры в разделах, посвященных операциям, также помогут разознать структуру XML, которая включена в сообщения SOAP, отправляемые на сервер и с сервера.</span><span class="sxs-lookup"><span data-stu-id="9789c-118">The examples in the operation topics also help you to understand the structure of the XML that is included in the SOAP messages that are sent to and from the server.</span></span>
  
<span data-ttu-id="9789c-119">В этом разделе также приведены примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="9789c-119">This section also provides examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the SOAP Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="9789c-120">В этой статье</span><span class="sxs-lookup"><span data-stu-id="9789c-120">In this section</span></span>
<span data-ttu-id="9789c-121"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="9789c-121"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="9789c-122">Операция Жетдомаинсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9789c-122">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
    
- [<span data-ttu-id="9789c-123">Операция Жетфедератионинформатион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9789c-123">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)
    
- [<span data-ttu-id="9789c-124">Операция GetUserSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9789c-124">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
    
- [<span data-ttu-id="9789c-125">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="9789c-125">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)
    
- [<span data-ttu-id="9789c-126">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="9789c-126">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)
    
## <a name="see-also"></a><span data-ttu-id="9789c-127">См. также</span><span class="sxs-lookup"><span data-stu-id="9789c-127">See also</span></span>


- [<span data-ttu-id="9789c-128">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="9789c-128">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="9789c-129">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="9789c-129">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="9789c-130">Поиск точек соединения с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="9789c-130">Use Autodiscover to find connection points</span></span>](https://msdn.microsoft.com/library/03896542-549b-4c45-973c-98f9025ea26c%28Office.15%29.aspx)
- [<span data-ttu-id="9789c-131">Получение параметров пользователя из Exchange с помощью службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="9789c-131">Get user settings from Exchange by using Autodiscover</span></span>](https://msdn.microsoft.com/library/6d90c305-4802-4e18-8d52-f60349feaa8d%28Office.15%29.aspx)
- [<span data-ttu-id="9789c-132">Получение параметров домена с сервера Exchange</span><span class="sxs-lookup"><span data-stu-id="9789c-132">Get domain settings from an Exchange server</span></span>](https://msdn.microsoft.com/library/2f9acb81-5135-4f72-94e8-65c235d725e6%28Office.15%29.aspx)
- [<span data-ttu-id="9789c-133">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="9789c-133">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

