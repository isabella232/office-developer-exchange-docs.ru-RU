---
title: UsePOPAuth (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 28f552d8-6bb8-49b4-a45c-b2053670f1cc
description: Элемент UsePOPAuth указывает, будет ли сведения о проверке подлинности, который предоставляется для типа учетной записи POP3 также используется для SMTP Simple Mail Transfer Protocol ().
ms.openlocfilehash: be03568d697b1f5461d49dba388a1d3f1008a67e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840404"
---
# <a name="usepopauth-pox"></a><span data-ttu-id="75c69-103">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-103">UsePOPAuth (POX)</span></span>

<span data-ttu-id="75c69-104">Элемент **UsePOPAuth** указывает, будет ли сведения о проверке подлинности, который предоставляется для типа учетной записи POP3 также используется для SMTP Simple Mail Transfer Protocol ().</span><span class="sxs-lookup"><span data-stu-id="75c69-104">The **UsePOPAuth** element indicates whether the authentication information that is provided for a POP3 type of account is also used for Simple Mail Transfer Protocol (SMTP).</span></span> 
  
[<span data-ttu-id="75c69-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="75c69-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="75c69-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="75c69-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-108">Protocol (POX)</span></span>](protocol-pox.md)
  
[<span data-ttu-id="75c69-109">UsePOPAuth (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-109">UsePOPAuth (POX)</span></span>](usepopauth-pox.md)
  
```xml
<UsePOPAuth>on or off</UsePOPAuth>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="75c69-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="75c69-110">Attributes and elements</span></span>

<span data-ttu-id="75c69-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="75c69-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75c69-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="75c69-112">Attributes</span></span>

<span data-ttu-id="75c69-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="75c69-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75c69-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="75c69-114">Child elements</span></span>

<span data-ttu-id="75c69-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="75c69-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="75c69-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="75c69-116">Parent elements</span></span>

|<span data-ttu-id="75c69-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="75c69-117">**Element**</span></span>|<span data-ttu-id="75c69-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="75c69-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75c69-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="75c69-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="75c69-120">Содержит спецификации для подключения клиентского компьютера, на котором выполняется Microsoft Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="75c69-120">Contains the specifications for connecting a client to the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75c69-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="75c69-121">Text value</span></span>

<span data-ttu-id="75c69-122">Текстовое значение указывает, используется ли также сведения о проверке подлинности, который предоставляется для типа учетной записи POP3 для SMTP.</span><span class="sxs-lookup"><span data-stu-id="75c69-122">The text value indicates whether the authentication information that is provided for a POP3 type of account is also used for SMTP.</span></span> <span data-ttu-id="75c69-123">Возможные значения: **и **отключает**** .</span><span class="sxs-lookup"><span data-stu-id="75c69-123">The possible values are **on** and **off**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75c69-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="75c69-124">Remarks</span></span>

<span data-ttu-id="75c69-125">Элемент **UsePOPAuth** используется только в том случае, если [Тип (POX)](type-pox.md) SMTP.</span><span class="sxs-lookup"><span data-stu-id="75c69-125">The **UsePOPAuth** element is only used when [Type (POX)](type-pox.md) is SMTP.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="75c69-126">См. также</span><span class="sxs-lookup"><span data-stu-id="75c69-126">See also</span></span>



[<span data-ttu-id="75c69-127">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="75c69-127">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

