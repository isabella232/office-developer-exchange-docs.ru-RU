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
description: Элемент Type определяет тип настроенной почтовой учетной записи.
ms.openlocfilehash: ad3570094ebe28498dfdc375cf7fc255434ba20d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465102"
---
# <a name="type-pox"></a><span data-ttu-id="d981b-103">Тип (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-103">Type (POX)</span></span>

<span data-ttu-id="d981b-104">Элемент **Type** определяет тип настроенной почтовой учетной записи.</span><span class="sxs-lookup"><span data-stu-id="d981b-104">The **Type** element identifies the type of the configured mail account.</span></span> 
  
[<span data-ttu-id="d981b-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d981b-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d981b-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d981b-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d981b-109">Тип (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-109">Type (POX)</span></span>](type-pox.md)
  
```XML
<Type>WEB or EXCH or EXPR or EXHTTP</Type>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d981b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d981b-110">Attributes and elements</span></span>

<span data-ttu-id="d981b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d981b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d981b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d981b-112">Attributes</span></span>

<span data-ttu-id="d981b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d981b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d981b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d981b-114">Child elements</span></span>

<span data-ttu-id="d981b-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d981b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d981b-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d981b-116">Parent elements</span></span>

|<span data-ttu-id="d981b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d981b-117">**Element**</span></span>|<span data-ttu-id="d981b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d981b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d981b-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d981b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d981b-120">Содержит спецификации для подключения клиента к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="d981b-120">Contains the specifications for connecting a client to the Exchange server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d981b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d981b-121">Text value</span></span>

<span data-ttu-id="d981b-122">Текстовое значение представляет тип учетной записи почты.</span><span class="sxs-lookup"><span data-stu-id="d981b-122">The text value represents the type of mail account.</span></span> <span data-ttu-id="d981b-123">В приведенной ниже таблице перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="d981b-123">The following table lists the possible values.</span></span>
  
|<span data-ttu-id="d981b-124">**Значение**</span><span class="sxs-lookup"><span data-stu-id="d981b-124">**Value**</span></span>|<span data-ttu-id="d981b-125">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d981b-125">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d981b-126">EXCH</span><span class="sxs-lookup"><span data-stu-id="d981b-126">EXCH</span></span>  <br/> |<span data-ttu-id="d981b-127">Протокол, используемый для подключения к серверу, — RPC RPC.</span><span class="sxs-lookup"><span data-stu-id="d981b-127">The protocol that is used to connect to the server is Exchange RPC.</span></span>  <br/> |
|<span data-ttu-id="d981b-128">ексхттп</span><span class="sxs-lookup"><span data-stu-id="d981b-128">EXHTTP</span></span>  <br/> |<span data-ttu-id="d981b-129">Протокол, используемый для подключения к серверу RPC/HTTP-подключениям.</span><span class="sxs-lookup"><span data-stu-id="d981b-129">The protocol that is used to connect to the server RPC/HTTP connections.</span></span>  <br/> |
|<span data-ttu-id="d981b-130">ВЫРАЖЕН</span><span class="sxs-lookup"><span data-stu-id="d981b-130">EXPR</span></span>  <br/> |<span data-ttu-id="d981b-131">Протокол, используемый для подключения к серверу, — это Exchange RPC через HTTP с использованием прокси-сервера RPC.</span><span class="sxs-lookup"><span data-stu-id="d981b-131">The protocol that is used to connect to the server is Exchange RPC over HTTP, using an RPC proxy server.</span></span>  <br/> <span data-ttu-id="d981b-132">Этот параметр применяется, только если для элемента [AccountType (POX)](accounttype-pox.md) задано значение email.</span><span class="sxs-lookup"><span data-stu-id="d981b-132">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
|<span data-ttu-id="d981b-133">WEB</span><span class="sxs-lookup"><span data-stu-id="d981b-133">WEB</span></span>  <br/> |<span data-ttu-id="d981b-134">Доступ к электронной почте осуществляется из веб-браузера с помощью URL-адреса, указанного в элементе [Server (POX)](server-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="d981b-134">E-mail is accessed from a Web browser by using the URL that is specified in the [Server (POX)](server-pox.md) element.</span></span>  <br/> <span data-ttu-id="d981b-135">Этот параметр применяется, только если для элемента [AccountType (POX)](accounttype-pox.md) задано значение email.</span><span class="sxs-lookup"><span data-stu-id="d981b-135">This is only applicable when the [AccountType (POX)](accounttype-pox.md) element is set to email.</span></span>  <br/> |
   
### <a name="version-differences"></a><span data-ttu-id="d981b-136">Различия версий</span><span class="sxs-lookup"><span data-stu-id="d981b-136">Version differences</span></span>

<span data-ttu-id="d981b-137">Office 365, Exchange Online и локальная версия Exchange, начиная с сборки 15.00.0995.014, возвращают значение "ЕКСХТТП" только в том случае, если сервер настроен на прием подключений RPC/HTTP, а клиент содержит заголовок [X-клиентканхандле](pox-autodiscover-request-for-exchange.md) , который содержит "ексхттпинфо".</span><span class="sxs-lookup"><span data-stu-id="d981b-137">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "EXHTTP" only if the server is configured to accept RPC/HTTP connections and the client includes an [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "ExHttpInfo".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d981b-138">См. также</span><span class="sxs-lookup"><span data-stu-id="d981b-138">See also</span></span>



[<span data-ttu-id="d981b-139">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="d981b-139">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

