---
title: TokenIssuers (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 26c55228-184e-4340-bd80-f86be56f3e7a
description: Элементы TokenIssuers представляет коллекцию TokenIssuer (SOAP).
ms.openlocfilehash: b070d85b32d5bce8461ac4e930329f237885bad7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840208"
---
# <a name="tokenissuers-soap"></a><span data-ttu-id="1b822-103">TokenIssuers (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b822-103">TokenIssuers (SOAP)</span></span>

<span data-ttu-id="1b822-104">Элементы **TokenIssuers** представляет коллекцию [TokenIssuer (SOAP)](tokenissuer-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1b822-104">The **TokenIssuers** elements represents the [TokenIssuer (SOAP)](tokenissuer-soap.md) collection.</span></span> 
  
```XML
<TokenIssuers>
    <TokenIssuer/>
</TokenIssuers>
```

 <span data-ttu-id="1b822-105">**TokenIssuers**</span><span class="sxs-lookup"><span data-stu-id="1b822-105">**TokenIssuers**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b822-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1b822-106">Attributes and elements</span></span>

<span data-ttu-id="1b822-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1b822-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b822-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1b822-108">Attributes</span></span>

<span data-ttu-id="1b822-109">Нет</span><span class="sxs-lookup"><span data-stu-id="1b822-109">None</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b822-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1b822-110">Child elements</span></span>

|<span data-ttu-id="1b822-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b822-111">**Element**</span></span>|<span data-ttu-id="1b822-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b822-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b822-113">TokenIssuer (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b822-113">TokenIssuer (SOAP)</span></span>](tokenissuer-soap.md) <br/> |<span data-ttu-id="1b822-114">Указывает [Uri (SOAP)](uri-soap.md) и [Конечной точки (SOAP)](endpoint-soap.md) для службы маркеров безопасности.</span><span class="sxs-lookup"><span data-stu-id="1b822-114">Specifies the [Uri (SOAP)](uri-soap.md) and [Endpoint (SOAP)](endpoint-soap.md) for the security token service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b822-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1b822-115">Parent elements</span></span>

|<span data-ttu-id="1b822-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1b822-116">**Element**</span></span>|<span data-ttu-id="1b822-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1b822-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b822-118">GetFederationInformationResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1b822-118">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md) <br/> |<span data-ttu-id="1b822-119">Содержит ответ [GetFederationInformation операции (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1b822-119">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b822-120">Замечания</span><span class="sxs-lookup"><span data-stu-id="1b822-120">Remarks</span></span>

<span data-ttu-id="1b822-121">**TokenIssuers** представляет коллекцию элементов [TokenIssuer (SOAP)](tokenissuer-soap.md) для использования в автоматического обнаружения.</span><span class="sxs-lookup"><span data-stu-id="1b822-121">The **TokenIssuers** represents a collection of [TokenIssuer (SOAP)](tokenissuer-soap.md) elements to be used in the Autodiscovery.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="1b822-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1b822-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b822-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1b822-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1b822-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1b822-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1b822-125">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1b822-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1b822-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1b822-126">Validation File</span></span>  <br/> |<span data-ttu-id="1b822-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b822-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b822-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1b822-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b822-129">True</span><span class="sxs-lookup"><span data-stu-id="1b822-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b822-130">См. также</span><span class="sxs-lookup"><span data-stu-id="1b822-130">See also</span></span>



[<span data-ttu-id="1b822-131">Ссылки веб-службу автообнаружения для Exchange</span><span class="sxs-lookup"><span data-stu-id="1b822-131">Autodiscover web service reference for Exchange</span></span>](autodiscover-web-service-reference-for-exchange.md)
  
[<span data-ttu-id="1b822-132">Элементы XML автоматического обнаружения SOAP для Exchange 2013</span><span class="sxs-lookup"><span data-stu-id="1b822-132">SOAP Autodiscover XML elements for Exchange 2013</span></span>](soap-autodiscover-xml-elements-for-exchange-2013.md)

