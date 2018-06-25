---
title: Элементы XML веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Найдите справочные сведения для веб-служб Exchange XML элементы в Exchange.
ms.openlocfilehash: 046a985ae4696616d28a0891ffe0aa8cc0552307
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762412"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="282f9-103">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="282f9-104">Найдите справочные сведения для веб-служб Exchange XML элементы в Exchange.</span><span class="sxs-lookup"><span data-stu-id="282f9-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="282f9-105">Веб-служб Exchange (EWS) — это служба веб-SOAP, что означает, что запрос и ответ сообщения, отправленные между клиентом и сервером состоят из XML-элементы.</span><span class="sxs-lookup"><span data-stu-id="282f9-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="282f9-106">В этом разделе документации основано на экземпляры XML, отправленные между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="282f9-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="282f9-107">Экземпляры XML определяются в файлах WSDL и схемы, которые расположены в виртуальном каталоге, на котором размещается веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="282f9-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="282f9-108">Пользователям, прошедшим проверку подлинности пользователя могут просматривать файлы WSDL и схемы с помощью следующие URL-адреса, где \<yourclientaccessserver\> — это имя сервера клиентского доступа:</span><span class="sxs-lookup"><span data-stu-id="282f9-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="282f9-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — расположение WSDL-файла.</span><span class="sxs-lookup"><span data-stu-id="282f9-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="282f9-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — расположение схемы сообщений.</span><span class="sxs-lookup"><span data-stu-id="282f9-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="282f9-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — расположение схемы типов.</span><span class="sxs-lookup"><span data-stu-id="282f9-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="282f9-112">Файлы схемы, которые описывают элементы XML веб-служб Exchange предоставляют общие схема XML структуры, возможно, для взаимодействия сообщения запросов и ответов.</span><span class="sxs-lookup"><span data-stu-id="282f9-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="282f9-113">Фактические XML-структура, пересылаемые между клиентом и сервером изменяется в зависимости от операции, который будет вызываться, нужные данные и параметры на сервере.</span><span class="sxs-lookup"><span data-stu-id="282f9-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="282f9-114">Веб-служб Exchange WSDL-файла, services.wsdl, не соответствует полностью стандартный WSDL-ФАЙЛУ, так как он не включает определение WSDL службы.</span><span class="sxs-lookup"><span data-stu-id="282f9-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="282f9-115">Это так, как веб-служб Exchange не может быть размещены на компьютере с предварительно заданных адресов.</span><span class="sxs-lookup"><span data-stu-id="282f9-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="282f9-116">Можно использовать службу автообнаружения для получения адреса конечной точки веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="282f9-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="282f9-117">Некоторые генераторы клиентскую объектную модель анализа WSDL-файла и могут возникнуть ошибки, так как WSDL-файла не содержит определение WSDL службы.</span><span class="sxs-lookup"><span data-stu-id="282f9-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="282f9-118">Если генератор объектной модели возникают ошибки, можно вставить заполнитель определения службы WSDL.</span><span class="sxs-lookup"><span data-stu-id="282f9-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="282f9-119">Если вы используете .NET Framework для разработки приложения, рекомендуется использовать [Управляемый API веб-служб Exchange](http://aka.ms/ews-managed-api-readme), а не генератор объектной модели.</span><span class="sxs-lookup"><span data-stu-id="282f9-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="282f9-120">Управляемый API веб-служб Exchange предоставляет простой в использовании объектную модель для обработки сериализации и десериализации XML веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="282f9-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="282f9-121">Дополнительные сведения можно [приступить к работе с клиентскими приложениями, управляемый API веб-служб Exchange](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="282f9-121">For more information, see [Get started with EWS Managed API client applications](http://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="282f9-122">Файл схемы messages.xsd содержит определения элементов для элементов верхнего уровня в тексте запроса SOAP.</span><span class="sxs-lookup"><span data-stu-id="282f9-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="282f9-123">За исключением коды ответа об ошибках большая часть определения в messages.xsd относятся только к операции.</span><span class="sxs-lookup"><span data-stu-id="282f9-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="282f9-124">Схема types.xsd содержит определения для заголовков SOAP и общие определения, которые являются общими для операций.</span><span class="sxs-lookup"><span data-stu-id="282f9-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="282f9-125">См. также</span><span class="sxs-lookup"><span data-stu-id="282f9-125">See also</span></span>

- [<span data-ttu-id="282f9-126">Справка по веб-служб Exchange для Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="282f9-127">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="282f9-128">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="282f9-129">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="282f9-130">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="282f9-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

