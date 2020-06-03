---
title: Имя_домена (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2b4af2b2-58b5-4f28-9cb3-c07a11377747
description: Элемент имя_домена указывает домен пользователя.
ms.openlocfilehash: ff38d6a876e396317dedece0a81a9f9f0db0f587
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458427"
---
# <a name="domainname-pox"></a><span data-ttu-id="8d8c4-103">Имя_домена (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-103">DomainName (POX)</span></span>

<span data-ttu-id="8d8c4-104">Элемент **имя_домена** указывает домен пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-104">The **DomainName** element specifies the user's domain.</span></span> 
  
- [<span data-ttu-id="8d8c4-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)  
- [<span data-ttu-id="8d8c4-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-106">Response (POX)</span></span>](response-pox.md)  
- [<span data-ttu-id="8d8c4-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-107">Account (POX)</span></span>](account-pox.md) 
- [<span data-ttu-id="8d8c4-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-108">Protocol (POX)</span></span>](protocol-pox.md) 
- [<span data-ttu-id="8d8c4-109">Имя_домена (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-109">DomainName (POX)</span></span>](domainname-pox.md)
  
```xml
<DomainName/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="8d8c4-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8d8c4-110">Attributes and elements</span></span>

<span data-ttu-id="8d8c4-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d8c4-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8d8c4-112">Attributes</span></span>

<span data-ttu-id="8d8c4-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d8c4-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8d8c4-114">Child elements</span></span>

<span data-ttu-id="8d8c4-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d8c4-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8d8c4-116">Parent elements</span></span>

|<span data-ttu-id="8d8c4-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8d8c4-117">**Element**</span></span>|<span data-ttu-id="8d8c4-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8d8c4-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d8c4-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="8d8c4-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="8d8c4-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d8c4-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8d8c4-121">Text value</span></span>

<span data-ttu-id="8d8c4-122">Текстовое значение указывает домен пользователя.</span><span class="sxs-lookup"><span data-stu-id="8d8c4-122">The text value specifies the user's domain.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d8c4-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="8d8c4-123">Remarks</span></span>

<span data-ttu-id="8d8c4-124">Если значение не указано, по умолчанию используется проверка подлинности в формате имени участника-пользователя (UPN).</span><span class="sxs-lookup"><span data-stu-id="8d8c4-124">If no value is specified, the default authentication is to use the e-mail address as a user principal name (UPN) format.</span></span> <span data-ttu-id="8d8c4-125">Пример: \<Username\> @ \<Domain\> .</span><span class="sxs-lookup"><span data-stu-id="8d8c4-125">For example: \<Username\>@\<Domain\>.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="8d8c4-126">См. также</span><span class="sxs-lookup"><span data-stu-id="8d8c4-126">See also</span></span>

- [<span data-ttu-id="8d8c4-127">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="8d8c4-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

