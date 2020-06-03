---
title: Справочник по веб-службе автообнаружения POX для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Найдите справочные сведения о службе автообнаружения POX в Exchange.
ms.openlocfilehash: 3c0ca368f4427be7759e2db58fb418b4822dea8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465655"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="9209e-103">Справочник по веб-службе автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="9209e-104">Найдите справочные сведения о службе автообнаружения POX в Exchange.</span><span class="sxs-lookup"><span data-stu-id="9209e-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="9209e-105">Служба автообнаружения предоставляет сведения о конфигурации, которые приложение использует для создания подключения к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="9209e-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="9209e-106">Службу автообнаружения "Plain Old XML" (POX) можно использовать для отправки сообщений, состоящих только из полезных данных XML, без почтовых конвертов SOAP, чтобы определить параметры, которые должны быть у клиентского приложения для подключения к Exchange.</span><span class="sxs-lookup"><span data-stu-id="9209e-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="9209e-107">Для клиентов, использующих версии Exchange, начиная с Exchange Server 2010, рекомендуется использовать службу автообнаружения SOAP вместо службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="9209e-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="9209e-108">Клиентам, которые нацелены на Exchange 2007, необходимо использовать службу автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="9209e-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="9209e-109">Мы рекомендуем использовать для клиентов, использующих платформу .NET Framework, управляемый API EWS, так как он содержит надежный и хорошо протестированный клиент автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="9209e-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="9209e-110">Дополнительные сведения об управляемом API EWS можно найти в статье Начало [работы с клиентскими приложениями для управляемого API EWS](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="9209e-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="9209e-111">В этом разделе представлены сведения об элементах XML, которые передаются между клиентом и сервером во время перенаправлений запросов автообнаружения POX, и пользовательских параметров, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="9209e-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="9209e-112">Справочник по XML-элементам содержит сводки элементов, которые представляют элементы, и описание потенциальных иерархий элементов, использующих этот элемент.</span><span class="sxs-lookup"><span data-stu-id="9209e-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="9209e-113">В этой документации описываются экземпляры XML, которые передаются между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="9209e-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="9209e-114">Служба автообнаружения POX не имеет явной схемы.</span><span class="sxs-lookup"><span data-stu-id="9209e-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="9209e-115">В статьях этого раздела приводятся примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="9209e-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="9209e-116">В этой статье</span><span class="sxs-lookup"><span data-stu-id="9209e-116">In this section</span></span>
<span data-ttu-id="9209e-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="9209e-117"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="9209e-118">Запрос автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="9209e-119">Отклик автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="9209e-120">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="9209e-121">См. также</span><span class="sxs-lookup"><span data-stu-id="9209e-121">See also</span></span>

- [<span data-ttu-id="9209e-122">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="9209e-123">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="9209e-124">Справочник по веб-службе автообнаружения SOAP для Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="9209e-125">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="9209e-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

