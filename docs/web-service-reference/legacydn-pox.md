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
ms.openlocfilehash: b9af4278a5421dc932573396c3563a64a78de41e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526384"
---
# <a name="legacydn-pox"></a><span data-ttu-id="3baa4-103">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="3baa4-103">LegacyDN (POX)</span></span>

<span data-ttu-id="3baa4-104">Элемент **LegacyDN** определяет почтовый ящик пользователя по устаревшему различающеу имени.</span><span class="sxs-lookup"><span data-stu-id="3baa4-104">The **LegacyDN** element identifies a user's mailbox by legacy distinguished name.</span></span> 
  
```xml
<LegacyDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3baa4-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3baa4-105">Attributes and elements</span></span>

<span data-ttu-id="3baa4-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3baa4-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3baa4-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3baa4-107">Attributes</span></span>

<span data-ttu-id="3baa4-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3baa4-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3baa4-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3baa4-109">Child elements</span></span>

<span data-ttu-id="3baa4-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="3baa4-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3baa4-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3baa4-111">Parent elements</span></span>

|<span data-ttu-id="3baa4-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3baa4-112">**Element**</span></span>|<span data-ttu-id="3baa4-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3baa4-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3baa4-114">Запрос (POX)</span><span class="sxs-lookup"><span data-stu-id="3baa4-114">Request (POX)</span></span>](request-pox.md) <br/> |<span data-ttu-id="3baa4-115">Содержит запрос к службе автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3baa4-115">Contains the request to the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3baa4-116">Пользователь (POX)</span><span class="sxs-lookup"><span data-stu-id="3baa4-116">User (POX)</span></span>](user-pox.md) <br/> |<span data-ttu-id="3baa4-117">Предоставляет сведения, относящиеся к пользователю.</span><span class="sxs-lookup"><span data-stu-id="3baa4-117">Provides user-specific information.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3baa4-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3baa4-118">Text value</span></span>

<span data-ttu-id="3baa4-119">Текстовое значение представляет устаревший адрес электронной почты пользователя.</span><span class="sxs-lookup"><span data-stu-id="3baa4-119">The text value represents a user's legacy e-mail address.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3baa4-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="3baa4-120">Remarks</span></span>

<span data-ttu-id="3baa4-121">Элемент [EmailAddress (нонемптистрингтипе)](emailaddress-nonemptystringtype.md) является альтернативным элементом для запроса автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="3baa4-121">The [EmailAddress (NonEmptyStringType)](emailaddress-nonemptystringtype.md) element is an alternative element for an Autodiscover request.</span></span> <span data-ttu-id="3baa4-122">Он используется при наличии почтового ящика на компьютере под управлением Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="3baa4-122">It is used when a mailbox exists on a computer that is running Microsoft Exchange Server 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3baa4-123">См. также</span><span class="sxs-lookup"><span data-stu-id="3baa4-123">See also</span></span>

- [<span data-ttu-id="3baa4-124">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="3baa4-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

