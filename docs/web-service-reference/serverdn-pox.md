---
title: ServerDN (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: Элемент ServerDN указывает различающееся имя компьютера, на котором выполняется Microsoft Exchange Server 2007.
ms.openlocfilehash: d2b9ce663d8245a78acd088b0622406c0dfcb4da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835374"
---
# <a name="serverdn-pox"></a><span data-ttu-id="09897-103">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-103">ServerDN (POX)</span></span>

<span data-ttu-id="09897-104">Элемент **ServerDN** указывает различающееся имя компьютера, на котором выполняется Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="09897-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="09897-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="09897-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="09897-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="09897-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="09897-109">ServerDN (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="09897-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="09897-110">Attributes and elements</span></span>

<span data-ttu-id="09897-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="09897-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="09897-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="09897-112">Attributes</span></span>

<span data-ttu-id="09897-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="09897-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="09897-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="09897-114">Child elements</span></span>

<span data-ttu-id="09897-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="09897-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="09897-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="09897-116">Parent elements</span></span>

|<span data-ttu-id="09897-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="09897-117">**Element**</span></span>|<span data-ttu-id="09897-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="09897-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="09897-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="09897-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="09897-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="09897-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="09897-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="09897-121">Text value</span></span>

<span data-ttu-id="09897-122">Текстовое значение представляет различающееся имя Exchange server.</span><span class="sxs-lookup"><span data-stu-id="09897-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="09897-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="09897-123">Remarks</span></span>

<span data-ttu-id="09897-124">**ServerDN** значение используется только в том случае, если [Тип (POX)](type-pox.md) равно курс</span><span class="sxs-lookup"><span data-stu-id="09897-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="09897-125">См. также</span><span class="sxs-lookup"><span data-stu-id="09897-125">See also</span></span>



[<span data-ttu-id="09897-126">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="09897-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

