---
title: Единой системы обмена сообщениями веб-службы ссылки для Exchange
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
description: Найдите справочные статьи для веб-службы единой системы обмена сообщениями (UM) в Exchange.
ms.openlocfilehash: 12ee91c5a8b7e1ba23b937f142a9ae2835697fef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840268"
---
# <a name="unified-messaging-web-service-reference-for-exchange"></a><span data-ttu-id="b51e9-103">Единой системы обмена сообщениями веб-службы ссылки для Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-103">Unified Messaging web service reference for Exchange</span></span>

<span data-ttu-id="b51e9-104">Найдите справочные статьи для веб-службы единой системы обмена сообщениями (UM) в Exchange.</span><span class="sxs-lookup"><span data-stu-id="b51e9-104">Find reference content for the Unified Messaging (UM) web service in Exchange.</span></span>
  
<span data-ttu-id="b51e9-105">Веб-служба единой системы обмена сообщениями (UM) предоставляет точку расширения, которая позволяет клиентам читать и изменять сведения о свойствах единой системы обмена СООБЩЕНИЯМИ и попросите синтаксический анализ и настройке через телефонное устройство элементы хранилища почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="b51e9-105">The Unified Messaging (UM) web service provides an extensibility point that enables clients to read and change information about UM properties and request that mailbox store items be parsed and dictated over a telephony device.</span></span> <span data-ttu-id="b51e9-106">В этом разделе содержатся сведения о работе и элементов, составляющих XML-сообщения для веб-службы единой системы обмена СООБЩЕНИЯМИ.</span><span class="sxs-lookup"><span data-stu-id="b51e9-106">This section contains information about the operations and elements that make up the XML messages for the UM web service.</span></span> <span data-ttu-id="b51e9-107">Этот контент применяется к URL-адрес конечной точки службы, похожие на https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span><span class="sxs-lookup"><span data-stu-id="b51e9-107">This content applies to the service endpoint URL that is similar to https://\<yourclientaccessserver\>.com/EWS/UM2007Legacy.asmx.</span></span> 
  
<span data-ttu-id="b51e9-108">Можно использовать службу автообнаружения для получения URL-адрес конечной веб-службы единой системы обмена СООБЩЕНИЯМИ.</span><span class="sxs-lookup"><span data-stu-id="b51e9-108">You can use the Autodiscover service to get the URL to the UM web service endpoint.</span></span> <span data-ttu-id="b51e9-109">Дополнительные сведения о автообнаружения можно [автообнаружения для Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span><span class="sxs-lookup"><span data-stu-id="b51e9-109">For more information about Autodiscover, see [Autodiscover for Exchange](../exchange-web-services/autodiscover-for-exchange.md).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="b51e9-110">Для версий Exchange, начиная с Exchange 2010, мы рекомендуем использовать операций единой системы обмена сообщениями, доступные в [Веб-служб Exchange (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) вместо веб-службы единой системы обмена СООБЩЕНИЯМИ по следующим причинам: > иметь возможности единой системы обмена СООБЩЕНИЯМИ на основе веб-служб Exchange поддержку в управляемый API веб-служб Exchange.</span><span class="sxs-lookup"><span data-stu-id="b51e9-110">For versions of Exchange starting with Exchange 2010, we recommend that you use the Unified Messaging operations that are available in [Exchange Web Services (EWS)](http://msdn.microsoft.com/library/60285497-0c4e-4e51-84e1-34dd6d89a5d8%28Office.15%29.aspx) instead of the UM web service, for the following reasons: >  The EWS-based UM features have first-class support in the EWS Managed API.</span></span> <span data-ttu-id="b51e9-111">> В версиях Exchange, начиная с Exchange 2010 новые возможности единой системы обмена СООБЩЕНИЯМИ будут добавлены к веб-служб Exchange, но не к веб-службе единой системы обмена сообщениями.</span><span class="sxs-lookup"><span data-stu-id="b51e9-111">>  In versions of Exchange starting with Exchange 2010, new UM features are added to EWS but not to the Unified Messaging web service.</span></span> 
  
<span data-ttu-id="b51e9-112">Веб-службы единой системы обмена СООБЩЕНИЯМИ не имеет явных схемы.</span><span class="sxs-lookup"><span data-stu-id="b51e9-112">The UM web service does not have an explicit schema.</span></span>
  
## <a name="in-this-section"></a><span data-ttu-id="b51e9-113">В этом разделе</span><span class="sxs-lookup"><span data-stu-id="b51e9-113">In this section</span></span>
<span data-ttu-id="b51e9-114"><a name="bk_InThisSection"> </a></span><span class="sxs-lookup"><span data-stu-id="b51e9-114"></span></span>

- [<span data-ttu-id="b51e9-115">Операции единой системы обмена сообщениями веб-службы для Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-115">Unified Messaging web service operations for Exchange</span></span>](unified-messaging-web-service-operations-for-exchange.md)
    
- [<span data-ttu-id="b51e9-116">Единой системы обмена сообщениями веб-службы XML элементов для Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-116">Unified Messaging web service XML elements for Exchange</span></span>](unified-messaging-web-service-xml-elements-for-exchange.md)
    
## <a name="see-also"></a><span data-ttu-id="b51e9-117">См. также</span><span class="sxs-lookup"><span data-stu-id="b51e9-117">See also</span></span>

- [<span data-ttu-id="b51e9-118">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-118">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
- [<span data-ttu-id="b51e9-119">Автообнаружение для Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-119">Autodiscover for Exchange</span></span>](../exchange-web-services/autodiscover-for-exchange.md)
- [<span data-ttu-id="b51e9-120">Начать работу с использованием веб-служб Exchange</span><span class="sxs-lookup"><span data-stu-id="b51e9-120">Start using web services in Exchange</span></span>](../exchange-web-services/start-using-web-services-in-exchange.md)
    

