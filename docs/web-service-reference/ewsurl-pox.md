---
title: EwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73cebc8c-770a-4f1b-b93e-51e7e2f3e342
description: Элемент EwsUrl указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: c968b13a069cdc15803c1eb491244b4dc1aa422f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762410"
---
# <a name="ewsurl-pox"></a><span data-ttu-id="98d7c-103">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-103">EwsUrl (POX)</span></span>

<span data-ttu-id="98d7c-104">Элемент **EwsUrl** указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="98d7c-104">The **EwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="98d7c-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="98d7c-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="98d7c-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="98d7c-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="98d7c-109">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-109">EwsUrl (POX)</span></span>](ewsurl-pox.md)
  
```XML
<EwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="98d7c-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="98d7c-110">Attributes and elements</span></span>

<span data-ttu-id="98d7c-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="98d7c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="98d7c-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="98d7c-112">Attributes</span></span>

<span data-ttu-id="98d7c-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="98d7c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="98d7c-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="98d7c-114">Child elements</span></span>

<span data-ttu-id="98d7c-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="98d7c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="98d7c-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="98d7c-116">Parent elements</span></span>

|<span data-ttu-id="98d7c-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="98d7c-117">**Element**</span></span>|<span data-ttu-id="98d7c-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="98d7c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="98d7c-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="98d7c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="98d7c-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="98d7c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="98d7c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="98d7c-121">Text value</span></span>

<span data-ttu-id="98d7c-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="98d7c-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="98d7c-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="98d7c-123">Remarks</span></span>

<span data-ttu-id="98d7c-124">Элемент **EwsUrl** является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="98d7c-124">The **EwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="98d7c-125">См. также</span><span class="sxs-lookup"><span data-stu-id="98d7c-125">See also</span></span>



[<span data-ttu-id="98d7c-126">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="98d7c-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

