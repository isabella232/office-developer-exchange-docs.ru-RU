---
title: SSL (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a7e2bdcd-a2f7-45a4-adcd-a03fe7fd4d9b
description: Элемент SSL указывает, требуется ли безопасный вход в систему.
ms.openlocfilehash: 9a51c715032cb2af846e764d28698c5697670d98
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835537"
---
# <a name="ssl-pox"></a><span data-ttu-id="e8bd3-103">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-103">SSL (POX)</span></span>

<span data-ttu-id="e8bd3-104">Элемент **SSL** указывает, требуется ли безопасный вход в систему.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-104">The **SSL** element specifies whether secure logon is required.</span></span> 
  
[<span data-ttu-id="e8bd3-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="e8bd3-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="e8bd3-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="e8bd3-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="e8bd3-109">SSL (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-109">SSL (POX)</span></span>](ssl-pox.md)
  
```xml
<SSL>on or off</SSL>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="e8bd3-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="e8bd3-110">Attributes and elements</span></span>

<span data-ttu-id="e8bd3-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8bd3-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="e8bd3-112">Attributes</span></span>

<span data-ttu-id="e8bd3-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8bd3-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="e8bd3-114">Child elements</span></span>

<span data-ttu-id="e8bd3-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8bd3-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="e8bd3-116">Parent elements</span></span>

|<span data-ttu-id="e8bd3-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="e8bd3-117">**Element**</span></span>|<span data-ttu-id="e8bd3-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="e8bd3-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8bd3-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="e8bd3-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="e8bd3-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8bd3-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="e8bd3-121">Text value</span></span>

<span data-ttu-id="e8bd3-122">Текстовое значение указывает, требуется ли безопасный вход в систему.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-122">The text value specifies whether secure logon is required.</span></span> <span data-ttu-id="e8bd3-123">Если значение не указано, по умолчанию устанавливается значение **On**.</span><span class="sxs-lookup"><span data-stu-id="e8bd3-123">If unspecified, the default value is set to **on**.</span></span> <span data-ttu-id="e8bd3-124">Возможные **значения:** **On и on** .</span><span class="sxs-lookup"><span data-stu-id="e8bd3-124">The possible values are **on** and **off**.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="e8bd3-125">См. также</span><span class="sxs-lookup"><span data-stu-id="e8bd3-125">See also</span></span>



[<span data-ttu-id="e8bd3-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="e8bd3-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

