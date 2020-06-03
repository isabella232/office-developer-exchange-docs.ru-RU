---
title: Домаинрекуиред (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 1f26b691-7331-4c7f-a92b-dfcc66c26963
description: Элемент Домаинрекуиред указывает, требуется ли домен для проверки подлинности.
ms.openlocfilehash: 97d602c40b247f9a6650cc4440b53bf23c18482e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461326"
---
# <a name="domainrequired-pox"></a><span data-ttu-id="9cb3a-103">Домаинрекуиред (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-103">DomainRequired (POX)</span></span>

<span data-ttu-id="9cb3a-104">Элемент **домаинрекуиред** указывает, требуется ли домен для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-104">The **DomainRequired** element indicates whether the domain is required for authentication.</span></span> 
  
- [<span data-ttu-id="9cb3a-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="9cb3a-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-106">Response (POX)</span></span>](response-pox.md) 
- [<span data-ttu-id="9cb3a-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-107">Account (POX)</span></span>](account-pox.md)  
- [<span data-ttu-id="9cb3a-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-108">Protocol (POX)</span></span>](protocol-pox.md)  
- [<span data-ttu-id="9cb3a-109">Домаинрекуиред (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-109">DomainRequired (POX)</span></span>](domainrequired-pox.md)
  
```xml
<DomainRequired>on or off</DomainRequired>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="9cb3a-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="9cb3a-110">Attributes and elements</span></span>

<span data-ttu-id="9cb3a-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cb3a-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="9cb3a-112">Attributes</span></span>

<span data-ttu-id="9cb3a-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cb3a-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="9cb3a-114">Child elements</span></span>

<span data-ttu-id="9cb3a-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cb3a-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="9cb3a-116">Parent elements</span></span>

|<span data-ttu-id="9cb3a-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="9cb3a-117">**Element**</span></span>|<span data-ttu-id="9cb3a-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="9cb3a-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cb3a-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="9cb3a-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="9cb3a-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cb3a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="9cb3a-121">Text value</span></span>

<span data-ttu-id="9cb3a-122">Текстовое значение указывает, требуется ли домен для проверки подлинности.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-122">The text value indicates whether the domain is required for authentication.</span></span> <span data-ttu-id="9cb3a-123">Возможные **значения:** **On и on** .</span><span class="sxs-lookup"><span data-stu-id="9cb3a-123">The possible values are **on** and **off**.</span></span> <span data-ttu-id="9cb3a-124">Если значение равно **On**, то следующий запрос должен содержать домен учетной записи пользователя.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-124">If the value is **on**, the subsequent request must contain the domain of the user's account.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9cb3a-125">Примечания</span><span class="sxs-lookup"><span data-stu-id="9cb3a-125">Remarks</span></span>

<span data-ttu-id="9cb3a-126">Если домен не указан в элементе [LoginName (POX)](loginname-pox.md) или элемент **LoginName** не был указан, пользователь должен ввести домен, прежде чем проверка подлинности будет выполнена.</span><span class="sxs-lookup"><span data-stu-id="9cb3a-126">If the domain is not specified in the [LoginName (POX)](loginname-pox.md) element, or the **LoginName** element was not specified, the user must enter the domain before authentication will succeed.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="9cb3a-127">См. также</span><span class="sxs-lookup"><span data-stu-id="9cb3a-127">See also</span></span>

- [<span data-ttu-id="9cb3a-128">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="9cb3a-128">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

