---
title: Усепопаус (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: Элемент Усепопаус указывает, используются ли для протокола SMTP сведения для проверки подлинности, предоставляемые для типа учетной записи POP3.
ms.openlocfilehash: 8d5bfffaab31c382ad43915e18b8a7a2b2737c21
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466509"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="e4c8b-103">Усепопаус (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="e4c8b-104">Элемент **усепопаус** указывает, используются ли для протокола SMTP сведения для проверки подлинности, предоставляемые для типа учетной записи POP3.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="e4c8b-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="e4c8b-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="e4c8b-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="e4c8b-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="e4c8b-109">Усепопаус (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e4c8b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e4c8b-110">Attributes and elements</span></span>

<span data-ttu-id="e4c8b-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4c8b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e4c8b-112">Attributes</span></span>

<span data-ttu-id="e4c8b-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4c8b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e4c8b-114">Child elements</span></span>

<span data-ttu-id="e4c8b-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4c8b-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e4c8b-116">Parent elements</span></span>

|<span data-ttu-id="e4c8b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e4c8b-117">**Element**</span></span>|<span data-ttu-id="e4c8b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e4c8b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4c8b-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="e4c8b-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="e4c8b-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4c8b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e4c8b-121">Text value</span></span>

<span data-ttu-id="e4c8b-122">Текстовое значение указывает, используются ли для протокола SMTP сведения для проверки подлинности, предоставляемые для типа учетной записи POP3.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="e4c8b-123">Возможные **значения:** **On и on** .</span><span class="sxs-lookup"><span data-stu-id="e4c8b-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4c8b-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="e4c8b-124">Remarks</span></span>

<span data-ttu-id="e4c8b-125">Элемент **усепопаус** используется только в том случае, если [тип (POX)](type-pox.md) — SMTP.</span><span class="sxs-lookup"><span data-stu-id="e4c8b-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="e4c8b-126">См. также</span><span class="sxs-lookup"><span data-stu-id="e4c8b-126">See also</span></span>



[<span data-ttu-id="e4c8b-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="e4c8b-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

