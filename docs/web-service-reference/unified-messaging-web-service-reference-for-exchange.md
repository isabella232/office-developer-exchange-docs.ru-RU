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
ms.openlocfilehash: e4bb63f34650dae8fc28016196c97a6b79e69df0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467377"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="47e93-103">Справочные материалы по веб-службе единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="47e93-104">Найдите справочный контент для веб-службы единой системы обмена сообщениями в Exchange.</span><span class="sxs-lookup"><span data-stu-id="47e93-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="47e93-105">Веб-служба единой системы обмена сообщениями предоставляет точку расширения, которая позволяет клиентам считывать и изменять сведения о свойствах единой системы обмена сообщениями и запрашивать синтаксический анализ и диктовку элементов хранилища почтовых ящиков на телефонное устройство.</span><span class="sxs-lookup"><span data-stu-id="47e93-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="47e93-106">В этом разделе содержатся сведения об операциях и элементах, которые составляют XML-сообщения для веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="47e93-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="47e93-107">Этот контент применяется к URL-адресу конечной точки службы, аналогичному https:// \<yourclientaccessserver\> . com/EWS/UM2007Legacy. asmx.</span><span class="sxs-lookup"><span data-stu-id="47e93-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="47e93-108">Вы можете использовать службу автообнаружения, чтобы получить URL-адрес конечной точки веб-службы единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="47e93-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="47e93-109">Дополнительные сведения о службе автообнаружения содержатся в разделе Служба [автообнаружения для Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="47e93-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="47e93-110">Для версий Exchange, начинающихся с Exchange 2010, рекомендуется использовать операции единой системы обмена сообщениями, доступные в [веб-службах Exchange (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) , а не в веб-службе единой системы обмена сообщениями по следующим причинам:</span><span class="sxs-lookup"><span data-stu-id="47e93-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](https://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons:</span></span> 
> - <span data-ttu-id="47e93-111">Функции единой системы обмена сообщениями на основе EWS имеют поддержку первого класса в управляемом API EWS.</span><span class="sxs-lookup"><span data-stu-id="47e93-111">The EWS-based UM features have first-class support in the EWS Managed API.</span></span> 
> - <span data-ttu-id="47e93-112">В версиях Exchange, начиная с Exchange 2010, новые функции единой системы обмена сообщениями добавляются в веб-службу EWS, но не в единую систему обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="47e93-112">In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="47e93-113">Веб-служба единой системы обмена сообщениями не имеет явной схемы.</span><span class="sxs-lookup"><span data-stu-id="47e93-113">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="47e93-114">В этой статье</span><span class="sxs-lookup"><span data-stu-id="47e93-114">In this section</span></span>
<span data-ttu-id="47e93-115"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="47e93-115"><a name="bk_InThisSection"> </a></span></span>

- [<span data-ttu-id="47e93-116">Операции веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-116">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)   
- [<span data-ttu-id="47e93-117">XML-элементы веб-службы единой системы обмена сообщениями для Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-117">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="47e93-118">См. также</span><span class="sxs-lookup"><span data-stu-id="47e93-118">See also</span></span>

- [<span data-ttu-id="47e93-119">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-119">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="47e93-120">Автообнаружение в Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-120">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="47e93-121">Начало работы с веб-службами Exchange</span><span class="sxs-lookup"><span data-stu-id="47e93-121">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

