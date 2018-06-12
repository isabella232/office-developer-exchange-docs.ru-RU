---
title: TTL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 178eefa1-995c-4bea-930b-e51293961191
description: Элемент TTL указывает срок жизни, в часах, во время которых параметры остаются действительными.
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840245"
---
# <a name="ttl-pox"></a><span data-ttu-id="2a305-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-103">TTL (POX)</span></span>

<span data-ttu-id="2a305-104">Элемент **TTL** Указывает срок жизни, в часах, во время которых параметры остаются действительными.</span><span class="sxs-lookup"><span data-stu-id="2a305-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="2a305-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="2a305-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="2a305-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="2a305-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="2a305-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2a305-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2a305-110">Attributes and elements</span></span>

<span data-ttu-id="2a305-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="2a305-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a305-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2a305-112">Attributes</span></span>

<span data-ttu-id="2a305-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="2a305-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a305-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2a305-114">Child elements</span></span>

<span data-ttu-id="2a305-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="2a305-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a305-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2a305-116">Parent elements</span></span>

|<span data-ttu-id="2a305-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2a305-117">**Element**</span></span>|<span data-ttu-id="2a305-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2a305-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a305-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="2a305-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="2a305-120">Содержит спецификации для подключения клиента Exchange Server 2007 компьютеру, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="2a305-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a305-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2a305-121">Text value</span></span>

<span data-ttu-id="2a305-122">Текстовое значение представляет время жизни, в часах, во время которых параметры остаются действительными.</span><span class="sxs-lookup"><span data-stu-id="2a305-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="2a305-123">Нулевое значение указывает, что не требуется, что поиск контроллеров домена.</span><span class="sxs-lookup"><span data-stu-id="2a305-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="2a305-124">Если значение не указано, значение по умолчанию для этого элемента — 1 час.</span><span class="sxs-lookup"><span data-stu-id="2a305-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2a305-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="2a305-125">Remarks</span></span>

<span data-ttu-id="2a305-126">По истечении времени, которая представляется элемент **TTL** обнаружить параметры необходимо повторно с помощью запроса службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2a305-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2a305-127">См. также</span><span class="sxs-lookup"><span data-stu-id="2a305-127">See also</span></span>



[<span data-ttu-id="2a305-128">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2a305-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

