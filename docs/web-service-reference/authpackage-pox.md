---
title: AuthPackage (POX)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 709dbe53-6141-41f8-a2b9-a399bae47991
description: Элемент AuthPackage указывает схемы проверки подлинности, используемый при проверке подлинности на сервере Exchange, с установленной ролью сервера почтовых ящиков.
ms.openlocfilehash: 120ec00ac82166ae2002a8fbac0edf9a1e23afc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761526"
---
# <a name="authpackage-pox"></a><span data-ttu-id="aa716-103">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-103">AuthPackage (POX)</span></span>

<span data-ttu-id="aa716-104">Элемент **AuthPackage** указывает схемы проверки подлинности, используемый при проверке подлинности на сервере Exchange, с установленной ролью сервера почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="aa716-104">The **AuthPackage** element specifies the authentication scheme that is used when authenticating against the Exchange server that has the Mailbox server role installed.</span></span> 
  
- [<span data-ttu-id="aa716-105">Автообнаружение (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
- [<span data-ttu-id="aa716-106">Ответ (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-106">Response (POX)</span></span>](response-pox.md)
  
- [<span data-ttu-id="aa716-107">Учетная запись (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-107">Account (POX)</span></span>](account-pox.md)
  
- [<span data-ttu-id="aa716-108">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-108">Protocol (POX)</span></span>](protocol-pox.md)
  
- [<span data-ttu-id="aa716-109">AuthPackage (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-109">AuthPackage (POX)</span></span>](authpackage-pox.md)
  
```xml
<AuthPackage>basic or kerb or kerbntlm or ntlm or certificate or negotiate or nego2</AuthPackage>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="aa716-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aa716-110">Attributes and elements</span></span>

<span data-ttu-id="aa716-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="aa716-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa716-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aa716-112">Attributes</span></span>

<span data-ttu-id="aa716-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa716-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa716-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aa716-114">Child elements</span></span>

<span data-ttu-id="aa716-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="aa716-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa716-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aa716-116">Parent elements</span></span>

|<span data-ttu-id="aa716-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aa716-117">**Element**</span></span>|<span data-ttu-id="aa716-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aa716-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa716-119">Протокол (POX)</span><span class="sxs-lookup"><span data-stu-id="aa716-119">Protocol (POX)</span></span>](protocol-pox.md) <br/> |<span data-ttu-id="aa716-120">Содержит спецификации для подключения клиента к серверу клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aa716-120">Contains the specifications for connecting a client to the Client Access server.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa716-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="aa716-121">Text value</span></span>

<span data-ttu-id="aa716-122">Текстовое значение определяет схемы проверки подлинности, используемый при проверке подлинности на сервере почтовых ящиков.</span><span class="sxs-lookup"><span data-stu-id="aa716-122">The text value specifies the authentication scheme that is used when authenticating against the Mailbox server.</span></span> <span data-ttu-id="aa716-123">Ниже перечислены возможные значения.</span><span class="sxs-lookup"><span data-stu-id="aa716-123">The following are the possible values:</span></span>
  
- <span data-ttu-id="aa716-124">Базовая</span><span class="sxs-lookup"><span data-stu-id="aa716-124">basic</span></span>
- <span data-ttu-id="aa716-125">kerb</span><span class="sxs-lookup"><span data-stu-id="aa716-125">kerb</span></span>
- <span data-ttu-id="aa716-126">kerbntlm</span><span class="sxs-lookup"><span data-stu-id="aa716-126">kerbntlm</span></span>
- <span data-ttu-id="aa716-127">NTLM</span><span class="sxs-lookup"><span data-stu-id="aa716-127">ntlm</span></span>
- <span data-ttu-id="aa716-128">certificate</span><span class="sxs-lookup"><span data-stu-id="aa716-128">certificate</span></span>
- <span data-ttu-id="aa716-129">согласование</span><span class="sxs-lookup"><span data-stu-id="aa716-129">negotiate</span></span>
- <span data-ttu-id="aa716-130">протокол nego2</span><span class="sxs-lookup"><span data-stu-id="aa716-130">nego2</span></span>
    
## <a name="remarks"></a><span data-ttu-id="aa716-131">Замечания</span><span class="sxs-lookup"><span data-stu-id="aa716-131">Remarks</span></span>

<span data-ttu-id="aa716-132">Элемент **AuthPackage** используется только в том случае, когда элемент [Типа (POX)](type-pox.md) имеет значение text EXCH или EXPR.</span><span class="sxs-lookup"><span data-stu-id="aa716-132">The **AuthPackage** element is only used when the [Type (POX)](type-pox.md) element has a text value of EXCH or EXPR.</span></span> 
  
### <a name="version-differences"></a><span data-ttu-id="aa716-133">Различия версий</span><span class="sxs-lookup"><span data-stu-id="aa716-133">Version differences</span></span>

<span data-ttu-id="aa716-134">Office 365, Exchange Online и локальной версии Exchange, начиная с построения 15.00.0995.014 возвращаемое значение «согласование» только в том случае, если сервер настроен на использование проверки подлинности согласование и клиент включает в себя заголовок [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) , содержит «Согласование».</span><span class="sxs-lookup"><span data-stu-id="aa716-134">Office 365, Exchange Online, and on-premises versions of Exchange starting with build 15.00.0995.014 return a value of "negotiate" only if the server is configured to use Negotiate authentication and the client includes a [X-ClientCanHandle](pox-autodiscover-request-for-exchange.md) header that contains "Negotiate".</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="aa716-135">См. также</span><span class="sxs-lookup"><span data-stu-id="aa716-135">See also</span></span>

- [<span data-ttu-id="aa716-136">Элементы XML автоматического обнаружения POX для Exchange</span><span class="sxs-lookup"><span data-stu-id="aa716-136">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

