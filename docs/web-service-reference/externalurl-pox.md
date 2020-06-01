---
title: ExternalUrl (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 3b647d88-6feb-40d7-9299-b2ca47b707db
description: Элемент ExternalUrl содержит URL-адрес для подключения клиента к серверу адресной книги или почтового ящика пользователя извне организации пользователя с помощью протокола MAPI/HTTP.
ms.openlocfilehash: 94265051be68ed06d1dab8d46dd4ce29d8694c93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457958"
---
# <a name="externalurl-pox"></a><span data-ttu-id="653cc-103">ExternalUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="653cc-103">ExternalUrl (POX)</span></span>

<span data-ttu-id="653cc-104">Элемент **ExternalURL** содержит URL-адрес для подключения клиента к серверу адресной книги или почтового ящика пользователя извне организации пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="653cc-104">The **ExternalUrl** element contains the URL for connecting a client to the address book server or a user's mailbox from outside the user's organization by using the MAPI/HTTP protocol.</span></span> 
  
```XML
<ExternalUrl/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="653cc-105">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="653cc-105">Attributes and elements</span></span>

<span data-ttu-id="653cc-106">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="653cc-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="653cc-107">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="653cc-107">Attributes</span></span>

<span data-ttu-id="653cc-108">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="653cc-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="653cc-109">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="653cc-109">Child elements</span></span>

<span data-ttu-id="653cc-110">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="653cc-110">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="653cc-111">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="653cc-111">Parent elements</span></span>

|<span data-ttu-id="653cc-112">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="653cc-112">**Element**</span></span>|<span data-ttu-id="653cc-113">**Описание**</span><span class="sxs-lookup"><span data-stu-id="653cc-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="653cc-114">AddressBook (POX)</span><span class="sxs-lookup"><span data-stu-id="653cc-114">AddressBook (POX)</span></span>](addressbook-pox.md) <br/> |<span data-ttu-id="653cc-115">Содержит спецификации для подключения клиента к серверу адресной книги с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="653cc-115">Contains the specifications for connecting a client to the address book server by using the MAPI/HTTP protocol.</span></span>  <br/> |
|[<span data-ttu-id="653cc-116">Маилсторе (POX)</span><span class="sxs-lookup"><span data-stu-id="653cc-116">MailStore (POX)</span></span>](mailstore-pox.md) <br/> |<span data-ttu-id="653cc-117">Содержит спецификации для подключения клиента к почтовому ящику пользователя с помощью протокола MAPI/HTTP.</span><span class="sxs-lookup"><span data-stu-id="653cc-117">Contains the specifications for connecting a client to the user's mailbox by using the MAPI/HTTP protocol.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="653cc-118">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="653cc-118">Text value</span></span>

<span data-ttu-id="653cc-119">Текстовое значение представляет собой URL-адрес, который можно использовать для доступа к серверу адресной книги или почтовому ящику пользователя извне организации пользователя.</span><span class="sxs-lookup"><span data-stu-id="653cc-119">The text value represents a URL that can be used to access an address book server or user's mailbox from outside the user's organization.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="653cc-120">Примечания</span><span class="sxs-lookup"><span data-stu-id="653cc-120">Remarks</span></span>

<span data-ttu-id="653cc-121">Элемент **ExternalURL** может присутствовать в отклике, у которого есть элемент [Protocol (POX)](protocol-pox.md) со значением атрибута **Type** "возможно".</span><span class="sxs-lookup"><span data-stu-id="653cc-121">The **ExternalUrl** element can be present in a response that has a [Protocol (POX)](protocol-pox.md) element with a **Type** attribute value of "mapiHttp".</span></span> 
  
<span data-ttu-id="653cc-122">Элемент **ExternalURL** доступен для клиентов, которые реализуют протокол MAPI/HTTP и целевую среду Exchange Online, Exchange Online в составе Office 365, а локальные версии Exchange, начиная с сборки 15.00.0847.032 (Exchange Server 2013 SP1).</span><span class="sxs-lookup"><span data-stu-id="653cc-122">The **ExternalUrl** element is available to clients that implement the MAPI/HTTP protocol and target Exchange Online, Exchange Online as part of Office 365, and on-premises versions of Exchange starting with build 15.00.0847.032 (Exchange Server 2013 SP1).</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="653cc-123">См. также</span><span class="sxs-lookup"><span data-stu-id="653cc-123">See also</span></span>



[<span data-ttu-id="653cc-124">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="653cc-124">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

