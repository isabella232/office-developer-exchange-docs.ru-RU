---
title: Токениссуер (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: Элемент Токениссуер указывает URI (SOAP) и конечную точку (SOAP) для службы маркеров безопасности.
ms.openlocfilehash: 1c267fc6cbfdadd471c568473cc9aeeafb43ae2d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19840196"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="d6b59-103">Токениссуер (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6b59-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="d6b59-104">Элемент **токениссуер** указывает [URI (SOAP)](uri-soap.md) и [конечную точку (SOAP)](endpoint-soap.md) для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="d6b59-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="d6b59-105">**токениссуер**</span><span class="sxs-lookup"><span data-stu-id="d6b59-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d6b59-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d6b59-106">Attributes and elements</span></span>

<span data-ttu-id="d6b59-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d6b59-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d6b59-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d6b59-108">Attributes</span></span>

<span data-ttu-id="d6b59-109">Нет</span><span class="sxs-lookup"><span data-stu-id="d6b59-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d6b59-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d6b59-110">Child elements</span></span>

|<span data-ttu-id="d6b59-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6b59-111">**Element**</span></span>|<span data-ttu-id="d6b59-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6b59-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6b59-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6b59-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="d6b59-114">Универсальный код ресурса (URI) службы маркеров безопасности, который выдал маркер безопасности.</span><span class="sxs-lookup"><span data-stu-id="d6b59-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="d6b59-115">Конечная точка (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6b59-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="d6b59-116">URI конечной точки веб-службы.</span><span class="sxs-lookup"><span data-stu-id="d6b59-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d6b59-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d6b59-117">Parent elements</span></span>

|<span data-ttu-id="d6b59-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d6b59-118">**Element**</span></span>|<span data-ttu-id="d6b59-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d6b59-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d6b59-120">Токениссуерс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d6b59-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="d6b59-121">Представляет коллекцию URI-кодов службы маркеров безопасности [(SOAP)](uri-soap.md) и [КОНЕЧНОЙ точки (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="d6b59-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d6b59-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="d6b59-122">Remarks</span></span>

<span data-ttu-id="d6b59-123">Используйте элемент **токениссуер** для указания службы маркеров безопасности при использовании маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="d6b59-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d6b59-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d6b59-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d6b59-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d6b59-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d6b59-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d6b59-126">Schema Name</span></span>  <br/> |<span data-ttu-id="d6b59-127">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="d6b59-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d6b59-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d6b59-128">Validation File</span></span>  <br/> |<span data-ttu-id="d6b59-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d6b59-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d6b59-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d6b59-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="d6b59-131">True</span><span class="sxs-lookup"><span data-stu-id="d6b59-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d6b59-132">См. также</span><span class="sxs-lookup"><span data-stu-id="d6b59-132">See also</span></span>



[<span data-ttu-id="d6b59-133">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="d6b59-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="d6b59-134">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="d6b59-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

