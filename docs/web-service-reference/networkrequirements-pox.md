---
title: Нетворкрекуирементс (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1555fd2e-05b6-4b94-907b-dae9174049d9
description: Элемент Нетворкрекуирементс содержит критерии, которые используются для определения того, находится ли клиентский компьютер в сети, удовлетворяющей требованиям поставщика услуг Интернета (ISP) для подключения к серверу.
ms.openlocfilehash: d588f7eb12a445fba9c997c4b9db0a6842105b4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462726"
---
# <a name="networkrequirements-pox"></a><span data-ttu-id="6ce3e-103">Нетворкрекуирементс (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-103">NetworkRequirements (POX)</span></span>

<span data-ttu-id="6ce3e-104">Элемент **нетворкрекуирементс** содержит критерии, которые используются для определения того, находится ли клиентский компьютер в сети, удовлетворяющей требованиям поставщика услуг Интернета (ISP) для подключения к серверу.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-104">The **NetworkRequirements** element contains the criteria that are used to determine whether the client computer is on a network that meets the requirements of the Internet service provider (ISP) to connect to the server.</span></span> 
  
[<span data-ttu-id="6ce3e-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="6ce3e-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="6ce3e-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="6ce3e-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="6ce3e-109">Нетворкрекуирементс (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-109">NetworkRequirements (POX)</span></span>](networkrequirements-pox.md)
  
```xml
<NetworkRequirements>
   <IPv4Start/>
   <IPv4End/>
   <IPv6Start/>
   <IPv6End/>
</NetworkRequirements>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="6ce3e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6ce3e-110">Attributes and elements</span></span>

<span data-ttu-id="6ce3e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ce3e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6ce3e-112">Attributes</span></span>

<span data-ttu-id="6ce3e-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ce3e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6ce3e-114">Child elements</span></span>

|<span data-ttu-id="6ce3e-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ce3e-115">**Element**</span></span>|<span data-ttu-id="6ce3e-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ce3e-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ce3e-117">IPv4Start (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-117">IPv4Start (POX)</span></span>](ipv4start-pox.md) <br/> |<span data-ttu-id="6ce3e-118">Указывает начало диапазона адресов IP версии 4 (IPv4), которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-118">Identifies the start of a range of IP version 4 (IPv4) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="6ce3e-119">IPv4End (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-119">IPv4End (POX)</span></span>](ipv4end-pox.md) <br/> |<span data-ttu-id="6ce3e-120">Определяет конец диапазона адресов IP версии 4 (IPv4), которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-120">Identifies the end of a range of IP version 4 (IPv4) addresses that are used to identify a computer on the network.</span></span>  <br/> |
|[<span data-ttu-id="6ce3e-121">IPv6Start (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-121">IPv6Start (POX)</span></span>](ipv6start-pox.md) <br/> |<span data-ttu-id="6ce3e-122">Указывает начало диапазона адресов IP версии 6 (IPv6), которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-122">Identifies the start of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
|[<span data-ttu-id="6ce3e-123">IPv6End (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-123">IPv6End (POX)</span></span>](ipv6end-pox.md) <br/> |<span data-ttu-id="6ce3e-124">Определяет конец диапазона адресов IP версии 6 (IPv6), которые используются для идентификации компьютера в сети.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-124">Identifies the end of a range of IP version 6 (IPv6) addresses that are used to identify a computer on a network.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ce3e-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6ce3e-125">Parent elements</span></span>

|<span data-ttu-id="6ce3e-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6ce3e-126">**Element**</span></span>|<span data-ttu-id="6ce3e-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6ce3e-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ce3e-128">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="6ce3e-128">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="6ce3e-129">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-129">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6ce3e-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="6ce3e-130">Remarks</span></span>

<span data-ttu-id="6ce3e-131">Если клиент электронной почты не отвечает требованиям сети, он должен использовать другие типы протокола.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-131">If the e-mail client does not match the network requirements, it should try other protocol types.</span></span> <span data-ttu-id="6ce3e-132">Поставщики услуг Интернета могут предоставлять один набор серверов с тегами [Protocol (POX)](protocol-pox.md) , которые не требуют проверки подлинности, но должны находиться в сети ISP.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-132">ISPs may provide one set of servers with [Protocol (POX)](protocol-pox.md) tags that do not require authentication but are required to be on the ISP network.</span></span> <span data-ttu-id="6ce3e-133">Поставщики услуг Интернета могут перечислить еще один набор серверов, требующих проверки подлинности, но не требующихся в конкретной сети.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-133">ISPs may list another set of servers that require authentication but are not required to be on a specific network.</span></span> 
  
<span data-ttu-id="6ce3e-134">Элемент **нетворкрекуирементс** является необязательным.</span><span class="sxs-lookup"><span data-stu-id="6ce3e-134">The **NetworkRequirements** element is optional.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="6ce3e-135">См. также</span><span class="sxs-lookup"><span data-stu-id="6ce3e-135">See also</span></span>



[<span data-ttu-id="6ce3e-136">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="6ce3e-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

