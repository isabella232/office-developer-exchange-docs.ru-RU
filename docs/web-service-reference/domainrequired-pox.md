---
title: DomainRequired (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: Элемент DomainRequired указывает, является ли домена для проверки подлинности требуется.
ms.openlocfilehash: f314b9d27d1b4ee472d249ec49af1a785ff9ac25
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762204"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="071c8-103">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-103">DomainRequired (POX)</span></span>

<span data-ttu-id="071c8-104">Элемент **DomainRequired** указывает, является ли домена для проверки подлинности требуется.</span><span class="sxs-lookup"><span data-stu-id="071c8-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="071c8-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="071c8-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="071c8-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="071c8-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="071c8-109">DomainRequired (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="071c8-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="071c8-110">Attributes and elements</span></span>

<span data-ttu-id="071c8-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="071c8-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="071c8-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="071c8-112">Attributes</span></span>

<span data-ttu-id="071c8-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="071c8-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="071c8-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="071c8-114">Child elements</span></span>

<span data-ttu-id="071c8-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="071c8-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="071c8-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="071c8-116">Parent elements</span></span>

|<span data-ttu-id="071c8-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="071c8-117">**Element**</span></span>|<span data-ttu-id="071c8-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="071c8-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="071c8-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="071c8-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="071c8-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="071c8-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="071c8-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="071c8-121">Text value</span></span>

<span data-ttu-id="071c8-122">Текстовое значение указывает, необходима ли домена для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="071c8-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="071c8-123">Возможные значения: **и **отключает**** .</span><span class="sxs-lookup"><span data-stu-id="071c8-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="071c8-124">Если значение **на**следующий запрос должен содержать домен учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="071c8-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="071c8-125">Замечания</span><span class="sxs-lookup"><span data-stu-id="071c8-125">Remarks</span></span>

<span data-ttu-id="071c8-126">Если домен не указан в элементе [LoginName (POX)](loginname-pox.md) или элемент **LoginName** не указан, пользователя необходимо ввести домен будет успешной проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="071c8-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="071c8-127">См. также</span><span class="sxs-lookup"><span data-stu-id="071c8-127">See also</span></span>

- [<span data-ttu-id="071c8-128">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="071c8-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

