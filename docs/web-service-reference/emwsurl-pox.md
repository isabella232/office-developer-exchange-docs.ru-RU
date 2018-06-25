---
title: EmwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: Элемент EmwsUrl указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762328"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="a0bc6-103">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="a0bc6-104">Элемент **EmwsUrl** указывает URL-адрес экземпляра наиболее конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="a0bc6-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="a0bc6-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="a0bc6-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="a0bc6-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="a0bc6-109">EmwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="a0bc6-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a0bc6-110">Attributes and elements</span></span>

<span data-ttu-id="a0bc6-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0bc6-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a0bc6-112">Attributes</span></span>

<span data-ttu-id="a0bc6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0bc6-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a0bc6-114">Child elements</span></span>

<span data-ttu-id="a0bc6-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0bc6-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a0bc6-116">Parent elements</span></span>

|<span data-ttu-id="a0bc6-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a0bc6-117">**Element**</span></span>|<span data-ttu-id="a0bc6-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a0bc6-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a0bc6-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a0bc6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a0bc6-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a0bc6-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a0bc6-121">Text value</span></span>

<span data-ttu-id="a0bc6-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="a0bc6-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="a0bc6-123">Это эквивалентно элемент [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="a0bc6-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a0bc6-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="a0bc6-124">Remarks</span></span>

<span data-ttu-id="a0bc6-125">Элемент **EmwsUrl** является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="a0bc6-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a0bc6-126">См. также</span><span class="sxs-lookup"><span data-stu-id="a0bc6-126">See also</span></span>

- [<span data-ttu-id="a0bc6-127">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a0bc6-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

