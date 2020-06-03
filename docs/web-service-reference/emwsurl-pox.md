---
title: Емвсурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: cad0fa91-8d75-4dde-a484-518c837ae063
description: Элемент Емвсурл указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.
ms.openlocfilehash: 19e1078ae8d08513e85d75d87e960a910986f727
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530672"
---
# <a name="emwsurl-pox"></a><span data-ttu-id="66464-103">Емвсурл (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-103">EmwsUrl (POX)</span></span>

<span data-ttu-id="66464-104">Элемент **емвсурл** указывает URL-адрес лучшего экземпляра конечной точки для веб-служб Exchange (EWS) для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="66464-104">The **EmwsUrl** element specifies the URL of the best endpoint instance for Exchange Web Services (EWS) for a mail-enabled user.</span></span> 
  
- [<span data-ttu-id="66464-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md) 
- [<span data-ttu-id="66464-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="66464-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="66464-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="66464-109">Емвсурл (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-109">EmwsUrl (POX)</span></span>](emwsurl-pox.md)
  
```XML
<EmwsUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="66464-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="66464-110">Attributes and elements</span></span>

<span data-ttu-id="66464-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="66464-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="66464-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="66464-112">Attributes</span></span>

<span data-ttu-id="66464-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="66464-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="66464-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="66464-114">Child elements</span></span>

<span data-ttu-id="66464-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="66464-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="66464-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="66464-116">Parent elements</span></span>

|<span data-ttu-id="66464-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="66464-117">**Element**</span></span>|<span data-ttu-id="66464-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="66464-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="66464-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="66464-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="66464-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="66464-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="66464-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="66464-121">Text value</span></span>

<span data-ttu-id="66464-122">Текстовое значение представляет URL-адрес конечной точки EWS для пользователя.</span><span class="sxs-lookup"><span data-stu-id="66464-122">The text value represents the URL of the EWS endpoint for the user.</span></span> <span data-ttu-id="66464-123">Он эквивалентен элементу [EwsUrl (POX)](ewsurl-pox.md) .</span><span class="sxs-lookup"><span data-stu-id="66464-123">It is equivalent to the [EwsUrl (POX)](ewsurl-pox.md) element.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="66464-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="66464-124">Remarks</span></span>

<span data-ttu-id="66464-125">Элемент **емвсурл** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="66464-125">The **EmwsUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="66464-126">См. также</span><span class="sxs-lookup"><span data-stu-id="66464-126">See also</span></span>

- [<span data-ttu-id="66464-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="66464-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

