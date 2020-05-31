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
ms.openlocfilehash: 3f5d5258a92840fe79c4936370323b78aa4715b3
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354430"
---
# <a name="request-pox"></a><span data-ttu-id="71401-103">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-103">Request (POX)</span></span>

<span data-ttu-id="71401-104">Элемент **request** содержит запрос к службе автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="71401-104">The **Request** element contains the request to the Autodiscover service.</span></span> 
  
- [<span data-ttu-id="71401-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="71401-106">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-106">Request (POX)</span></span>](request-pox.md)
  
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

## <a name="attributes-and-elements"></a><span data-ttu-id="71401-107">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71401-107">Attributes and elements</span></span>

<span data-ttu-id="71401-108">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71401-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71401-109">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71401-109">Attributes</span></span>

<span data-ttu-id="71401-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="71401-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71401-111">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71401-111">Child elements</span></span>

|<span data-ttu-id="71401-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71401-112">**Element**</span></span>|<span data-ttu-id="71401-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71401-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71401-114">Акцептаблереспонсесчема (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-114">AcceptableResponseSchema (POX)</span></span>](acceptableresponseschema-pox.md) <br/> |<span data-ttu-id="71401-115">Определяет схему ответа автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="71401-115">Identifies the schema for an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="71401-116">EmailAddress (Нонемптистрингтипе)</span><span class="sxs-lookup"><span data-stu-id="71401-116">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="71401-117">Определяет адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="71401-117">Identifies the user's e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="71401-118">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-118">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="71401-119">Определяет почтовый ящик пользователя, используя устаревшее различающееся имя.</span><span class="sxs-lookup"><span data-stu-id="71401-119">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="71401-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71401-120">Parent elements</span></span>

|<span data-ttu-id="71401-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71401-121">**Element**</span></span>|<span data-ttu-id="71401-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71401-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71401-123">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="71401-123">AutoDiscover (POX)</span></span>](autodiscover-pox.md) <br/> |<span data-ttu-id="71401-124">Корневой элемент запроса на обнаружение.</span><span class="sxs-lookup"><span data-stu-id="71401-124">The root element in an Autodiscover request.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="71401-125">См. также</span><span class="sxs-lookup"><span data-stu-id="71401-125">See also</span></span>

- [<span data-ttu-id="71401-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="71401-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

