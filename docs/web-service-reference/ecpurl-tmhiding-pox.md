---
title: EcpUrl-tmHiding (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 9b9ae15b-3ac1-45ac-85ba-38c7231fe508
description: Элемент EcpUrl tmHiding указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента EcpUrl (POX) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта.
ms.openlocfilehash: 461e9780dbd657ba0ba8b9ce9ea4fe902cba9698
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762248"
---
# <a name="ecpurl-tmhiding-pox"></a><span data-ttu-id="dd022-103">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-103">EcpUrl-tmHiding (POX)</span></span>

<span data-ttu-id="dd022-104">Элемент **EcpUrl tmHiding** указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dd022-104">The **EcpUrl-tmHiding** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> 
  
[<span data-ttu-id="dd022-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="dd022-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="dd022-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="dd022-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="dd022-109">EcpUrl-tmHiding (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-109">EcpUrl-tmHiding (POX)</span></span>](ecpurl-tmhiding-pox.md)
  
```XML
<EcpUrl-tmHiding/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="dd022-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="dd022-110">Attributes and elements</span></span>

<span data-ttu-id="dd022-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="dd022-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd022-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="dd022-112">Attributes</span></span>

<span data-ttu-id="dd022-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd022-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd022-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="dd022-114">Child elements</span></span>

<span data-ttu-id="dd022-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="dd022-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd022-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="dd022-116">Parent elements</span></span>

|<span data-ttu-id="dd022-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="dd022-117">**Element**</span></span>|<span data-ttu-id="dd022-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="dd022-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd022-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="dd022-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="dd022-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="dd022-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd022-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="dd022-121">Text value</span></span>

<span data-ttu-id="dd022-122">Текстовое значение представляет сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для отмены подписки пользователя из почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dd022-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to unsubscribe the user from a site mailbox.</span></span> <span data-ttu-id="dd022-123">Значение элемента **EcpUrl tmHiding** содержит параметры, содержащиеся в "<" и ">" символы, которые заменяются клиентом, как показано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="dd022-123">The value of the **EcpUrl-tmHiding** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="dd022-124">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="dd022-124">**Parameter**</span></span>|<span data-ttu-id="dd022-125">**Заменить**</span><span class="sxs-lookup"><span data-stu-id="dd022-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="dd022-126">
  _Id_</span><span class="sxs-lookup"><span data-stu-id="dd022-126">_Id_</span></span> <br/> |<span data-ttu-id="dd022-127">Адрес электронной почты SMTP или X500 различающееся имя почтового ящика сайта.</span><span class="sxs-lookup"><span data-stu-id="dd022-127">The SMTP email address or the X500 distinguished name of the site mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd022-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="dd022-128">Remarks</span></span>

<span data-ttu-id="dd022-129">Элемент **EcpUrl tmHiding** является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="dd022-129">The **EcpUrl-tmHiding** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="dd022-130">См. также</span><span class="sxs-lookup"><span data-stu-id="dd022-130">See also</span></span>



[<span data-ttu-id="dd022-131">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="dd022-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

