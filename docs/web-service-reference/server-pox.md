---
title: Сервер (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 0ce51644-7f3a-408c-a398-814439b658dc
description: Элемент Server указывает имя почтового сервера.
ms.openlocfilehash: 6b29b153bc75b8836bfa113e126d122d620c2984
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462012"
---
# <a name="server-pox"></a><span data-ttu-id="d086c-103">Сервер (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-103">Server (POX)</span></span>

<span data-ttu-id="d086c-104">Элемент **Server** указывает имя почтового сервера.</span><span class="sxs-lookup"><span data-stu-id="d086c-104">The **Server** element specifies the name of the mail server.</span></span> 
  
[<span data-ttu-id="d086c-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="d086c-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="d086c-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="d086c-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="d086c-109">Сервер (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-109">Server (POX)</span></span>](server-pox.md)
  
```xml
<Server/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="d086c-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d086c-110">Attributes and elements</span></span>

<span data-ttu-id="d086c-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d086c-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d086c-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d086c-112">Attributes</span></span>

<span data-ttu-id="d086c-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d086c-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d086c-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d086c-114">Child elements</span></span>

<span data-ttu-id="d086c-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d086c-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d086c-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d086c-116">Parent elements</span></span>

|<span data-ttu-id="d086c-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d086c-117">**Element**</span></span>|<span data-ttu-id="d086c-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d086c-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d086c-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="d086c-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="d086c-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d086c-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d086c-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d086c-121">Text value</span></span>

<span data-ttu-id="d086c-122">Текстовое значение идентифицирует сервер.</span><span class="sxs-lookup"><span data-stu-id="d086c-122">The text value identifies the server.</span></span> <span data-ttu-id="d086c-123">Для таких протоколов, как POP3, SMTP, IMAP или NNTP, это значение будет либо именем узла, либо IP-адресом.</span><span class="sxs-lookup"><span data-stu-id="d086c-123">For protocols such as POP3, SMTP, IMAP, or NNTP, this value will be either a host name or an IP address.</span></span> <span data-ttu-id="d086c-124">Для таких протоколов, как DAV или Интернет, это будет URL-адрес.</span><span class="sxs-lookup"><span data-stu-id="d086c-124">For protocols such as DAV or WEB, this will be a URL.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d086c-125">См. также</span><span class="sxs-lookup"><span data-stu-id="d086c-125">See also</span></span>



[<span data-ttu-id="d086c-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="d086c-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

