---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: Элемент ExternalUrl содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 603e2109e7b3c98acdd4cbc13df81ed9717630ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762512"
---
# <a name="externalurl-pox"></a><span data-ttu-id="1d260-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="1d260-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="1d260-104">Элемент **ExternalUrl** содержит URL-адрес для подключения клиента на сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1d260-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="1d260-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1d260-105">Attributes and elements</span></span>

<span data-ttu-id="1d260-106">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1d260-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d260-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1d260-107">Attributes</span></span>

<span data-ttu-id="1d260-108">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d260-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d260-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1d260-109">Child elements</span></span>

<span data-ttu-id="1d260-110">Нет.</span><span class="sxs-lookup"><span data-stu-id="1d260-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1d260-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1d260-111">Parent elements</span></span>

|<span data-ttu-id="1d260-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1d260-112">**Element**</span></span>|<span data-ttu-id="1d260-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1d260-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d260-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="1d260-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="1d260-115">Содержит спецификации для подключения клиента к сервер адресной книги с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1d260-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="1d260-116">MailStore (POX)</span><span class="sxs-lookup"><span data-stu-id="1d260-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="1d260-117">Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="1d260-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1d260-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1d260-118">Text value</span></span>

<span data-ttu-id="1d260-119">Текстовое значение представляет URL-адрес, который можно использовать для доступа к сервер адресной книги или почтового ящика пользователя из за пределами организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="1d260-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1d260-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="1d260-120">Remarks</span></span>

<span data-ttu-id="1d260-121">Элемент **ExternalUrl** могут быть представлены в соответствии с элементом [Протокола (POX)](protocol-pox.md) со значением атрибута **типа** «mapiHttp».</span><span class="sxs-lookup"><span data-stu-id="1d260-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="1d260-122">Элемент **ExternalUrl** доступен для клиентов, использующих протокол MAPI/HTTP и конечного Exchange Online, Exchange Online в составе Office 365 и локальной версии Exchange, начиная с построения 15.00.0847.032 (Exchange Server 2013 с пакетом обновления 1) .</span><span class="sxs-lookup"><span data-stu-id="1d260-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="1d260-123">См. также</span><span class="sxs-lookup"><span data-stu-id="1d260-123">See also</span></span>



[<span data-ttu-id="1d260-124">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="1d260-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

