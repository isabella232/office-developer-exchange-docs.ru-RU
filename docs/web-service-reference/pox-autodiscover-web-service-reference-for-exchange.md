---
title: Служба POX автоматического обнаружения веб-ссылки для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 877152f0-f4b1-4f63-b2ce-924f4bdf2d20
description: Найдите справочные сведения для службы автообнаружения POX в Exchange.
ms.openlocfilehash: a8797fe714fd23049094c3ec2475b93fec4282c0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834867"
---
# <a name="pox-autodiscover-web-service-reference-for-exchange"></a><span data-ttu-id="2adfe-103">Служба POX автоматического обнаружения веб-ссылки для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-103">POX Autodiscover web service reference for Exchange</span></span>

<span data-ttu-id="2adfe-104">Найдите справочные сведения для службы автообнаружения POX в Exchange.</span><span class="sxs-lookup"><span data-stu-id="2adfe-104">Find reference information for the POX Autodiscover service in Exchange.</span></span>
  
<span data-ttu-id="2adfe-105">Служба автообнаружения предоставляет сведения о конфигурации, используемые приложением для создания подключения к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="2adfe-105">The Autodiscover service provides the configuration information that your application uses to create a connection to an Exchange server.</span></span> <span data-ttu-id="2adfe-106">Можно использовать «Обычная старые XML» службы автообнаружения (POX) для отправки сообщений, которые состоят только из полезных данных XML, без любого заключающего конверты SOAP для обнаружения параметров, которые необходимо клиентское приложение для подключения к Exchange.</span><span class="sxs-lookup"><span data-stu-id="2adfe-106">You can use the "plain old XML" (POX) Autodiscover service to send messages that consist only of XML payloads, without any enclosing SOAP envelopes, in order to locate the settings that a client application must have in order to connect to Exchange.</span></span>
  
> [!NOTE]
> <span data-ttu-id="2adfe-107">Для клиентов, предназначенных для версии Exchange, начиная с Exchange Server 2010 мы рекомендуем использовать службу автообнаружения SOAP вместо службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="2adfe-107">For clients that target versions of Exchange starting with Exchange Server 2010, we recommend that you use the SOAP Autodiscover service instead of the POX Autodiscover service.</span></span> <span data-ttu-id="2adfe-108">Клиенты, предназначенных для Exchange 2007 необходимо использовать службу автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="2adfe-108">Clients that target Exchange 2007 have to use the POX Autodiscover service.</span></span> <span data-ttu-id="2adfe-109">Мы рекомендуем, что клиентов, использующих .NET Framework использовать управляемый API EWS, так как он содержит надежных и хорошо проверенные автообнаружения POX клиента.</span><span class="sxs-lookup"><span data-stu-id="2adfe-109">We recommend that clients that use the .NET Framework use the EWS Managed API because it contains a robust and well-tested POX Autodiscover client.</span></span> <span data-ttu-id="2adfe-110">Дополнительные сведения о управляемый API EWS можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2adfe-110">For more information about the EWS Managed API, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="2adfe-111">В этом разделе приведены сведения об XML-элементы, отправленные между клиентом и сервером во время перенаправления запроса POX автообнаружения и параметров пользователя, которые возвращаются в ответе.</span><span class="sxs-lookup"><span data-stu-id="2adfe-111">This section provides information about the XML elements that are sent between the client and server during POX Autodiscover request redirections and the user settings that are returned in a response.</span></span> <span data-ttu-id="2adfe-112">Справочник по элементам XML содержит элементы представления сводки и описание возможных иерархии элементов, используйте элемент.</span><span class="sxs-lookup"><span data-stu-id="2adfe-112">The XML element reference contains summaries of what the elements represent and a description of the potential element hierarchies that use the element.</span></span> <span data-ttu-id="2adfe-113">В этой документации описываются экземпляры XML, отправленные между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="2adfe-113">This documentation covers the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="2adfe-114">Служба автообнаружения POX нет явных схемы.</span><span class="sxs-lookup"><span data-stu-id="2adfe-114">The POX Autodiscover service does not have an explicit schema.</span></span>
  
<span data-ttu-id="2adfe-115">В статьях в этом разделе приведены примеры и описания сообщений, которые используются для получения сведений о конфигурации автообнаружения с помощью службы автообнаружения POX.</span><span class="sxs-lookup"><span data-stu-id="2adfe-115">The articles in this section provide examples and descriptions of the messages that are used to retrieve Autodiscover configuration information by using the POX Autodiscover service.</span></span> 
  
## <a name="in-this-section"></a><span data-ttu-id="2adfe-116">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="2adfe-116">In this section</span></span>
<span data-ttu-id="2adfe-117"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="2adfe-117"></span></span>

- [<span data-ttu-id="2adfe-118">Запрос автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-118">POX Autodiscover request for Exchange</span></span>](pox-autodiscover-request-for-exchange.md)
    
- [<span data-ttu-id="2adfe-119">POX ответа службы автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-119">POX Autodiscover response for Exchange</span></span>](pox-autodiscover-response-for-exchange.md)
    
- [<span data-ttu-id="2adfe-120">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-120">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="2adfe-121">См. также</span><span class="sxs-lookup"><span data-stu-id="2adfe-121">See also</span></span>

- [<span data-ttu-id="2adfe-122">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-122">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="2adfe-123">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-123">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)   
- [<span data-ttu-id="2adfe-124">SOAP ссылку веб-службы автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-124">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="2adfe-125">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="2adfe-125">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

