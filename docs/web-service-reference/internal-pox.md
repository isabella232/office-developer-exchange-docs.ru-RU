---
title: Internal (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: Внутренний элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из сети Организации.
ms.openlocfilehash: 8164a018a11f9bae9c3abcbfebf6cf0694ca4183
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465599"
---
# <a name="internal-pox"></a><span data-ttu-id="7edd4-103">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-103">Internal (POX)</span></span>

<span data-ttu-id="7edd4-104">**Внутренний** элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из сети Организации.</span><span class="sxs-lookup"><span data-stu-id="7edd4-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="7edd4-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="7edd4-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="7edd4-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="7edd4-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="7edd4-109">Internal (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="7edd4-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7edd4-110">Attributes and elements</span></span>

<span data-ttu-id="7edd4-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="7edd4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7edd4-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7edd4-112">Attributes</span></span>

<span data-ttu-id="7edd4-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="7edd4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7edd4-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7edd4-114">Child elements</span></span>

|<span data-ttu-id="7edd4-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7edd4-115">**Element**</span></span>|<span data-ttu-id="7edd4-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7edd4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7edd4-117">Оваурл (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="7edd4-118">Описание URL-адреса и схемы проверки подлинности, которая используется для доступа к определенному компьютеру, на котором установлен сервер Microsoft Exchange Server с установленной ролью сервера клиентского доступа, на котором размещена служба Outlook Web Access.</span><span class="sxs-lookup"><span data-stu-id="7edd4-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="7edd4-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="7edd4-120">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7edd4-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="7edd4-121">Этот элемент **Protocol** содержит только два дочерних элемента: [тип (POX)](type-pox.md) , указывающий протокол подключения, и элемент [асурл (POX)](asurl-pox.md) , указав конечную точку EWS для веб-службы доступности.</span><span class="sxs-lookup"><span data-stu-id="7edd4-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7edd4-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7edd4-122">Parent elements</span></span>

|<span data-ttu-id="7edd4-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7edd4-123">**Element**</span></span>|<span data-ttu-id="7edd4-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7edd4-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7edd4-125">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="7edd4-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="7edd4-126">Содержит спецификации для подключения клиента к компьютеру, на котором установлен сервер Microsoft Exchange с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="7edd4-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7edd4-127">Примечания</span><span class="sxs-lookup"><span data-stu-id="7edd4-127">Remarks</span></span>

<span data-ttu-id="7edd4-128">**Внутренний** элемент — это необязательный дочерний элемент элемента **Protocol** .</span><span class="sxs-lookup"><span data-stu-id="7edd4-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="7edd4-129">См. также</span><span class="sxs-lookup"><span data-stu-id="7edd4-129">See also</span></span>



[<span data-ttu-id="7edd4-130">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="7edd4-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

