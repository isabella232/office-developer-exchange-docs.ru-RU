---
title: EwsUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 73cebc8c-770a-4f1b-b93e-51e7e2f3e342
description: Элемент EwsUrl указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: 295e65ddf14524a41c5cb714df78703dbf855a05
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44454353"
---
# <a name="ewsurl-pox"></a><span data-ttu-id="80046-103">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-103">EwsUrl (POX)</span></span>

<span data-ttu-id="80046-104">Элемент **EwsUrl** указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="80046-104">The **EwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="80046-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="80046-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="80046-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="80046-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="80046-109">EwsUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-109">EwsUrl (POX)</span></span>](ewsurl-pox.md)
  
```XML
<EwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="80046-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="80046-110">Attributes and elements</span></span>

<span data-ttu-id="80046-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="80046-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="80046-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="80046-112">Attributes</span></span>

<span data-ttu-id="80046-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80046-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="80046-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="80046-114">Child elements</span></span>

<span data-ttu-id="80046-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="80046-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="80046-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="80046-116">Parent elements</span></span>

|<span data-ttu-id="80046-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="80046-117">**Element**</span></span>|<span data-ttu-id="80046-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="80046-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="80046-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="80046-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="80046-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="80046-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="80046-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="80046-121">Text value</span></span>

<span data-ttu-id="80046-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="80046-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="80046-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="80046-123">Remarks</span></span>

<span data-ttu-id="80046-124">Элемент **EwsUrl** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="80046-124">The **EwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="80046-125">См. также</span><span class="sxs-lookup"><span data-stu-id="80046-125">See also</span></span>



[<span data-ttu-id="80046-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="80046-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

