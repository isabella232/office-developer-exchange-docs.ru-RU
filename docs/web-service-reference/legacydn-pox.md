---
title: LegacyDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 9fb9529f-52c5-4907-a84b-935b78de16c3
description: Элемент LegacyDN определяет почтовый ящик пользователя по устаревшему различающеу имени.
ms.openlocfilehash: f7ec1dea29a7d3ad6d470ef7812390d179fe1d2a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834243"
---
# <a name="legacydn-pox"></a><span data-ttu-id="2b26f-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="2b26f-103">LegacyDN (POX)</span></span>

<span data-ttu-id="2b26f-104">Элемент **LegacyDN** определяет почтовый ящик пользователя по устаревшему различающеу имени.</span><span class="sxs-lookup"><span data-stu-id="2b26f-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="2b26f-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="2b26f-105">Attributes and elements</span></span>

<span data-ttu-id="2b26f-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="2b26f-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b26f-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="2b26f-107">Attributes</span></span>

<span data-ttu-id="2b26f-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b26f-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b26f-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="2b26f-109">Child elements</span></span>

<span data-ttu-id="2b26f-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="2b26f-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b26f-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="2b26f-111">Parent elements</span></span>

|<span data-ttu-id="2b26f-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="2b26f-112">**Element**</span></span>|<span data-ttu-id="2b26f-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="2b26f-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b26f-114">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="2b26f-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="2b26f-115">Содержит запрос к службе автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2b26f-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="2b26f-116">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="2b26f-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="2b26f-117">Предоставляет сведения, относящиеся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="2b26f-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2b26f-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="2b26f-118">Text value</span></span>

<span data-ttu-id="2b26f-119">Текстовое значение представляет устаревший адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="2b26f-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2b26f-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="2b26f-120">Remarks</span></span>

<span data-ttu-id="2b26f-121">Элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) является альтернативным элементом для запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="2b26f-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="2b26f-122">Он используется при наличии почтового ящика на компьютере под управлением Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="2b26f-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="2b26f-123">См. также</span><span class="sxs-lookup"><span data-stu-id="2b26f-123">See also</span></span>

- [<span data-ttu-id="2b26f-124">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="2b26f-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

