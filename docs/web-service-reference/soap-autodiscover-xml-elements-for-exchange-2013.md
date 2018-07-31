---
title: Элементы XML автоматического обнаружения SOAP для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Найдите XML элемент справочные сведения для веб-службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353394"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="695cd-103">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="695cd-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="695cd-104">Найдите XML элемент справочные сведения для веб-службы автообнаружения SOAP в Exchange.</span><span class="sxs-lookup"><span data-stu-id="695cd-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="695cd-105">В этом разделе документации основано на экземпляры элемент XML автоматического обнаружения SOAP, отправленные между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="695cd-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="695cd-106">В этой документации экземпляр XML основано на WSDL и схеме файлы, расположенные в виртуальном каталоге, на котором размещается служба автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="695cd-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="695cd-107">Прошедшего проверку подлинности пользователи могут просматривать файлы WSDL и схемы с помощью URL-адреса, который похож на один из следующих:</span><span class="sxs-lookup"><span data-stu-id="695cd-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="695cd-108">Расположение WSDL-файла: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="695cd-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="695cd-109">Расположение схемы сообщений: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="695cd-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="695cd-110">Расположение службы автообнаружения WSDL SOAP и схеме файлов зависит от установки Exchange.</span><span class="sxs-lookup"><span data-stu-id="695cd-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="695cd-111">Файл схемы messages.xsd описывает XML-элементы, которые могут быть отправлены в SOAP автообнаружения заголовок и тело SOAP.</span><span class="sxs-lookup"><span data-stu-id="695cd-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="695cd-112">Этот файл предоставляет общая схема XML-структура может быть для диалога сообщения заданного запросов и ответов.</span><span class="sxs-lookup"><span data-stu-id="695cd-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="695cd-113">Фактические XML-структура, пересылаемые между клиентом и сервером на основе параметров и контекст, в котором она используется.</span><span class="sxs-lookup"><span data-stu-id="695cd-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="695cd-114">Файлы схемы определения возможности возможные XML.</span><span class="sxs-lookup"><span data-stu-id="695cd-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="695cd-115">Фактический диапазон XML, отправляемые по сети основано на какие операция называется запрошенные данные и параметры на сервере.</span><span class="sxs-lookup"><span data-stu-id="695cd-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="695cd-116">Связанные разделы</span><span class="sxs-lookup"><span data-stu-id="695cd-116">Related sections</span></span>

- [<span data-ttu-id="695cd-117">SOAP ссылку веб-службы автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="695cd-118">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="695cd-119">Единой системы обмена сообщениями веб-службы ссылки для Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="695cd-120">См. также</span><span class="sxs-lookup"><span data-stu-id="695cd-120">See also</span></span>

- [<span data-ttu-id="695cd-121">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="695cd-122">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="695cd-123">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="695cd-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

