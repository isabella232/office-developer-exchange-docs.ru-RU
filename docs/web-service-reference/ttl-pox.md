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
description: Элемент TTL указывает время жизни (в часах), в течение которого параметры действительны.
ms.openlocfilehash: 5fecf3103553a82ed2aeeecfc1e4e1b9fe38583c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840245"
---
# <a name="ttl-pox"></a><span data-ttu-id="d940a-103">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-103">TTL (POX)</span></span>

<span data-ttu-id="d940a-104">Элемент **TTL** указывает время жизни (в часах), в течение которого параметры действительны.</span><span class="sxs-lookup"><span data-stu-id="d940a-104">The **TTL** element specifies the Time to Live, in hours, during which the settings remain valid.</span></span> 
  
[<span data-ttu-id="d940a-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d940a-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d940a-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d940a-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d940a-109">TTL (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-109">TTL (POX)</span></span>](ttl-pox.md)
  
```xml
<TTL/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d940a-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d940a-110">Attributes and elements</span></span>

<span data-ttu-id="d940a-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d940a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d940a-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d940a-112">Attributes</span></span>

<span data-ttu-id="d940a-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="d940a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d940a-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d940a-114">Child elements</span></span>

<span data-ttu-id="d940a-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="d940a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d940a-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d940a-116">Parent elements</span></span>

|<span data-ttu-id="d940a-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d940a-117">**Element**</span></span>|<span data-ttu-id="d940a-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d940a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d940a-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d940a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d940a-120">Содержит спецификации для подключения клиента к компьютеру Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d940a-120">Contains the specifications for connecting a client to the Exchange Server 2007 computer on which the Client Access server role is installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d940a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d940a-121">Text value</span></span>

<span data-ttu-id="d940a-122">Текстовое значение представляет срок жизни (в часах), в течение которого параметры оставались действительными.</span><span class="sxs-lookup"><span data-stu-id="d940a-122">The text value represents the Time to Live, in hours, during which the settings remain valid.</span></span> <span data-ttu-id="d940a-123">Нулевое значение указывает на то, что повторное обнаружение не является обязательным.</span><span class="sxs-lookup"><span data-stu-id="d940a-123">A value of zero indicates that rediscovery is not required.</span></span> <span data-ttu-id="d940a-124">Если значение не указано, по умолчанию для этого элемента используется значение 1 час.</span><span class="sxs-lookup"><span data-stu-id="d940a-124">If no value is specified, the default value for this element is 1 hour.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d940a-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="d940a-125">Remarks</span></span>

<span data-ttu-id="d940a-126">После истечения времени, представленного элементом **TTL** , необходимо повторно обнаружить параметры с помощью запроса на обнаружение.</span><span class="sxs-lookup"><span data-stu-id="d940a-126">After the time that is represented by the **TTL** element has elapsed, the settings should be rediscovered by using an Autodiscover request.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="d940a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="d940a-127">See also</span></span>



[<span data-ttu-id="d940a-128">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="d940a-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

