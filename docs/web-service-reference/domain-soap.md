---
title: Домен (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 849629a0-0467-422f-88f6-3b8a95c17bba
description: Элемент domain содержит федеративный домен в ответе Жетфедератионинформатион или содержит домен, параметры конфигурации которого запрашиваются в запросе Жетдомаинсеттингс.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762203"
---
# <a name="domain-soap"></a><span data-ttu-id="d88e5-103">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d88e5-103">Domain (SOAP)</span></span>

<span data-ttu-id="d88e5-104">Элемент **domain** содержит федеративный домен в ответе **жетфедератионинформатион** или содержит домен, параметры конфигурации которого запрашиваются в запросе **жетдомаинсеттингс** .</span><span class="sxs-lookup"><span data-stu-id="d88e5-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="d88e5-105">**строка**</span><span class="sxs-lookup"><span data-stu-id="d88e5-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d88e5-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d88e5-106">Attributes and elements</span></span>

<span data-ttu-id="d88e5-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d88e5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d88e5-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d88e5-108">Attributes</span></span>

<span data-ttu-id="d88e5-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d88e5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d88e5-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d88e5-110">Child elements</span></span>

<span data-ttu-id="d88e5-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d88e5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d88e5-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d88e5-112">Parent elements</span></span>

|<span data-ttu-id="d88e5-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d88e5-113">**Element**</span></span>|<span data-ttu-id="d88e5-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d88e5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d88e5-115">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d88e5-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="d88e5-116">Представляет домены параметры конфигурации, которые возвращаются в операции **жетдомаинсеттингс** или в доменах, Федеративных в Организации в операции **жетфедератионинформатион** .</span><span class="sxs-lookup"><span data-stu-id="d88e5-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d88e5-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="d88e5-117">Text value</span></span>

<span data-ttu-id="d88e5-118">Текстовое значение элемента **domain** представляет доменное имя.</span><span class="sxs-lookup"><span data-stu-id="d88e5-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d88e5-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d88e5-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d88e5-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d88e5-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d88e5-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d88e5-121">Schema Name</span></span>  <br/> |<span data-ttu-id="d88e5-122">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="d88e5-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d88e5-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d88e5-123">Validation File</span></span>  <br/> |<span data-ttu-id="d88e5-124">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="d88e5-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d88e5-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d88e5-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="d88e5-126">True</span><span class="sxs-lookup"><span data-stu-id="d88e5-126">True</span></span>  <br/> |
   

