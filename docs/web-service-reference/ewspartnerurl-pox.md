---
title: Евспартнерурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ebae21c-3efa-4239-9b49-4a3a8871449b
description: Элемент Евспартнерурл указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: a67eb17bb3db67a922c53ba5e37900ee0a9b956b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526111"
---
# <a name="ewspartnerurl-pox"></a><span data-ttu-id="cf524-103">Евспартнерурл (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-103">EwsPartnerUrl (POX)</span></span>

<span data-ttu-id="cf524-104">Элемент **евспартнерурл** указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="cf524-104">The **EwsPartnerUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="cf524-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="cf524-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="cf524-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="cf524-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="cf524-109">Евспартнерурл (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-109">EwsPartnerUrl (POX)</span></span>](ewspartnerurl-pox.md)
  
```XML
<EwsPartnerUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cf524-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cf524-110">Attributes and elements</span></span>

<span data-ttu-id="cf524-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cf524-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf524-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cf524-112">Attributes</span></span>

<span data-ttu-id="cf524-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf524-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf524-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cf524-114">Child elements</span></span>

<span data-ttu-id="cf524-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="cf524-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cf524-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cf524-116">Parent elements</span></span>

|<span data-ttu-id="cf524-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cf524-117">**Element**</span></span>|<span data-ttu-id="cf524-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cf524-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf524-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="cf524-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cf524-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cf524-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cf524-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="cf524-121">Text value</span></span>

<span data-ttu-id="cf524-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="cf524-122">The text value represents the URL of the EWS endpoint for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cf524-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="cf524-123">Remarks</span></span>

<span data-ttu-id="cf524-124">Элемент **евспартнерурл** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="cf524-124">The **EwsPartnerUrl** element is an optional child element of the **Protocol** element.</span></span> <span data-ttu-id="cf524-125">Он эквивалентен элементу [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="cf524-125">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cf524-126">См. также</span><span class="sxs-lookup"><span data-stu-id="cf524-126">See also</span></span>



[<span data-ttu-id="cf524-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="cf524-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

