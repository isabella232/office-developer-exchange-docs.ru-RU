---
title: Элементы XML веб-служб Exchange в Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
api_name:
- Exchange
api_type:
- schema
ms.assetid: 4653466a-a596-456f-bbff-7da4ef1d18d3
description: Справочные сведения о XML-элементах EWS в Exchange.
localization_priority: Priority
ms.openlocfilehash: 29b90ad137141e30484ef804b6fcb6bb049ef3e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526118"
---
# <a name="ews-xml-elements-in-exchange"></a><span data-ttu-id="e67a5-103">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-103">EWS XML elements in Exchange</span></span>

<span data-ttu-id="e67a5-104">Справочные сведения о XML-элементах EWS в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e67a5-104">Find reference information for the EWS XML elements in Exchange.</span></span>
  
<span data-ttu-id="e67a5-105">Веб-службы Exchange (EWS) — это веб-служба на основе SOAP, которая означает, что сообщения запроса и ответа, которые передаются между клиентом и сервером, состоят из XML-элементов.</span><span class="sxs-lookup"><span data-stu-id="e67a5-105">Exchange Web Services (EWS) is a SOAP-based web service, which means that the request and response messages that are sent between the client and server are comprised of XML elements.</span></span> <span data-ttu-id="e67a5-106">Документация в этом разделе основана на экземплярах XML, которые передаются между клиентом и сервером.</span><span class="sxs-lookup"><span data-stu-id="e67a5-106">The documentation in this section is based on the XML instances that are sent between the client and server.</span></span> <span data-ttu-id="e67a5-107">Экземпляры XML определяются в файлах WSDL и Schema, расположенных в виртуальном каталоге, на котором размещается EWS.</span><span class="sxs-lookup"><span data-stu-id="e67a5-107">The XML instances are defined in the WSDL and schema files that are located in the virtual directory that hosts EWS.</span></span> <span data-ttu-id="e67a5-108">Если вы прошедший проверку подлинности пользователя, вы можете перейти к файлам WSDL и Schema, используя следующие URL-адреса, где \<yourclientaccessserver\> — имя сервера клиентского доступа:</span><span class="sxs-lookup"><span data-stu-id="e67a5-108">If you are an authenticated user, you can browse to the WSDL and schema files by using the following URLs, where \<yourclientaccessserver\> is the name of your Client Access server:</span></span>
  
- <span data-ttu-id="e67a5-109">http:// \<yourclientaccessserver\> . com/EWS/Services. WSDL — расположение WSDL-файла.</span><span class="sxs-lookup"><span data-stu-id="e67a5-109">http://\<yourclientaccessserver\>.com/ews/services.wsdl — The location of the WSDL file.</span></span>
    
- <span data-ttu-id="e67a5-110">http:// \<yourclientaccessserver\> . com/EWS/messages. xsd — расположение схемы messages.</span><span class="sxs-lookup"><span data-stu-id="e67a5-110">http://\<yourclientaccessserver\>.com/ews/messages.xsd — The location of the messages schema.</span></span>
    
- <span data-ttu-id="e67a5-111">http:// \<yourclientaccessserver\> . com/EWS/Types. xsd — расположение схемы типов.</span><span class="sxs-lookup"><span data-stu-id="e67a5-111">http://\<yourclientaccessserver\>.com/ews/types.xsd — The location of the types schema.</span></span>
    
<span data-ttu-id="e67a5-112">Файлы схемы, описывающие элементы XML EWS, предоставляют общий план структуры XML, который можно использовать для взаимодействия с сообщениями request-response.</span><span class="sxs-lookup"><span data-stu-id="e67a5-112">The schema files that describe the EWS XML elements provide a general roadmap of the XML structure that is possible for request-response message interactions.</span></span> <span data-ttu-id="e67a5-113">Реальная структура XML, которая передается между клиентом и сервером, зависит от вызываемой операции, запрашиваемых сведений и параметров на стороне сервера.</span><span class="sxs-lookup"><span data-stu-id="e67a5-113">The actual XML structure that is sent between client and server varies according to the operation that is called, the information requested, and the server-side settings.</span></span>
  
<span data-ttu-id="e67a5-114">WSDL-файл EWS, Services. WSDL, не полностью соответствует стандарту WSDL, так как он не включает определение службы WSDL.</span><span class="sxs-lookup"><span data-stu-id="e67a5-114">The EWS WSDL file, services.wsdl, does not fully conform to the WSDL standard because it does not include a WSDL service definition.</span></span> <span data-ttu-id="e67a5-115">Это вызвано тем, что веб-сервер EWS не предназначен для размещения на компьютере с предварительно определенным адресом.</span><span class="sxs-lookup"><span data-stu-id="e67a5-115">This is because EWS is not designed to be hosted on a computer that has a predefined address.</span></span> <span data-ttu-id="e67a5-116">Вы можете использовать службу автообнаружения, чтобы получить адрес конечной точки EWS.</span><span class="sxs-lookup"><span data-stu-id="e67a5-116">You can use the Autodiscover service to get the EWS endpoint address.</span></span> <span data-ttu-id="e67a5-117">Некоторые генераторы объектной модели на стороне клиента анализируют WSDL и могут возникать из-за ошибки, потому что WSDL-файл не содержит определения службы WSDL.</span><span class="sxs-lookup"><span data-stu-id="e67a5-117">Some client-side object model generators parse the WSDL and can encounter an error condition because the WSDL file does not contain a WSDL service definition.</span></span> <span data-ttu-id="e67a5-118">Если генератор объектной модели обнаруживает ошибку, вы можете вставить заполнитель для определения службы WSDL.</span><span class="sxs-lookup"><span data-stu-id="e67a5-118">If your object model generator encounters an error, you can insert a placeholder WSDL service definition.</span></span>
  
> [!TIP]
> <span data-ttu-id="e67a5-119">Если вы используете .NET Framework для разработки приложения, мы рекомендуем использовать [управляемый API EWS](http://aka.ms/ews-managed-api-readme), а не генератор объектной модели.</span><span class="sxs-lookup"><span data-stu-id="e67a5-119">If you are using the .NET Framework to develop your application, we recommend that you use the [EWS Managed API](http://aka.ms/ews-managed-api-readme), rather than an object model generator.</span></span> <span data-ttu-id="e67a5-120">Управляемый API EWS предоставляет простую в использовании объектную модель для обработки сериализации и десериализации XML-кода EWS.</span><span class="sxs-lookup"><span data-stu-id="e67a5-120">The EWS Managed API provides an easy-to-use object model to handle the serialization and deserialization of the EWS XML.</span></span> <span data-ttu-id="e67a5-121">Дополнительные сведения см. в статье [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="e67a5-121">For more information, see [Get started with EWS Managed API client applications](https://msdn.microsoft.com/library/c2267733-6f4f-49e5-9614-1e4a24c3af1a%28Office.15%29.aspx).</span></span> 
  
<span data-ttu-id="e67a5-122">Файл схемы messages. XSD содержит определения элементов для элементов верхнего уровня в теле SOAP.</span><span class="sxs-lookup"><span data-stu-id="e67a5-122">The messages.xsd schema file contains the element definitions for the top-level elements in the SOAP body.</span></span> <span data-ttu-id="e67a5-123">За исключением кодов отклика об ошибках, большинство определений в messages. xsd характерны для операции.</span><span class="sxs-lookup"><span data-stu-id="e67a5-123">With the exception of the error response codes, most of the definitions in messages.xsd are specific to an operation.</span></span> <span data-ttu-id="e67a5-124">Схема Types. XSD содержит определения для заголовков SOAP и все общие определения, которые используются совместно несколькими операциями.</span><span class="sxs-lookup"><span data-stu-id="e67a5-124">The types.xsd schema contains the definitions for the SOAP headers and all the common definitions that are shared across operations.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e67a5-125">См. также</span><span class="sxs-lookup"><span data-stu-id="e67a5-125">See also</span></span>

- [<span data-ttu-id="e67a5-126">Справка по службам EWS для Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-126">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="e67a5-127">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-127">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
- [<span data-ttu-id="e67a5-128">Сведения об управляемом API EWS, EWS и веб-службах в Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-128">Explore the EWS Managed API, EWS, and web services in Exchange</span></span>](../exchange-web-services/explore-the-ews-managed-api-ews-and-web-services-in-exchange.md)
- [<span data-ttu-id="e67a5-129">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-129">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
- [<span data-ttu-id="e67a5-130">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="e67a5-130">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
    

