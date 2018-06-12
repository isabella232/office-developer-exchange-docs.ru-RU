---
title: Тип (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9a627244-554f-4223-b9d8-a601b81a4a1a
description: Элемент Type определяет тип учетной записи электронной почты настроена.
ms.openlocfilehash: 6e1349769c6a5349304f576419e0c609d3edd9a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840247"
---
# <a name="type-pox"></a><span data-ttu-id="70212-103">Тип (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-103">Type (POX)</span></span>

<span data-ttu-id="70212-104">Элемент **Type** определяет тип учетной записи электронной почты настроена.</span><span class="sxs-lookup"><span data-stu-id="70212-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="70212-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="70212-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="70212-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="70212-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="70212-109">Тип (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="70212-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="70212-110">Attributes and elements</span></span>

<span data-ttu-id="70212-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="70212-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70212-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="70212-112">Attributes</span></span>

<span data-ttu-id="70212-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="70212-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70212-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="70212-114">Child elements</span></span>

<span data-ttu-id="70212-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="70212-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70212-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="70212-116">Parent elements</span></span>

|<span data-ttu-id="70212-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="70212-117">**Element**</span></span>|<span data-ttu-id="70212-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70212-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70212-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="70212-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="70212-120">Содержит спецификации для подключения клиента к серверу Exchange.</span><span class="sxs-lookup"><span data-stu-id="70212-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70212-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="70212-121">Text value</span></span>

<span data-ttu-id="70212-122">Текстовое значение представляет тип учетной записи почты.</span><span class="sxs-lookup"><span data-stu-id="70212-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="70212-123">В следующей таблице приведены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="70212-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="70212-124">**Значение**</span><span class="sxs-lookup"><span data-stu-id="70212-124">**Value**</span></span>|<span data-ttu-id="70212-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="70212-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70212-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="70212-126">EXCH</span></span>  <br/> |<span data-ttu-id="70212-127">Протокол, используемый для подключения к серверу используется Exchange RPC.</span><span class="sxs-lookup"><span data-stu-id="70212-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="70212-128">EXHTTP</span><span class="sxs-lookup"><span data-stu-id="70212-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="70212-129">Протокол, используемый для подключения RPC/HTTP-подключений сервера.</span><span class="sxs-lookup"><span data-stu-id="70212-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="70212-130">ВЫРАЖЕНИЕ</span><span class="sxs-lookup"><span data-stu-id="70212-130">EXPR</span></span>  <br/> |<span data-ttu-id="70212-131">Протокол, используемый для подключения к серверу — Exchange RPC через HTTP, прокси-сервер RPC.</span><span class="sxs-lookup"><span data-stu-id="70212-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="70212-132">Это применимо только если для элемента [AccountType (POX)](accounttype-pox.md) в электронной почты.</span><span class="sxs-lookup"><span data-stu-id="70212-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="70212-133">WEB</span><span class="sxs-lookup"><span data-stu-id="70212-133">WEB</span></span>  <br/> |<span data-ttu-id="70212-134">Для доступа к электронной почты из веб-браузера с помощью URL-адреса, указанного в элементе [Сервера (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="70212-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="70212-135">Это применимо только если для элемента [AccountType (POX)](accounttype-pox.md) в электронной почты.</span><span class="sxs-lookup"><span data-stu-id="70212-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="70212-136">Различия версий</span><span class="sxs-lookup"><span data-stu-id="70212-136">Version differences</span></span>

<span data-ttu-id="70212-137">Office 365, Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014 возвращаемое значение «EXHTTP» только в том случае, если сервер настроен на прием RPC/HTTP-подключений и клиент включает в себя заголовок [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) , содержит «ExHttpInfo».</span><span class="sxs-lookup"><span data-stu-id="70212-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="70212-138">См. также</span><span class="sxs-lookup"><span data-stu-id="70212-138">See also</span></span>



[<span data-ttu-id="70212-139">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="70212-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

