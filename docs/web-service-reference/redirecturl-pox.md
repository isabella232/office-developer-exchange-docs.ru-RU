---
title: RedirectUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: c54f310f-8c99-4c37-8e73-ac87722b6229
description: Элемент RedirectUrl содержит URL-адрес компьютера, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, который следует использовать для получения параметров службы автообнаружения.
ms.openlocfilehash: 3b634f1a3a3d44b6aae1a826a005149200641dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835027"
---
# <a name="redirecturl-pox"></a><span data-ttu-id="013bd-103">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-103">RedirectUrl (POX)</span></span>

<span data-ttu-id="013bd-104">Элемент **RedirectUrl** содержит URL-адрес компьютера, на котором выполняется Microsoft Exchange Server 2007, который имеет роль сервера клиентского доступа установлен, который следует использовать для получения параметров службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="013bd-104">The **RedirectUrl** element contains the URL of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed that should be used to obtain Autodiscover settings.</span></span> 
  
[<span data-ttu-id="013bd-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="013bd-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="013bd-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="013bd-108">RedirectUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-108">RedirectUrl (POX)</span></span>](redirecturl-pox.md)
  
```xml
<RedirectUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="013bd-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="013bd-109">Attributes and elements</span></span>

<span data-ttu-id="013bd-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="013bd-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="013bd-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="013bd-111">Attributes</span></span>

<span data-ttu-id="013bd-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="013bd-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="013bd-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="013bd-113">Child elements</span></span>

<span data-ttu-id="013bd-114">Нет.</span><span class="sxs-lookup"><span data-stu-id="013bd-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="013bd-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="013bd-115">Parent elements</span></span>

|<span data-ttu-id="013bd-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="013bd-116">**Element**</span></span>|<span data-ttu-id="013bd-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="013bd-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="013bd-118">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="013bd-118">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="013bd-119">Задает параметры учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="013bd-119">Specifies account settings for the user.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="013bd-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="013bd-120">Text value</span></span>

<span data-ttu-id="013bd-121">Текстовое значение представляет URL-адрес сервера клиентского доступа, который следует использовать для получения параметров службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="013bd-121">The text value represents the URL of the Client Access server that should be used to obtain Autodiscover settings.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="013bd-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="013bd-122">Remarks</span></span>

<span data-ttu-id="013bd-123">Клиентское приложение должны прекратить перенаправление после 10 перенаправлений.</span><span class="sxs-lookup"><span data-stu-id="013bd-123">The client application should stop redirecting after 10 redirects.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="013bd-124">См. также</span><span class="sxs-lookup"><span data-stu-id="013bd-124">See also</span></span>



[<span data-ttu-id="013bd-125">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="013bd-125">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

