---
title: EcpUrl-mt (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 5221745b-572c-44a5-afdb-41b58af44971
description: Элемент EcpUrl mt указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента EcpUrl (POX) для создания URL-адрес, который можно использовать для доступа к отслеживания параметров для пользователя с включенной поддержкой почты сообщений электронной почты.
ms.openlocfilehash: 13954a4dab8e81f4ba75b3578e6ba7f67f4b8b96
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762234"
---
# <a name="ecpurl-mt-pox"></a><span data-ttu-id="20981-103">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-103">EcpUrl-mt (POX)</span></span>

<span data-ttu-id="20981-104">Элемент **EcpUrl mt** указывает сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для доступа к отслеживания параметров для пользователя с включенной поддержкой почты сообщений электронной почты.</span><span class="sxs-lookup"><span data-stu-id="20981-104">The **EcpUrl-mt** element specifies a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email message tracking settings for a mail-enabled user.</span></span> 
  
[<span data-ttu-id="20981-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="20981-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="20981-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="20981-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="20981-109">EcpUrl-mt (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-109">EcpUrl-mt (POX)</span></span>](ecpurl-mt-pox.md)
  
```XML
<EcpUrl-mt/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="20981-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="20981-110">Attributes and elements</span></span>

<span data-ttu-id="20981-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="20981-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20981-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="20981-112">Attributes</span></span>

<span data-ttu-id="20981-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="20981-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20981-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="20981-114">Child elements</span></span>

<span data-ttu-id="20981-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="20981-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20981-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="20981-116">Parent elements</span></span>

|<span data-ttu-id="20981-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="20981-117">**Element**</span></span>|<span data-ttu-id="20981-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="20981-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20981-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="20981-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="20981-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="20981-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20981-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="20981-121">Text value</span></span>

<span data-ttu-id="20981-122">Текстовое значение представляет сокращенный URL-адрес, который может использоваться совместно с значение элемента [EcpUrl (POX)](ecpurl-pox.md) для создания URL-адрес, который можно использовать для доступа к электронной почте, отслеживание параметры для пользователя.</span><span class="sxs-lookup"><span data-stu-id="20981-122">The text value represents a partial URL that can be combined with the [EcpUrl (POX)](ecpurl-pox.md) element's value to generate a URL that can be used to access email tracking settings for the user.</span></span> <span data-ttu-id="20981-123">Значение элемента **EcpUrl mt** содержит параметры, содержащиеся в "<" и ">" символы, которые заменяются клиентом, как показано в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="20981-123">The value of the **EcpUrl-mt** element contains parameters contained within '<' and '>' characters that are substituted by the client as shown in the following table.</span></span> 
  
|<span data-ttu-id="20981-124">**Параметр**</span><span class="sxs-lookup"><span data-stu-id="20981-124">**Parameter**</span></span>|<span data-ttu-id="20981-125">**Заменить**</span><span class="sxs-lookup"><span data-stu-id="20981-125">**Substitute with**</span></span>|
|:-----|:-----|
| <span data-ttu-id="20981-126">_IsOwa_</span><span class="sxs-lookup"><span data-stu-id="20981-126">_IsOwa_</span></span> <br/> |<span data-ttu-id="20981-127">n</span><span class="sxs-lookup"><span data-stu-id="20981-127">n</span></span>  <br/> |
| <span data-ttu-id="20981-128">_MsgID_</span><span class="sxs-lookup"><span data-stu-id="20981-128">_MsgID_</span></span> <br/> |<span data-ttu-id="20981-129">Идентификатор сообщения Интернета сообщения для отслеживания в соответствии с заголовком идентификатор сообщения.</span><span class="sxs-lookup"><span data-stu-id="20981-129">Internet message identifier of the message to be tracked as specified by the Message-ID header.</span></span>  <br/> |
| <span data-ttu-id="20981-130">_MBX_</span><span class="sxs-lookup"><span data-stu-id="20981-130">_Mbx_</span></span> <br/> |<span data-ttu-id="20981-131">SMTP-адрес владельца почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="20981-131">The SMTP address of the mailbox owner.</span></span>  <br/> |
| <span data-ttu-id="20981-132">_Отправитель_</span><span class="sxs-lookup"><span data-stu-id="20981-132">_Sender_</span></span> <br/> |<span data-ttu-id="20981-133">SMTP-адрес отправителя сообщения.</span><span class="sxs-lookup"><span data-stu-id="20981-133">The SMTP address of the message's sender.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="20981-134">Замечания</span><span class="sxs-lookup"><span data-stu-id="20981-134">Remarks</span></span>

<span data-ttu-id="20981-135">Элемент **EcpUrl mt** является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="20981-135">The **EcpUrl-mt** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="20981-136">См. также</span><span class="sxs-lookup"><span data-stu-id="20981-136">See also</span></span>



[<span data-ttu-id="20981-137">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="20981-137">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

