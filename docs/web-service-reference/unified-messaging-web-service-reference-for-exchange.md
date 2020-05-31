---
title: Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_name:
- Unified
api_type:
- schema
ms.assetid: 83afea8a-c716-41df-9eb2-e1000357afb6
description: Найдите справочный контент для веб-службы единой системы обмена сообщениями в Exchange.
ms.openlocfilehash: 9e124f504ecee517edc51610696f06729904d75f
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354276"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="e2560-103">Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="e2560-104">Найдите справочный контент для веб-службы единой системы обмена сообщениями в Exchange.</span><span class="sxs-lookup"><span data-stu-id="e2560-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="e2560-105">Веб-служба единой системы обмена сообщениями предоставляет точку расширения, которая позволяет клиентам считывать и изменять сведения о свойствах единой системы обмена сообщениями и запрашивать синтаксический анализ и диктовку элементов хранилища почтовых ящиков на телефонное устройство.</span><span class="sxs-lookup"><span data-stu-id="e2560-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="e2560-106">В этом разделе содержатся сведения об операциях и элементах, которые составляют XML-сообщения для веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="e2560-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="e2560-107">Этот контент применяется к URL-адресу конечной точки службы,\<аналогичному\>HTTPS://ЙОУРКЛИЕНТАКЦЕСССЕРВЕР. com/EWS/UM2007Legacy. asmx.</span><span class="sxs-lookup"><span data-stu-id="e2560-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="e2560-108">Вы можете использовать службу автообнаружения, чтобы получить URL-адрес конечной точки веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="e2560-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="e2560-109">Дополнительные сведения о службе автообнаружения содержатся в разделе Служба [автообнаружения для Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="e2560-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="e2560-110">Для версий Exchange, начинающихся с Exchange 2010, рекомендуется использовать операции единой системы обмена сообщениями, доступные в [веб-службах Exchange (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) , а не в веб-службе единой системы обмена сообщениями по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="e2560-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="e2560-111">Функции единой системы обмена сообщениями на основе EWS имеют поддержку первого класса в управляемом API EWS.</span><span class="sxs-lookup"><span data-stu-id="e2560-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="e2560-112">В версиях Exchange, начиная с Exchange 2010, новые функции единой системы обмена сообщениями добавляются в веб-службу EWS, но не в единую систему обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="e2560-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="e2560-113">Веб-служба единой системы обмена сообщениями не имеет явной схемы.</span><span class="sxs-lookup"><span data-stu-id="e2560-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="e2560-114">В этом разделе:</span><span class="sxs-lookup"><span data-stu-id="e2560-114">In this section</span></span>
<span data-ttu-id="e2560-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="e2560-115"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="e2560-116">Операции веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="e2560-117">XML-элементы веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="e2560-118">См. также</span><span class="sxs-lookup"><span data-stu-id="e2560-118">See also</span></span>

- [<span data-ttu-id="e2560-119">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="e2560-120">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="e2560-121">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="e2560-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

