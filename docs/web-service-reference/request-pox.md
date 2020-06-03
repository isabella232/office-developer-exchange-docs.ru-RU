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
description: Элемент Request содержит запрос к службе автообнаружения.
ms.openlocfilehash: bc215d614441ed8f12c0f1490f4abdbb7b574ad0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459548"
---
# <a name="request-pox"></a><span data-ttu-id="fc10e-103">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-103">Request (POX)</span></span>

<span data-ttu-id="fc10e-104">Элемент **request** содержит запрос к службе автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="fc10e-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="fc10e-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="fc10e-106">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-106">Request (POX)</span></span>](request-pox.md)
  
```xml
<Request>
   <AcceptableResponseSchema/>
   <EMailAddress/>
</Request>
```

```xml
<Request>
   <AcceptableResponseSchema/> 
   <LegacyDN/>
</Request>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="fc10e-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fc10e-107">Attributes and elements</span></span>

<span data-ttu-id="fc10e-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="fc10e-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fc10e-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fc10e-109">Attributes</span></span>

<span data-ttu-id="fc10e-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="fc10e-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fc10e-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fc10e-111">Child elements</span></span>

|<span data-ttu-id="fc10e-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc10e-112">**Element**</span></span>|<span data-ttu-id="fc10e-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc10e-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc10e-114">Акцептаблереспонсесчема (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="fc10e-115">Определяет схему ответа автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="fc10e-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="fc10e-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="fc10e-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="fc10e-117">Определяет адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="fc10e-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="fc10e-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="fc10e-119">Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.</span><span class="sxs-lookup"><span data-stu-id="fc10e-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fc10e-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fc10e-120">Parent elements</span></span>

|<span data-ttu-id="fc10e-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fc10e-121">**Element**</span></span>|<span data-ttu-id="fc10e-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fc10e-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fc10e-123">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="fc10e-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="fc10e-124">Корневой элемент запроса на обнаружение.</span><span class="sxs-lookup"><span data-stu-id="fc10e-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fc10e-125">См. также</span><span class="sxs-lookup"><span data-stu-id="fc10e-125">See also</span></span>

- [<span data-ttu-id="fc10e-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="fc10e-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

