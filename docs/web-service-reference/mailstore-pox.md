---
title: Маилсторе (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: Элемент Маилсторе содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 635228fcfeb3ad791c845050b82666a6e060b229
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459793"
---
# <a name="mailstore-pox"></a><span data-ttu-id="9de24-103">Маилсторе (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-103">MailStore (POX)</span></span>

<span data-ttu-id="9de24-104">Элемент **маилсторе** содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="9de24-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="9de24-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="9de24-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="9de24-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="9de24-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="9de24-109">Маилсторе (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9de24-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9de24-110">Attributes and elements</span></span>

<span data-ttu-id="9de24-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9de24-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9de24-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9de24-112">Attributes</span></span>

<span data-ttu-id="9de24-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9de24-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9de24-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9de24-114">Child elements</span></span>

|<span data-ttu-id="9de24-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9de24-115">**Element**</span></span>|<span data-ttu-id="9de24-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9de24-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9de24-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="9de24-118">Содержит URL-адрес, который должен использоваться для доступа к почтовому ящику пользователя извне сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="9de24-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="9de24-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="9de24-120">Содержит URL-адрес, который должен использоваться для доступа к почтовому ящику пользователя из сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="9de24-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9de24-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9de24-121">Parent elements</span></span>

|<span data-ttu-id="9de24-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9de24-122">**Element**</span></span>|<span data-ttu-id="9de24-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9de24-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9de24-124">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9de24-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9de24-125">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9de24-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9de24-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="9de24-126">Remarks</span></span>

<span data-ttu-id="9de24-127">Элемент **маилсторе** присутствует в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно".</span><span class="sxs-lookup"><span data-stu-id="9de24-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="9de24-128">Элемент **маилсторе** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="9de24-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9de24-129">См. также</span><span class="sxs-lookup"><span data-stu-id="9de24-129">See also</span></span>



[<span data-ttu-id="9de24-130">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9de24-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

