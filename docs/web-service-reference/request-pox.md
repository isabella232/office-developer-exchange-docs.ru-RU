---
title: Запрос (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: da54eb32-7ce5-4384-9893-255a2243a959
description: Элемент запрос содержит запрос к службе автообнаружения.
ms.openlocfilehash: ed6b0a80e83e160287f382a881dc5405bfb47a37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835124"
---
# <a name="request-pox"></a><span data-ttu-id="5f3cb-103">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-103">Request (POX)</span></span>

<span data-ttu-id="5f3cb-104">Элемент **запрос** содержит запрос к службе автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
[<span data-ttu-id="5f3cb-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="5f3cb-106">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="5f3cb-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="5f3cb-107">Attributes and elements</span></span>

<span data-ttu-id="5f3cb-108">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5f3cb-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="5f3cb-109">Attributes</span></span>

<span data-ttu-id="5f3cb-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5f3cb-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="5f3cb-111">Child elements</span></span>

|<span data-ttu-id="5f3cb-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5f3cb-112">**Element**</span></span>|<span data-ttu-id="5f3cb-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5f3cb-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f3cb-114">AcceptableResponseSchema (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="5f3cb-115">Определяет схему для ответа на службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="5f3cb-116">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="5f3cb-117">Указывает адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="5f3cb-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="5f3cb-119">Определяет, устаревшее различающееся имя почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5f3cb-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="5f3cb-120">Parent elements</span></span>

|<span data-ttu-id="5f3cb-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="5f3cb-121">**Element**</span></span>|<span data-ttu-id="5f3cb-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="5f3cb-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5f3cb-123">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="5f3cb-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="5f3cb-124">Корневой элемент в запросе службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="5f3cb-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5f3cb-125">См. также</span><span class="sxs-lookup"><span data-stu-id="5f3cb-125">See also</span></span>



[<span data-ttu-id="5f3cb-126">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="5f3cb-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

