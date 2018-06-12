---
title: TokenIssuer (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: Элемент TokenIssuer указывает Uri (SOAP) и конечной точки (SOAP) для службы маркеров безопасности.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840196"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="58e2c-103">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58e2c-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="58e2c-104">Элемент **TokenIssuer** указывает [Uri (SOAP)](uri-soap.md) и [Конечной точки (SOAP)](endpoint-soap.md) для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="58e2c-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="58e2c-105">**TokenIssuer**</span><span class="sxs-lookup"><span data-stu-id="58e2c-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58e2c-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="58e2c-106">Attributes and elements</span></span>

<span data-ttu-id="58e2c-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="58e2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58e2c-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="58e2c-108">Attributes</span></span>

<span data-ttu-id="58e2c-109">Нет</span><span class="sxs-lookup"><span data-stu-id="58e2c-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58e2c-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="58e2c-110">Child elements</span></span>

|<span data-ttu-id="58e2c-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e2c-111">**Element**</span></span>|<span data-ttu-id="58e2c-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e2c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e2c-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58e2c-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="58e2c-114">URI службы маркеров безопасности, выдавшей маркер безопасности.</span><span class="sxs-lookup"><span data-stu-id="58e2c-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="58e2c-115">Конечная точка (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58e2c-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="58e2c-116">URI конечной точки веб-службы.</span><span class="sxs-lookup"><span data-stu-id="58e2c-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58e2c-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="58e2c-117">Parent elements</span></span>

|<span data-ttu-id="58e2c-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="58e2c-118">**Element**</span></span>|<span data-ttu-id="58e2c-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="58e2c-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58e2c-120">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="58e2c-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="58e2c-121">Представляет коллекцию службы маркеров безопасности [Uri (SOAP)](uri-soap.md) и [Конечной точки (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="58e2c-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="58e2c-122">Замечания</span><span class="sxs-lookup"><span data-stu-id="58e2c-122">Remarks</span></span>

<span data-ttu-id="58e2c-123">Используйте элемент **TokenIssuer** для указания службы маркеров безопасности при использовании маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="58e2c-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="58e2c-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="58e2c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58e2c-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="58e2c-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="58e2c-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="58e2c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="58e2c-127">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="58e2c-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="58e2c-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="58e2c-128">Validation File</span></span>  <br/> |<span data-ttu-id="58e2c-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="58e2c-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="58e2c-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="58e2c-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="58e2c-131">True</span><span class="sxs-lookup"><span data-stu-id="58e2c-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="58e2c-132">См. также</span><span class="sxs-lookup"><span data-stu-id="58e2c-132">See also</span></span>



[<span data-ttu-id="58e2c-133">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="58e2c-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="58e2c-134">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="58e2c-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

