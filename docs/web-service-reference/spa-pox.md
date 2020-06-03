---
title: SPA (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fba018d5-0c65-4e1b-9767-d1ce8b356278
description: Элемент SPA указывает, требуется ли безопасная проверка пароля (SPA).
ms.openlocfilehash: cf57b3a6046b1b9b030b7cae81381189eee92c1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467643"
---
# <a name="spa-pox"></a><span data-ttu-id="b15c1-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-103">SPA (POX)</span></span>

<span data-ttu-id="b15c1-104">Элемент **Spa** указывает, требуется ли безопасная проверка пароля (SPA).</span><span class="sxs-lookup"><span data-stu-id="b15c1-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="b15c1-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="b15c1-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="b15c1-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="b15c1-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="b15c1-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="b15c1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b15c1-110">Attributes and elements</span></span>

<span data-ttu-id="b15c1-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b15c1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b15c1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b15c1-112">Attributes</span></span>

<span data-ttu-id="b15c1-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b15c1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b15c1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b15c1-114">Child elements</span></span>

<span data-ttu-id="b15c1-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b15c1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b15c1-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b15c1-116">Parent elements</span></span>

|<span data-ttu-id="b15c1-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b15c1-117">**Element**</span></span>|<span data-ttu-id="b15c1-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b15c1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b15c1-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="b15c1-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="b15c1-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b15c1-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b15c1-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b15c1-121">Text value</span></span>

<span data-ttu-id="b15c1-122">Текстовое значение указывает, требуется ли SPA.</span><span class="sxs-lookup"><span data-stu-id="b15c1-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="b15c1-123">Если текстовое значение — **включено**, то Spa является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b15c1-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b15c1-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="b15c1-124">Remarks</span></span>

<span data-ttu-id="b15c1-125">Если этот элемент отсутствует, используется значение по умолчанию, равное **On**.</span><span class="sxs-lookup"><span data-stu-id="b15c1-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="b15c1-126">См. также</span><span class="sxs-lookup"><span data-stu-id="b15c1-126">See also</span></span>



[<span data-ttu-id="b15c1-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="b15c1-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

