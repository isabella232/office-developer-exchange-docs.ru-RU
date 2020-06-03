---
title: Екпурл (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 7cbd6076-9981-4c65-a296-5e57518671b5
description: Элемент Екпурл указывает URL-адрес панели управления Exchange для пользователя с включенной поддержкой почты.
ms.openlocfilehash: b761147dc5912652bca2847bd5ec0d305e0624b3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461277"
---
# <a name="ecpurl-pox"></a><span data-ttu-id="ddcc2-103">Екпурл (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-103">EcpUrl (POX)</span></span>

<span data-ttu-id="ddcc2-104">Элемент **екпурл** указывает URL-адрес панели управления Exchange для пользователя с включенной поддержкой почты.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-104">The **EcpUrl** element specifies the URL of the Exchange Control Panel for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="ddcc2-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ddcc2-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ddcc2-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ddcc2-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ddcc2-109">Екпурл (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-109">EcpUrl (POX)</span></span>](ecpurl-pox.md)
  
```XML
<EcpUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ddcc2-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ddcc2-110">Attributes and elements</span></span>

<span data-ttu-id="ddcc2-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ddcc2-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ddcc2-112">Attributes</span></span>

<span data-ttu-id="ddcc2-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ddcc2-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ddcc2-114">Child elements</span></span>

<span data-ttu-id="ddcc2-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ddcc2-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ddcc2-116">Parent elements</span></span>

|<span data-ttu-id="ddcc2-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ddcc2-117">**Element**</span></span>|<span data-ttu-id="ddcc2-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ddcc2-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ddcc2-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="ddcc2-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ddcc2-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ddcc2-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ddcc2-121">Text value</span></span>

<span data-ttu-id="ddcc2-122">Текстовое значение представляет URL-адрес панели управления Exchange для пользователя.</span><span class="sxs-lookup"><span data-stu-id="ddcc2-122">The text value represents the URL of the Exchange Control Panel for the user.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ddcc2-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="ddcc2-123">Remarks</span></span>

<span data-ttu-id="ddcc2-124">Элемент **екпурл** является необязательным дочерним элементом элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="ddcc2-124">The **EcpUrl** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ddcc2-125">См. также</span><span class="sxs-lookup"><span data-stu-id="ddcc2-125">See also</span></span>



[<span data-ttu-id="ddcc2-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ddcc2-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

