---
title: XML-элементы автообнаружения SOAP для Exchange 2013
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: ae18a5b3-ae44-4cff-8654-db8028565e01
description: Найдите справочные сведения о XML-элементе для веб-службы автообнаружения SOAP в Exchange.
ms.openlocfilehash: 3b88429488dbecd4ed7c3adf56462f34fa0d4b17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465186"
---
# <a name="soap-autodiscover-xml-elements-for-exchange-2013"></a><span data-ttu-id="11818-103">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="11818-103">SOAP Autodiscover XML elements for Exchange 2013</span></span>

<span data-ttu-id="11818-104">Найдите справочные сведения о XML-элементе для веб-службы автообнаружения SOAP в Exchange.</span><span class="sxs-lookup"><span data-stu-id="11818-104">Find XML element reference information for the SOAP Autodiscover web service in Exchange.</span></span>
  
<span data-ttu-id="11818-105">Документация в этом разделе основана на экземплярах XML-элементов автообнаружения SOAP, которые передаются между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="11818-105">The documentation in this section is based on the SOAP Autodiscover XML element instances that are sent between the client and server.</span></span> <span data-ttu-id="11818-106">Эта документация по экземпляру XML основана на файлах WSDL и Schema, расположенных в виртуальном каталоге, где размещается служба автообнаружения SOAP.</span><span class="sxs-lookup"><span data-stu-id="11818-106">This XML instance documentation is based on the WSDL and schema files that are located in the virtual directory that hosts the SOAP Autodiscover service.</span></span> <span data-ttu-id="11818-107">Пользователи, прошедшие проверку подлинности, могут перейти к файлам WSDL и Schema, используя URL-адрес, подобный одному из следующих:</span><span class="sxs-lookup"><span data-stu-id="11818-107">Authenticated users can browse to the WSDL and schema files by using a URL that is similar to one of the following:</span></span>
  
- <span data-ttu-id="11818-108">Расположение WSDL-файла: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span><span class="sxs-lookup"><span data-stu-id="11818-108">The location of the WSDL file: `http://<yourclientaccessserver>.com/autodiscover/services.wsdl` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/services.wsdl`</span></span>
    
- <span data-ttu-id="11818-109">Расположение схемы messages: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` или`http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span><span class="sxs-lookup"><span data-stu-id="11818-109">The location of the messages schema: `http://<yourclientaccessserver>.com/autodiscover/messages.xsd` or `http://autodiscover.<yourclientaccessserver>.com/autodiscover/messages.xsd`</span></span> 
    
<span data-ttu-id="11818-110">Расположение WSDL и файлов схемы автообнаружения SOAP зависит от установки Exchange.</span><span class="sxs-lookup"><span data-stu-id="11818-110">The location of the SOAP Autodiscover WSDL and schema files varies based on the Exchange installation.</span></span>
  
<span data-ttu-id="11818-111">В файле схемы messages. xsd описываются элементы XML, которые можно отправить в заголовке SOAP автообнаружения и теле SOAP.</span><span class="sxs-lookup"><span data-stu-id="11818-111">The messages.xsd schema file describes the XML elements that can be sent in an Autodiscover SOAP header and SOAP body.</span></span> <span data-ttu-id="11818-112">В этом файле представлен общий обзор структуры XML, которую можно использовать для взаимодействия с сообщением о ответе на запрос.</span><span class="sxs-lookup"><span data-stu-id="11818-112">This file provides a general roadmap of what the XML structure can be for a given request-response message interaction.</span></span> <span data-ttu-id="11818-113">Фактическая структура XML, которая передается между клиентом и сервером, основана на параметрах и контексте, в котором они используются.</span><span class="sxs-lookup"><span data-stu-id="11818-113">The actual XML structure that is sent between the client and server is based on the options and the context in which it is used.</span></span> <span data-ttu-id="11818-114">Файлы схемы определяют, какой возможен XML-файл.</span><span class="sxs-lookup"><span data-stu-id="11818-114">The schema files define what XML is possible.</span></span> <span data-ttu-id="11818-115">Фактический диапазон XML-данных, передаваемых по сети, зависит от того, какая операция вызывается, запрашиваемые сведения и параметры на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="11818-115">The actual range of XML that is sent over the wire is based on which operation is called, the requested information, and the server-side settings.</span></span> 
  
## <a name="related-sections"></a><span data-ttu-id="11818-116">Связанные разделы</span><span class="sxs-lookup"><span data-stu-id="11818-116">Related sections</span></span>

- [<span data-ttu-id="11818-117">Справочник по веб-службе автообнаружения SOAP для Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-117">SOAP Autodiscover web service reference for Exchange</span></span>](soap-autodiscover-web-service-reference-for-exchange.md)    
- [<span data-ttu-id="11818-118">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-118">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)    
- [<span data-ttu-id="11818-119">Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-119">Unified Messaging web service reference for Exchange</span></span>](unified-messaging-web-service-reference-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="11818-120">См. также</span><span class="sxs-lookup"><span data-stu-id="11818-120">See also</span></span>

- [<span data-ttu-id="11818-121">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-121">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="11818-122">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-122">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="11818-123">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="11818-123">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

