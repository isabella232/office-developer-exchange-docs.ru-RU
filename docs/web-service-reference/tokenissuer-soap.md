---
title: Токениссуер (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2d7be675-626c-4173-89e9-e32beef81ad5
description: Элемент Токениссуер указывает URI (SOAP) и конечную точку (SOAP) для службы маркеров безопасности.
ms.openlocfilehash: e9c0b4140de26c7ff05daf4e863b3e8a17fedc62
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526328"
---
# <a name="tokenissuer-soap"></a><span data-ttu-id="34a10-103">Токениссуер (SOAP)</span><span class="sxs-lookup"><span data-stu-id="34a10-103">TokenIssuer (SOAP)</span></span>

<span data-ttu-id="34a10-104">Элемент **токениссуер** указывает [URI (SOAP)](uri-soap.md) и [конечную точку (SOAP)](endpoint-soap.md) для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="34a10-104">The **TokenIssuer** element specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span> 
  
```XML
<TokenIssuer>
   <Uri/>
   <Endpoint/>
</TokenIssuer>
```

 <span data-ttu-id="34a10-105">**токениссуер**</span><span class="sxs-lookup"><span data-stu-id="34a10-105">**TokenIssuer**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34a10-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="34a10-106">Attributes and elements</span></span>

<span data-ttu-id="34a10-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="34a10-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34a10-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="34a10-108">Attributes</span></span>

<span data-ttu-id="34a10-109">Нет</span><span class="sxs-lookup"><span data-stu-id="34a10-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="34a10-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="34a10-110">Child elements</span></span>

|<span data-ttu-id="34a10-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="34a10-111">**Element**</span></span>|<span data-ttu-id="34a10-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="34a10-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34a10-113">URI (SOAP)</span><span class="sxs-lookup"><span data-stu-id="34a10-113">Uri (SOAP)</span></span>](uri-soap.md) <br/> |<span data-ttu-id="34a10-114">Универсальный код ресурса (URI) службы маркеров безопасности, который выдал маркер безопасности.</span><span class="sxs-lookup"><span data-stu-id="34a10-114">The URI of the security token service that issued the security token.</span></span>  <br/> |
|[<span data-ttu-id="34a10-115">Конечная точка (SOAP)</span><span class="sxs-lookup"><span data-stu-id="34a10-115">Endpoint (SOAP)</span></span>](endpoint-soap.md) <br/> |<span data-ttu-id="34a10-116">URI конечной точки веб-службы.</span><span class="sxs-lookup"><span data-stu-id="34a10-116">The web service Endpoint URI.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34a10-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="34a10-117">Parent elements</span></span>

|<span data-ttu-id="34a10-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="34a10-118">**Element**</span></span>|<span data-ttu-id="34a10-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="34a10-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34a10-120">Токениссуерс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="34a10-120">TokenIssuers (SOAP)</span></span>](tokenissuers-soap.md) <br/> |<span data-ttu-id="34a10-121">Представляет коллекцию URI-кодов службы маркеров безопасности [(SOAP)](uri-soap.md) и [КОНЕЧНОЙ точки (SOAP)](endpoint-soap.md).</span><span class="sxs-lookup"><span data-stu-id="34a10-121">Represents a collection of security token service [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md).</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34a10-122">Примечания</span><span class="sxs-lookup"><span data-stu-id="34a10-122">Remarks</span></span>

<span data-ttu-id="34a10-123">Используйте элемент **токениссуер** для указания службы маркеров безопасности при использовании маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="34a10-123">Use the **TokenIssuer** element to specify the security token service when using security tokens.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="34a10-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="34a10-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34a10-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="34a10-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="34a10-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="34a10-126">Schema Name</span></span>  <br/> |<span data-ttu-id="34a10-127">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="34a10-127">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="34a10-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="34a10-128">Validation File</span></span>  <br/> |<span data-ttu-id="34a10-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="34a10-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34a10-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="34a10-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="34a10-131">True</span><span class="sxs-lookup"><span data-stu-id="34a10-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34a10-132">См. также</span><span class="sxs-lookup"><span data-stu-id="34a10-132">See also</span></span>



[<span data-ttu-id="34a10-133">Справочные материалы по веб-службе автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="34a10-133">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="34a10-134">XML-элементы автообнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="34a10-134">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

