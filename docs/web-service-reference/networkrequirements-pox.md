---
title: NetworkRequirements (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: Элемент NetworkRequirements содержит критерии, используемые для определения, является ли на клиентском компьютере в сети, которая соответствует требованиям поставщика услуг Интернета (поставщика услуг Интернета) для подключения к серверу.
ms.openlocfilehash: f3abcff04cd4121b8dcc7ceff7658ad389e6d0b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834529"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="6c563-103">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="6c563-104">Элемент **NetworkRequirements** содержит критерии, используемые для определения, является ли на клиентском компьютере в сети, которая соответствует требованиям поставщика услуг Интернета (поставщика услуг Интернета) для подключения к серверу.</span><span class="sxs-lookup"><span data-stu-id="6c563-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="6c563-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6c563-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6c563-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6c563-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6c563-109">NetworkRequirements (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6c563-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6c563-110">Attributes and elements</span></span>

<span data-ttu-id="6c563-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6c563-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6c563-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6c563-112">Attributes</span></span>

<span data-ttu-id="6c563-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6c563-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6c563-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6c563-114">Child elements</span></span>

|<span data-ttu-id="6c563-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6c563-115">**Element**</span></span>|<span data-ttu-id="6c563-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c563-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c563-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="6c563-118">Определяет начало диапазона IP версии 4 (IPv4) адреса, которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6c563-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="6c563-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="6c563-120">Определяет конец диапазона IP версии 4 (IPv4) адреса, которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6c563-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="6c563-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="6c563-122">Определяет начало диапазона IP-адресов версии 6 (IPv6) адреса, которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6c563-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="6c563-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="6c563-124">Определяет конец диапазона IP-адресов версии 6 (IPv6) адреса, которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6c563-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6c563-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6c563-125">Parent elements</span></span>

|<span data-ttu-id="6c563-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6c563-126">**Element**</span></span>|<span data-ttu-id="6c563-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6c563-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6c563-128">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="6c563-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6c563-129">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6c563-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6c563-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="6c563-130">Remarks</span></span>

<span data-ttu-id="6c563-131">Если клиентом электронной почты не соответствует требованиям сети, его следует попробуйте других типов протокола.</span><span class="sxs-lookup"><span data-stu-id="6c563-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="6c563-132">Поставщики услуг Интернета можно указать один набор серверов с тегами [Протокола (POX)](protocol-pox.md) , которые не требуют проверки подлинности, но требуется быть в сети поставщика услуг Интернета.</span><span class="sxs-lookup"><span data-stu-id="6c563-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="6c563-133">Поставщики услуг Интернета могут списки другой набор серверов, которые требуют проверки подлинности, но не обязательно должны быть в конкретной сети.</span><span class="sxs-lookup"><span data-stu-id="6c563-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="6c563-134">Элемент **NetworkRequirements** является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6c563-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6c563-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6c563-135">See also</span></span>



[<span data-ttu-id="6c563-136">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="6c563-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

