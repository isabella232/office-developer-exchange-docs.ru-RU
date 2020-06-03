---
title: RedirectUrl адресом (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: Элемент redirectUrl адресом содержит URL-адрес компьютера, на котором работает Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения.
ms.openlocfilehash: 5400b1e7a4bb7ebebc58b6a0f1fc9bf37f5a2e22
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468091"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="0a79f-103">RedirectUrl адресом (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="0a79f-104">Элемент **redirectUrl адресом** содержит URL-адрес компьютера, на котором работает Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа, который следует использовать для получения параметров автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0a79f-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="0a79f-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="0a79f-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="0a79f-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="0a79f-108">RedirectUrl адресом (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="0a79f-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0a79f-109">Attributes and elements</span></span>

<span data-ttu-id="0a79f-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0a79f-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0a79f-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0a79f-111">Attributes</span></span>

<span data-ttu-id="0a79f-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0a79f-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0a79f-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0a79f-113">Child elements</span></span>

<span data-ttu-id="0a79f-114">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0a79f-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0a79f-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0a79f-115">Parent elements</span></span>

|<span data-ttu-id="0a79f-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0a79f-116">**Element**</span></span>|<span data-ttu-id="0a79f-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0a79f-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0a79f-118">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="0a79f-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="0a79f-119">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="0a79f-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0a79f-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0a79f-120">Text value</span></span>

<span data-ttu-id="0a79f-121">Текстовое значение представляет URL-адрес сервера клиентского доступа, который должен использоваться для получения параметров автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="0a79f-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0a79f-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="0a79f-122">Remarks</span></span>

<span data-ttu-id="0a79f-123">Клиентское приложение должно прекратить перенаправление после 10 перенаправлений.</span><span class="sxs-lookup"><span data-stu-id="0a79f-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="0a79f-124">См. также</span><span class="sxs-lookup"><span data-stu-id="0a79f-124">See also</span></span>



[<span data-ttu-id="0a79f-125">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="0a79f-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

