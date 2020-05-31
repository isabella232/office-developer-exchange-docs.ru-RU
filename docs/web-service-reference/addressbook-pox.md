---
title: AddressBook (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: b2d62fd0-741c-4a41-9762-cc7d0ff01c9c
description: Элемент AddressBook содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.
ms.openlocfilehash: c30f0ee7c36de7e63157d07d003a11187d661fd7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761353"
---
# <a name="addressbook-pox"></a><span data-ttu-id="cd750-103">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-103">AddressBook (POX)</span></span>

<span data-ttu-id="cd750-104">Элемент **addressBook** содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="cd750-104">The **AddressBook** element contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span> 
  
[<span data-ttu-id="cd750-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="cd750-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="cd750-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="cd750-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="cd750-109">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-109">AddressBook (POX)</span></span>](addressbook-pox.md)
  
```XML
<AddressBook>
   <ExternalUrl/>
   <InternalUrl/>
</AddressBook>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="cd750-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="cd750-110">Attributes and elements</span></span>

<span data-ttu-id="cd750-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="cd750-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cd750-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="cd750-112">Attributes</span></span>

<span data-ttu-id="cd750-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="cd750-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cd750-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="cd750-114">Child elements</span></span>

|<span data-ttu-id="cd750-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd750-115">**Element**</span></span>|<span data-ttu-id="cd750-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd750-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd750-117">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-117">ExternalUrl (POX)</span></span>](externalurl-pox.md) <br/> |<span data-ttu-id="cd750-118">Содержит URL-адрес, который должен использоваться для доступа к адресной книге извне сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="cd750-118">Contains the URL that should be used to access the address book from outside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="cd750-119">InternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-119">InternalUrl (POX)</span></span>](internalurl-pox.md) <br/> |<span data-ttu-id="cd750-120">Содержит URL-адрес, который должен использоваться для доступа к адресной книге из сети Организации с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="cd750-120">Contains the URL that should be used to access the address book from inside the organization's network by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cd750-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="cd750-121">Parent elements</span></span>

|<span data-ttu-id="cd750-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="cd750-122">**Element**</span></span>|<span data-ttu-id="cd750-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="cd750-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cd750-124">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="cd750-124">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="cd750-125">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="cd750-125">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cd750-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="cd750-126">Remarks</span></span>

<span data-ttu-id="cd750-127">Элемент **addressBook** присутствует в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно".</span><span class="sxs-lookup"><span data-stu-id="cd750-127">The **AddressBook** element is present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="cd750-128">Элемент **addressBook** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="cd750-128">The **AddressBook** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="cd750-129">См. также</span><span class="sxs-lookup"><span data-stu-id="cd750-129">See also</span></span>

- [<span data-ttu-id="cd750-130">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="cd750-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

