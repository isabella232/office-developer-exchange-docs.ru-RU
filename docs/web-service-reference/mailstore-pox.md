---
title: Маилсторе (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: Элемент Маилсторе содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834301"
---
# <a name="mailstore-pox"></a><span data-ttu-id="07bc3-103">Маилсторе (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-103">MailStore (POX)</span></span>

<span data-ttu-id="07bc3-104">Элемент **маилсторе** содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="07bc3-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="07bc3-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="07bc3-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="07bc3-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="07bc3-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="07bc3-109">Маилсторе (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="07bc3-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="07bc3-110">Attributes and elements</span></span>

<span data-ttu-id="07bc3-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="07bc3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="07bc3-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="07bc3-112">Attributes</span></span>

<span data-ttu-id="07bc3-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="07bc3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="07bc3-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="07bc3-114">Child elements</span></span>

|<span data-ttu-id="07bc3-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07bc3-115">**Element**</span></span>|<span data-ttu-id="07bc3-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07bc3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07bc3-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="07bc3-118">Содержит URL-адрес, который должен использоваться для доступа к почтовому ящику пользователя извне сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="07bc3-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="07bc3-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="07bc3-120">Содержит URL-адрес, который должен использоваться для доступа к почтовому ящику пользователя из сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="07bc3-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="07bc3-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="07bc3-121">Parent elements</span></span>

|<span data-ttu-id="07bc3-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="07bc3-122">**Element**</span></span>|<span data-ttu-id="07bc3-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="07bc3-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="07bc3-124">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="07bc3-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="07bc3-125">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="07bc3-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="07bc3-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="07bc3-126">Remarks</span></span>

<span data-ttu-id="07bc3-127">Элемент **маилсторе** присутствует в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно".</span><span class="sxs-lookup"><span data-stu-id="07bc3-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="07bc3-128">Элемент **маилсторе** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="07bc3-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="07bc3-129">См. также</span><span class="sxs-lookup"><span data-stu-id="07bc3-129">See also</span></span>



[<span data-ttu-id="07bc3-130">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="07bc3-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

