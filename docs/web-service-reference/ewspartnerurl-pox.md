---
title: Евспартнерурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: Элемент Евспартнерурл указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: 97c33e1fed4adc8a9e8542d85e67c942118f6096
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762414"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="79c37-103">Евспартнерурл (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="79c37-104">Элемент **евспартнерурл** указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="79c37-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="79c37-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="79c37-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="79c37-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="79c37-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="79c37-109">Евспартнерурл (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="79c37-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="79c37-110">Attributes and elements</span></span>

<span data-ttu-id="79c37-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="79c37-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="79c37-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="79c37-112">Attributes</span></span>

<span data-ttu-id="79c37-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="79c37-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="79c37-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="79c37-114">Child elements</span></span>

<span data-ttu-id="79c37-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="79c37-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="79c37-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="79c37-116">Parent elements</span></span>

|<span data-ttu-id="79c37-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="79c37-117">**Element**</span></span>|<span data-ttu-id="79c37-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="79c37-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="79c37-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="79c37-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="79c37-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="79c37-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="79c37-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="79c37-121">Text value</span></span>

<span data-ttu-id="79c37-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="79c37-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="79c37-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="79c37-123">Remarks</span></span>

<span data-ttu-id="79c37-124">Элемент **евспартнерурл** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="79c37-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="79c37-125">Он эквивалентен элементу [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="79c37-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="79c37-126">См. также</span><span class="sxs-lookup"><span data-stu-id="79c37-126">See also</span></span>



[<span data-ttu-id="79c37-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="79c37-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

