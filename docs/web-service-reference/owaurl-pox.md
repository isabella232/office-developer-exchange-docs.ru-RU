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
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834673"
---
# <a name="owaurl-pox"></a><span data-ttu-id="a0890-103">Оваурл (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-103">OWAUrl (POX)</span></span>

<span data-ttu-id="a0890-104">Элемент **оваурл** описывает URL-адрес и схему проверки подлинности, которая используется для доступа к определенному компьютеру под управлением Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="a0890-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="a0890-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a0890-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a0890-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a0890-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a0890-109">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="a0890-110">Оваурл (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a0890-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a0890-111">Attributes and elements</span></span>

<span data-ttu-id="a0890-112">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a0890-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0890-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a0890-113">Attributes</span></span>

|<span data-ttu-id="a0890-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="a0890-114">**Attribute**</span></span>|<span data-ttu-id="a0890-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0890-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0890-116">**Параметр authenticationmethod**</span><span class="sxs-lookup"><span data-stu-id="a0890-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="a0890-117">Описывает методы проверки подлинности для доступа к Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="a0890-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="a0890-118">Атрибут AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="a0890-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="a0890-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="a0890-119">**Value**</span></span>|<span data-ttu-id="a0890-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0890-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a0890-121">виндовсинтегратед</span><span class="sxs-lookup"><span data-stu-id="a0890-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="a0890-122">Встроенная проверка подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="a0890-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="a0890-123">FBA</span><span class="sxs-lookup"><span data-stu-id="a0890-123">FBA</span></span>  <br/> |<span data-ttu-id="a0890-124">Проверка подлинности на основе форм.</span><span class="sxs-lookup"><span data-stu-id="a0890-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="a0890-125">NTLM;</span><span class="sxs-lookup"><span data-stu-id="a0890-125">NTLM</span></span>  <br/> |<span data-ttu-id="a0890-126">Проверка подлинности NTLM.</span><span class="sxs-lookup"><span data-stu-id="a0890-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="a0890-127">Digest</span><span class="sxs-lookup"><span data-stu-id="a0890-127">Digest</span></span>  <br/> |<span data-ttu-id="a0890-128">Дайджест-проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="a0890-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="a0890-129">Базовая</span><span class="sxs-lookup"><span data-stu-id="a0890-129">Basic</span></span>  <br/> |<span data-ttu-id="a0890-130">Обычная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="a0890-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="a0890-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a0890-131">Child elements</span></span>

<span data-ttu-id="a0890-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="a0890-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0890-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a0890-133">Parent elements</span></span>

|<span data-ttu-id="a0890-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0890-134">**Element**</span></span>|<span data-ttu-id="a0890-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0890-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0890-136">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="a0890-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="a0890-137">Содержит коллекцию URL-адресов Outlook Web Access, к которым клиент может подключаться, если он находится в брандмауэре.</span><span class="sxs-lookup"><span data-stu-id="a0890-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0890-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a0890-138">Text value</span></span>

<span data-ttu-id="a0890-139">Текстовое значение представляет URL-адрес службы Outlook Web Access на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a0890-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a0890-140">См. также</span><span class="sxs-lookup"><span data-stu-id="a0890-140">See also</span></span>



[<span data-ttu-id="a0890-141">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a0890-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

