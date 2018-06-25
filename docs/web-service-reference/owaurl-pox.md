---
title: OWAUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 450b86a1-1722-49f5-b541-16c1edc3db7a
description: Элемент OWAUrl описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.
ms.openlocfilehash: 93d03506e2a74aa1b4ef6d2a49ccbda01cfc1f9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834673"
---
# <a name="owaurl-pox"></a><span data-ttu-id="8af60-103">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-103">OWAUrl (POX)</span></span>

<span data-ttu-id="8af60-104">Элемент **OWAUrl** описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.</span><span class="sxs-lookup"><span data-stu-id="8af60-104">The **OWAUrl** element describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that hosts Outlook Web Access.</span></span> 
  
[<span data-ttu-id="8af60-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8af60-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8af60-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8af60-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8af60-109">Внутренний (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-109">Internal (POX)</span></span>](internal-pox.md)
  
[<span data-ttu-id="8af60-110">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-110">OWAUrl (POX)</span></span>](owaurl-pox.md)
  
```xml
<OWAUrl AuthenticationMethod=""/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8af60-111">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8af60-111">Attributes and elements</span></span>

<span data-ttu-id="8af60-112">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8af60-112">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8af60-113">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8af60-113">Attributes</span></span>

|<span data-ttu-id="8af60-114">**Атрибут**</span><span class="sxs-lookup"><span data-stu-id="8af60-114">**Attribute**</span></span>|<span data-ttu-id="8af60-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8af60-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8af60-116">**AuthenticationMethod**</span><span class="sxs-lookup"><span data-stu-id="8af60-116">**AuthenticationMethod**</span></span> <br/> |<span data-ttu-id="8af60-117">Описываются методы проверки подлинности для доступа к Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="8af60-117">Describes the authentication methods for accessing Outlook Web Access.</span></span>  <br/> |
   
#### <a name="authenticationmethod-attribute"></a><span data-ttu-id="8af60-118">Атрибут AuthenticationMethod</span><span class="sxs-lookup"><span data-stu-id="8af60-118">AuthenticationMethod Attribute</span></span>

|<span data-ttu-id="8af60-119">**Значение**</span><span class="sxs-lookup"><span data-stu-id="8af60-119">**Value**</span></span>|<span data-ttu-id="8af60-120">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8af60-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8af60-121">WindowsIntegrated</span><span class="sxs-lookup"><span data-stu-id="8af60-121">WindowsIntegrated</span></span>  <br/> |<span data-ttu-id="8af60-122">Встроенная проверка подлинности Windows.</span><span class="sxs-lookup"><span data-stu-id="8af60-122">Integrated Windows authentication.</span></span>  <br/> |
|<span data-ttu-id="8af60-123">FBA</span><span class="sxs-lookup"><span data-stu-id="8af60-123">FBA</span></span>  <br/> |<span data-ttu-id="8af60-124">Проверка подлинности на основе форм.</span><span class="sxs-lookup"><span data-stu-id="8af60-124">Forms-based authentication.</span></span>  <br/> |
|<span data-ttu-id="8af60-125">NTLM</span><span class="sxs-lookup"><span data-stu-id="8af60-125">NTLM</span></span>  <br/> |<span data-ttu-id="8af60-126">Проверка подлинности NTLM.</span><span class="sxs-lookup"><span data-stu-id="8af60-126">NTLM authentication.</span></span>  <br/> |
|<span data-ttu-id="8af60-127">Дайджест-проверка</span><span class="sxs-lookup"><span data-stu-id="8af60-127">Digest</span></span>  <br/> |<span data-ttu-id="8af60-128">Дайджест-проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="8af60-128">Digest authentication.</span></span>  <br/> |
|<span data-ttu-id="8af60-129">Общая</span><span class="sxs-lookup"><span data-stu-id="8af60-129">Basic</span></span>  <br/> |<span data-ttu-id="8af60-130">Обычная проверка подлинности.</span><span class="sxs-lookup"><span data-stu-id="8af60-130">Basic authentication.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8af60-131">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8af60-131">Child elements</span></span>

<span data-ttu-id="8af60-132">Нет.</span><span class="sxs-lookup"><span data-stu-id="8af60-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8af60-133">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8af60-133">Parent elements</span></span>

|<span data-ttu-id="8af60-134">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8af60-134">**Element**</span></span>|<span data-ttu-id="8af60-135">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8af60-135">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8af60-136">Внутренний (POX)</span><span class="sxs-lookup"><span data-stu-id="8af60-136">Internal (POX)</span></span>](internal-pox.md) <br/> |<span data-ttu-id="8af60-137">Содержит коллекцию Outlook Web Access URL-адреса, клиент может подключиться к, когда в сети брандмауэра.</span><span class="sxs-lookup"><span data-stu-id="8af60-137">Contains the collection of Outlook Web Access URLs that a client can connect to when it is inside the firewall.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8af60-138">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8af60-138">Text value</span></span>

<span data-ttu-id="8af60-139">Текстовое значение представляет URL-адрес для службы Outlook Web Access на сервере клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8af60-139">The text value represents the URL for the Outlook Web Access service on a Client Access server.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8af60-140">См. также</span><span class="sxs-lookup"><span data-stu-id="8af60-140">See also</span></span>



[<span data-ttu-id="8af60-141">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="8af60-141">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

