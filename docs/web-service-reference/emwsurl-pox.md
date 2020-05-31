---
title: Емвсурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: Элемент Емвсурл указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: d8905d098c9978c3413f67e9a1b2443a52fb0d1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762328"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="1942e-103">Емвсурл (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="1942e-104">Элемент **емвсурл** указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="1942e-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="1942e-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="1942e-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="1942e-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="1942e-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="1942e-109">Емвсурл (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1942e-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1942e-110">Attributes and elements</span></span>

<span data-ttu-id="1942e-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="1942e-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1942e-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1942e-112">Attributes</span></span>

<span data-ttu-id="1942e-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="1942e-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1942e-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1942e-114">Child elements</span></span>

<span data-ttu-id="1942e-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="1942e-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1942e-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1942e-116">Parent elements</span></span>

|<span data-ttu-id="1942e-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1942e-117">**Element**</span></span>|<span data-ttu-id="1942e-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1942e-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1942e-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="1942e-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="1942e-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="1942e-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1942e-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1942e-121">Text value</span></span>

<span data-ttu-id="1942e-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="1942e-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="1942e-123">Он эквивалентен элементу [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="1942e-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1942e-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="1942e-124">Remarks</span></span>

<span data-ttu-id="1942e-125">Элемент **емвсурл** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="1942e-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1942e-126">См. также</span><span class="sxs-lookup"><span data-stu-id="1942e-126">See also</span></span>

- [<span data-ttu-id="1942e-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="1942e-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

