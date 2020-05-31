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
ms.openlocfilehash: 5045c0c5a9f15d5a31ac2e884b942e00dfb1f520
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835037"
---
# <a name="referralport-pox"></a><span data-ttu-id="3b539-103">Реферралпорт (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-103">ReferralPort (POX)</span></span>

<span data-ttu-id="3b539-104">Элемент **реферралпорт** указывает порт, используемый для получения ссылки на каталог.</span><span class="sxs-lookup"><span data-stu-id="3b539-104">The **ReferralPort** element specifies the port that is used to get a referral to a directory.</span></span> 
  
[<span data-ttu-id="3b539-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="3b539-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="3b539-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="3b539-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="3b539-109">Реферралпорт (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-109">ReferralPort (POX)</span></span>](referralport-pox.md)
  
```xml
<ReferralPort/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="3b539-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3b539-110">Attributes and elements</span></span>

<span data-ttu-id="3b539-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3b539-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b539-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3b539-112">Attributes</span></span>

<span data-ttu-id="3b539-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b539-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b539-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3b539-114">Child elements</span></span>

<span data-ttu-id="3b539-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="3b539-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3b539-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3b539-116">Parent elements</span></span>

|<span data-ttu-id="3b539-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3b539-117">**Element**</span></span>|<span data-ttu-id="3b539-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3b539-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b539-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="3b539-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="3b539-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3b539-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3b539-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="3b539-121">Text value</span></span>

<span data-ttu-id="3b539-122">Текстовое значение представляет порт, используемый для доступа к серверу Exchange Server.</span><span class="sxs-lookup"><span data-stu-id="3b539-122">The text value represents the port that is used to access the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3b539-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="3b539-123">Remarks</span></span>

<span data-ttu-id="3b539-124">Элемент **реферралпорт** используется только в том случае, если элемент [Type (POX)](type-pox.md) равен "сумме" или "expr".</span><span class="sxs-lookup"><span data-stu-id="3b539-124">The **ReferralPort** element is only used when the [Type (POX)](type-pox.md) element equals EXCH or EXPR.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="3b539-125">См. также</span><span class="sxs-lookup"><span data-stu-id="3b539-125">See also</span></span>



[<span data-ttu-id="3b539-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="3b539-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

