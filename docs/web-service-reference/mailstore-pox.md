---
title: MailStore (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: af338f99-9e62-4124-9bff-8d7cc2008161
description: Элемент MailStore содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 4c82c7b61752cf7d91287a3968f6c642f4943855
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834301"
---
# <a name="mailstore-pox"></a><span data-ttu-id="ccbdf-103">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-103">MailStore (POX)</span></span>

<span data-ttu-id="ccbdf-104">Элемент **MailStore** содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-104">The **MailStore** element contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="ccbdf-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="ccbdf-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="ccbdf-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="ccbdf-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="ccbdf-109">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-109">MailStore (POX)</span></span>](mailstore-pox.md)
  
```XML
<MailStore>
   <ExternalUrl/>
   <InternalUrl/>
</MailStore>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="ccbdf-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ccbdf-110">Attributes and elements</span></span>

<span data-ttu-id="ccbdf-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ccbdf-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ccbdf-112">Attributes</span></span>

<span data-ttu-id="ccbdf-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ccbdf-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ccbdf-114">Child elements</span></span>

|<span data-ttu-id="ccbdf-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ccbdf-115">**Element**</span></span>|<span data-ttu-id="ccbdf-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ccbdf-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ccbdf-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="ccbdf-118">Содержит URL-адрес, который должен использоваться для доступа к почтового ящика пользователя из за пределами сети организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-118">Contains the URL that should be used to access the user's mailbox from outside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="ccbdf-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="ccbdf-120">Содержит URL-адрес, который должен использоваться для доступа к почтового ящика пользователя из внутри сети организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-120">Contains the URL that should be used to access the user's mailbox from inside the organization's network by means of the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ccbdf-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ccbdf-121">Parent elements</span></span>

|<span data-ttu-id="ccbdf-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ccbdf-122">**Element**</span></span>|<span data-ttu-id="ccbdf-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ccbdf-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ccbdf-124">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="ccbdf-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="ccbdf-125">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ccbdf-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ccbdf-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="ccbdf-126">Remarks</span></span>

<span data-ttu-id="ccbdf-127">Элемент **MailStore** присутствует в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp».</span><span class="sxs-lookup"><span data-stu-id="ccbdf-127">The **MailStore** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="ccbdf-128">Элемент **MailStore** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1).</span><span class="sxs-lookup"><span data-stu-id="ccbdf-128">The **MailStore** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="ccbdf-129">См. также</span><span class="sxs-lookup"><span data-stu-id="ccbdf-129">See also</span></span>



[<span data-ttu-id="ccbdf-130">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="ccbdf-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

