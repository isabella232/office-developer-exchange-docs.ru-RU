---
title: Сервердн (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 2ef73d13-e8bb-43f6-96c7-3ee157fed739
description: Элемент Сервердн указывает различающееся имя компьютера, на котором работает Microsoft Exchange Server 2007.
ms.openlocfilehash: 16c6e7368e221b7e54c8d7d63532bb29464a7e54
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461998"
---
# <a name="serverdn-pox"></a><span data-ttu-id="49599-103">Сервердн (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-103">ServerDN (POX)</span></span>

<span data-ttu-id="49599-104">Элемент **сервердн** указывает различающееся имя компьютера, на котором работает Microsoft Exchange Server 2007.</span><span class="sxs-lookup"><span data-stu-id="49599-104">The **ServerDN** element specifies the distinguished name of the computer that is running Microsoft Exchange Server 2007.</span></span> 
  
[<span data-ttu-id="49599-105">Служба автообнаружения (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="49599-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="49599-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="49599-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="49599-109">Сервердн (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-109">ServerDN (POX)</span></span>](serverdn-pox.md)
  
```xml
<ServerDN/>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="49599-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="49599-110">Attributes and elements</span></span>

<span data-ttu-id="49599-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="49599-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49599-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="49599-112">Attributes</span></span>

<span data-ttu-id="49599-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49599-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="49599-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="49599-114">Child elements</span></span>

<span data-ttu-id="49599-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="49599-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="49599-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="49599-116">Parent elements</span></span>

|<span data-ttu-id="49599-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="49599-117">**Element**</span></span>|<span data-ttu-id="49599-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="49599-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49599-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="49599-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="49599-120">Содержит спецификации для подключения клиента к компьютеру, на котором работает Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="49599-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49599-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="49599-121">Text value</span></span>

<span data-ttu-id="49599-122">Текстовое значение представляет различающееся имя сервера Exchange.</span><span class="sxs-lookup"><span data-stu-id="49599-122">The text value represents the distinguished name of the Exchange server.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49599-123">Примечания</span><span class="sxs-lookup"><span data-stu-id="49599-123">Remarks</span></span>

<span data-ttu-id="49599-124">Значение **сервердн** используется только в том случае, если [тип (POX)](type-pox.md) равен курсу.</span><span class="sxs-lookup"><span data-stu-id="49599-124">The **ServerDN** value is only used when [Type (POX)](type-pox.md) is equal to EXCH.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="49599-125">См. также</span><span class="sxs-lookup"><span data-stu-id="49599-125">See also</span></span>



[<span data-ttu-id="49599-126">XML-элементы автообнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="49599-126">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

