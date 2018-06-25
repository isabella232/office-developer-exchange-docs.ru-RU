---
title: Внешние (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8eed1f79-6eb3-4a88-80fb-d4edf9f34fda
description: Внешний элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из за пределами сети организации.
ms.openlocfilehash: 7f01fc29b5ce63b02de0a4a6e42887dcffbb4b82
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762474"
---
# <a name="external-pox"></a><span data-ttu-id="a17a6-103">Внешние (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-103">External (POX)</span></span>

<span data-ttu-id="a17a6-104">**Внешний** элемент содержит коллекцию URL-адресов, которые клиент может использовать для подключения к Exchange из за пределами сети организации.</span><span class="sxs-lookup"><span data-stu-id="a17a6-104">The **External** element contains a collection of URLs that a client can use to connect to Exchange from outside of the organization's network.</span></span> 
  
[<span data-ttu-id="a17a6-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="a17a6-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="a17a6-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="a17a6-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="a17a6-109">Внешние (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-109">External (POX)</span></span>](external-pox.md)
  
```XML
<External>
   <OWAUrl/>
   <Protocol>
      <Type/>
      <ASUrl/>
   </Protocol>
</External>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="a17a6-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a17a6-110">Attributes and elements</span></span>

<span data-ttu-id="a17a6-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a17a6-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a17a6-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a17a6-112">Attributes</span></span>

<span data-ttu-id="a17a6-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a17a6-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a17a6-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a17a6-114">Child elements</span></span>

|<span data-ttu-id="a17a6-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a17a6-115">**Element**</span></span>|<span data-ttu-id="a17a6-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a17a6-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a17a6-117">OWAUrl (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-117">OWAUrl (POX)</span></span>](owaurl-pox.md) <br/> |<span data-ttu-id="a17a6-118">Описывает URL-адрес и схемы проверки подлинности, используемый для доступа к на конкретном компьютере, на котором выполняется Microsoft Exchange Server, который имеет роль сервера клиентского доступа установлен, на котором размещается веб-клиент Outlook.</span><span class="sxs-lookup"><span data-stu-id="a17a6-118">Describes the URL and authentication schema that is used to access a particular computer that is running Microsoft Exchange Server that has the Client Access server role installed that hosts Outlook Web Access.</span></span>  <br/> |
|[<span data-ttu-id="a17a6-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a17a6-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a17a6-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span> <span data-ttu-id="a17a6-121">Этот элемент **протокола** имеет только два дочерних элементов: [Тип (POX)](type-pox.md) элемент, указывающий протокол подключения и элемент управления [ASUrl (POX)](asurl-pox.md) , определяющее конечной точки веб-служб Exchange для обеспечения доступности веб-службы.</span><span class="sxs-lookup"><span data-stu-id="a17a6-121">This **Protocol** element has only two child elements: a [Type (POX)](type-pox.md) element specifying the connection protocol, and an [ASUrl (POX)](asurl-pox.md) element, specifying the EWS endpoint for the Availability web service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a17a6-122">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a17a6-122">Parent elements</span></span>

|<span data-ttu-id="a17a6-123">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a17a6-123">**Element**</span></span>|<span data-ttu-id="a17a6-124">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a17a6-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a17a6-125">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="a17a6-125">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="a17a6-126">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a17a6-126">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a17a6-127">Замечания</span><span class="sxs-lookup"><span data-stu-id="a17a6-127">Remarks</span></span>

<span data-ttu-id="a17a6-128">**Внешний** элемент является необязательным дочерним элементом элемента **протокола** .</span><span class="sxs-lookup"><span data-stu-id="a17a6-128">The **External** element is an optional child element of the **Protocol** element.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a17a6-129">См. также</span><span class="sxs-lookup"><span data-stu-id="a17a6-129">See also</span></span>



[<span data-ttu-id="a17a6-130">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="a17a6-130">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

