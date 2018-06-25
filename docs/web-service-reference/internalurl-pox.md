---
title: InternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 4649baa9-eec9-426d-952b-361818c25fe0
description: Элемент InternalUrl содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 3823236081961128b31bb2c0f563062897c55814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833950"
---
# <a name="internalurl-pox"></a><span data-ttu-id="69191-103">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="69191-103">InternalUrl (POX)</span></span>

<span data-ttu-id="69191-104">Элемент **InternalUrl** содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="69191-104">The **InternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from inside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<InternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="69191-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="69191-105">Attributes and elements</span></span>

<span data-ttu-id="69191-106">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="69191-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="69191-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="69191-107">Attributes</span></span>

<span data-ttu-id="69191-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="69191-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="69191-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="69191-109">Child elements</span></span>

<span data-ttu-id="69191-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="69191-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="69191-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="69191-111">Parent elements</span></span>

|<span data-ttu-id="69191-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="69191-112">**Element**</span></span>|<span data-ttu-id="69191-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="69191-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="69191-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="69191-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="69191-115">Содержит спецификации для подключения клиента к сервер адресной книги с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="69191-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="69191-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="69191-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="69191-117">Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="69191-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="69191-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="69191-118">Text value</span></span>

<span data-ttu-id="69191-119">Текстовое значение представляет URL-адрес, который можно использовать для доступа к сервер адресной книги или почтового ящика пользователя из внутренней организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="69191-119">The text value represents a URL that can be used to access an address book server or user's mailbox from inside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="69191-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="69191-120">Remarks</span></span>

<span data-ttu-id="69191-121">Элемент **InternalUrl** могут быть представлены в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp».</span><span class="sxs-lookup"><span data-stu-id="69191-121">The **InternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="69191-122">Элемент **InternalUrl** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1) .</span><span class="sxs-lookup"><span data-stu-id="69191-122">The **InternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="69191-123">См. также</span><span class="sxs-lookup"><span data-stu-id="69191-123">See also</span></span>



[<span data-ttu-id="69191-124">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="69191-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

