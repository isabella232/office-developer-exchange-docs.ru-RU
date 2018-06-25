---
title: Внутренний (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 69c22546-ebd6-4a03-b0b4-bbac72ec5551
description: Внутренний элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из внутри сети организации.
ms.openlocfilehash: 0dc5b679af98b52f15ef3b40181c2d97f102f373
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833946"
---
# <a name="internal-pox"></a><span data-ttu-id="8151f-103">Внутренний (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-103">Internal (POX)</span></span>

<span data-ttu-id="8151f-104">**Внутренний** элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из внутри сети организации.</span><span class="sxs-lookup"><span data-stu-id="8151f-104">The **Internal** element contains the collection of URLs that a client can use to connect to Exchange from inside the organization's network.</span></span> 
  
[<span data-ttu-id="8151f-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="8151f-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="8151f-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="8151f-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="8151f-109">Внутренний (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-109">Internal (POX)</span></span>](internal-pox.md)
  
```xml
<Internal>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</Internal>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8151f-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8151f-110">Attributes and elements</span></span>

<span data-ttu-id="8151f-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8151f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8151f-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8151f-112">Attributes</span></span>

<span data-ttu-id="8151f-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="8151f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8151f-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8151f-114">Child elements</span></span>

|<span data-ttu-id="8151f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8151f-115">**Element**</span></span>|<span data-ttu-id="8151f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8151f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8151f-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="8151f-118">Описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.</span><span class="sxs-lookup"><span data-stu-id="8151f-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="8151f-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8151f-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8151f-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="8151f-121">Этот элемент **протокола** имеет только два дочерних элементов: [Тип (POX)](type-pox.md) элемент, указывающий протокол подключения и элемент управления [ASUrl (POX)](asurl-pox.md) , определяющее конечной точки веб-служб Exchange для обеспечения доступности веб-службы.</span><span class="sxs-lookup"><span data-stu-id="8151f-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8151f-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8151f-122">Parent elements</span></span>

|<span data-ttu-id="8151f-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8151f-123">**Element**</span></span>|<span data-ttu-id="8151f-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8151f-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8151f-125">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8151f-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8151f-126">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8151f-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8151f-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="8151f-127">Remarks</span></span>

<span data-ttu-id="8151f-128">**Внутренний** элемент является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="8151f-128">The **Internal** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="8151f-129">См. также</span><span class="sxs-lookup"><span data-stu-id="8151f-129">See also</span></span>



[<span data-ttu-id="8151f-130">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="8151f-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

