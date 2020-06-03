---
title: Оваурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: Элемент Оваурл описывает URL-адрес и схему проверки подлинности, которая используется для доступа к определенному компьютеру под управлением Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.
ms.openlocfilehash: c0728af063cfbf1353eb7d3b81f5fcfe8b398f7d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457265"
---
# <a name="owaurl-pox"></a><span data-ttu-id="00ea1-103">Оваурл (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-103">OWAUrl (POX)</span></span>

<span data-ttu-id="00ea1-104">Элемент **оваурл** описывает URL-адрес и схему проверки подлинности, которая используется для доступа к определенному компьютеру под управлением Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="00ea1-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="00ea1-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="00ea1-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="00ea1-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="00ea1-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="00ea1-109">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="00ea1-110">Оваурл (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="00ea1-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="00ea1-111">Attributes and elements</span></span>

<span data-ttu-id="00ea1-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="00ea1-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00ea1-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="00ea1-113">Attributes</span></span>

|<span data-ttu-id="00ea1-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="00ea1-114">**Attribute**</span></span>|<span data-ttu-id="00ea1-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00ea1-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="00ea1-116">**Параметр authenticationmethod**</span><span class="sxs-lookup"><span data-stu-id="00ea1-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="00ea1-117">Описывает методы проверки подлинности для доступа к Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="00ea1-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="00ea1-118">Атрибут AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="00ea1-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="00ea1-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="00ea1-119">**Value**</span></span>|<span data-ttu-id="00ea1-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00ea1-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="00ea1-121">виндовсинтегратед</span><span class="sxs-lookup"><span data-stu-id="00ea1-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="00ea1-122">Встроенная проверка подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="00ea1-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="00ea1-123">FBA</span><span class="sxs-lookup"><span data-stu-id="00ea1-123">FBA</span></span>  <br/> |<span data-ttu-id="00ea1-124">Проверка подлинности на основе форм.</span><span class="sxs-lookup"><span data-stu-id="00ea1-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="00ea1-125">NTLM;</span><span class="sxs-lookup"><span data-stu-id="00ea1-125">NTLM</span></span>  <br/> |<span data-ttu-id="00ea1-126">Проверка подлинности NTLM.</span><span class="sxs-lookup"><span data-stu-id="00ea1-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="00ea1-127">Digest</span><span class="sxs-lookup"><span data-stu-id="00ea1-127">Digest</span></span>  <br/> |<span data-ttu-id="00ea1-128">Дайджест-проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="00ea1-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="00ea1-129">Базовая</span><span class="sxs-lookup"><span data-stu-id="00ea1-129">Basic</span></span>  <br/> |<span data-ttu-id="00ea1-130">Обычная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="00ea1-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="00ea1-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="00ea1-131">Child elements</span></span>

<span data-ttu-id="00ea1-132">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="00ea1-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00ea1-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="00ea1-133">Parent elements</span></span>

|<span data-ttu-id="00ea1-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="00ea1-134">**Element**</span></span>|<span data-ttu-id="00ea1-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00ea1-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00ea1-136">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="00ea1-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="00ea1-137">Содержит коллекцию URL-адресов Outlook Web Access, к которым клиент может подключаться, если он находится в брандмауэре.</span><span class="sxs-lookup"><span data-stu-id="00ea1-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00ea1-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="00ea1-138">Text value</span></span>

<span data-ttu-id="00ea1-139">Текстовое значение представляет URL-адрес службы Outlook Web Access на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="00ea1-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="00ea1-140">См. также</span><span class="sxs-lookup"><span data-stu-id="00ea1-140">See also</span></span>



[<span data-ttu-id="00ea1-141">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="00ea1-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

