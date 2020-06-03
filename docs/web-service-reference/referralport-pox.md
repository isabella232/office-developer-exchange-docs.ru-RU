---
title: Реферралпорт (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: cd693f1e-fed4-4eb9-8297-178906f47050
description: Элемент Реферралпорт указывает порт, используемый для получения ссылки на каталог.
ms.openlocfilehash: 6b3968d7b2f252439d2dfbc647bd8337668cf818
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456796"
---
# <a name="referralport-pox"></a><span data-ttu-id="71e22-103">Реферралпорт (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-103">ReferralPort (POX)</span></span>

<span data-ttu-id="71e22-104">Элемент **реферралпорт** указывает порт, используемый для получения ссылки на каталог.</span><span class="sxs-lookup"><span data-stu-id="71e22-104">The **ReferralPort** element specifies the port that is used to get a referral to a directory.</span></span> 
  
[<span data-ttu-id="71e22-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="71e22-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="71e22-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="71e22-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="71e22-109">Реферралпорт (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-109">ReferralPort (POX)</span></span>](referralport-pox.md)
  
```xml
<ReferralPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="71e22-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="71e22-110">Attributes and elements</span></span>

<span data-ttu-id="71e22-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="71e22-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71e22-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="71e22-112">Attributes</span></span>

<span data-ttu-id="71e22-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="71e22-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71e22-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="71e22-114">Child elements</span></span>

<span data-ttu-id="71e22-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="71e22-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71e22-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="71e22-116">Parent elements</span></span>

|<span data-ttu-id="71e22-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="71e22-117">**Element**</span></span>|<span data-ttu-id="71e22-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="71e22-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="71e22-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="71e22-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="71e22-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="71e22-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="71e22-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="71e22-121">Text value</span></span>

<span data-ttu-id="71e22-122">Текстовое значение представляет порт, используемый для доступа к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="71e22-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="71e22-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="71e22-123">Remarks</span></span>

<span data-ttu-id="71e22-124">Элемент **реферралпорт** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен "сумме" или "expr".</span><span class="sxs-lookup"><span data-stu-id="71e22-124">The **ReferralPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="71e22-125">См. также</span><span class="sxs-lookup"><span data-stu-id="71e22-125">See also</span></span>



[<span data-ttu-id="71e22-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="71e22-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

