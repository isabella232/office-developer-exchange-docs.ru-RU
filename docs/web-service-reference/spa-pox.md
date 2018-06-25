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
description: Элемент SPA указывает, необходима ли проверка подлинности пароля (SPA).
ms.openlocfilehash: 1fb0f3bb40e64be89eae7dfc208d51387f532191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835533"
---
# <a name="spa-pox"></a><span data-ttu-id="a662f-103">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-103">SPA (POX)</span></span>

<span data-ttu-id="a662f-104">Элемент **SPA** указывает, необходима ли проверка подлинности пароля (SPA).</span><span class="sxs-lookup"><span data-stu-id="a662f-104">The **SPA** element indicates whether Secure Password Authentication (SPA) is required.</span></span> 
  
[<span data-ttu-id="a662f-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a662f-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a662f-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a662f-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a662f-109">SPA (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-109">SPA (POX)</span></span>](spa-pox.md)
  
```xml
<SPA/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a662f-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a662f-110">Attributes and elements</span></span>

<span data-ttu-id="a662f-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a662f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a662f-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a662f-112">Attributes</span></span>

<span data-ttu-id="a662f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a662f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a662f-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a662f-114">Child elements</span></span>

<span data-ttu-id="a662f-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="a662f-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a662f-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a662f-116">Parent elements</span></span>

|<span data-ttu-id="a662f-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a662f-117">**Element**</span></span>|<span data-ttu-id="a662f-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a662f-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a662f-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a662f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a662f-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a662f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a662f-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a662f-121">Text value</span></span>

<span data-ttu-id="a662f-122">Текстовое значение указывает, будет ли SPA является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a662f-122">The text value indicates whether SPA is required.</span></span> <span data-ttu-id="a662f-123">**Если значение текста,** SPA является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a662f-123">If the text value is **on**, SPA is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a662f-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="a662f-124">Remarks</span></span>

<span data-ttu-id="a662f-125">Если этот элемент не указан, значением по умолчанию — это значение **на**.</span><span class="sxs-lookup"><span data-stu-id="a662f-125">If this element is not present, the default value is set to **on**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="a662f-126">См. также</span><span class="sxs-lookup"><span data-stu-id="a662f-126">See also</span></span>



[<span data-ttu-id="a662f-127">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a662f-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

