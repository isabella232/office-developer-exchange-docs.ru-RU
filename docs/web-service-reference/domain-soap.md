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
description: Элемент домена содержит федеративного домена в ответ GetFederationInformation или домена, параметры конфигурации, для которого запрашивается в запросе GetDomainSettings.
ms.openlocfilehash: 411ca866800322ef06eeecc2ab92adc6f711917c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762203"
---
# <a name="domain-soap"></a><span data-ttu-id="38ece-103">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="38ece-103">Domain (SOAP)</span></span>

<span data-ttu-id="38ece-104">Элемент **домена** содержит федеративного домена в ответ **GetFederationInformation** или домена, параметры конфигурации, для которого запрашивается в запросе **GetDomainSettings** .</span><span class="sxs-lookup"><span data-stu-id="38ece-104">The **Domain** element contains a federated domain in a **GetFederationInformation** response or contains a domain the configuration settings for which are requested in a **GetDomainSettings** request.</span></span> 
  
```XML
<Domain/> 
```

 <span data-ttu-id="38ece-105">**string**</span><span class="sxs-lookup"><span data-stu-id="38ece-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="38ece-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="38ece-106">Attributes and elements</span></span>

<span data-ttu-id="38ece-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="38ece-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38ece-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="38ece-108">Attributes</span></span>

<span data-ttu-id="38ece-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="38ece-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="38ece-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="38ece-110">Child elements</span></span>

<span data-ttu-id="38ece-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="38ece-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="38ece-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="38ece-112">Parent elements</span></span>

|<span data-ttu-id="38ece-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="38ece-113">**Element**</span></span>|<span data-ttu-id="38ece-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="38ece-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38ece-115">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="38ece-115">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="38ece-116">Представляет доменов, параметры конфигурации, для которого возвращаются в ходе операции **GetDomainSettings** или домены, которые организации федеративных в **GetFederationInformation** операции.</span><span class="sxs-lookup"><span data-stu-id="38ece-116">Represents the domains the configuration settings for which are returned in a **GetDomainSettings** operation or the domains that the organization has federated in a **GetFederationInformation** operation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="38ece-117">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="38ece-117">Text value</span></span>

<span data-ttu-id="38ece-118">Текстовое значение элемента **домена** представляет имя домена.</span><span class="sxs-lookup"><span data-stu-id="38ece-118">The text value of the **Domain** element represents a domain name.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="38ece-119">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="38ece-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38ece-120">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="38ece-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="38ece-121">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="38ece-121">Schema Name</span></span>  <br/> |<span data-ttu-id="38ece-122">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="38ece-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="38ece-123">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="38ece-123">Validation File</span></span>  <br/> |<span data-ttu-id="38ece-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="38ece-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="38ece-125">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="38ece-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="38ece-126">True</span><span class="sxs-lookup"><span data-stu-id="38ece-126">True</span></span>  <br/> |
   

