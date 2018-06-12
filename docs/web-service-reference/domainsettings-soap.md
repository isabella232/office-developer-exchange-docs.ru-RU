---
title: DomainSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: f3d37f5a-c9ea-4ed9-a011-94d33bda64d1
description: Элемент DomainSettings представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.
ms.openlocfilehash: 961051399dc8babd8cba6eeaf43456071d0f40a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762224"
---
# <a name="domainsettings-soap"></a><span data-ttu-id="4e3ad-103">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4e3ad-103">DomainSettings (SOAP)</span></span>

<span data-ttu-id="4e3ad-104">Элемент **DomainSettings** представляет параметры домена, которые были отправленными в запрос автообнаружения или возвращаемых ответа службы автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-104">The **DomainSettings** element represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span> 
  
```XML
<DomainSettings>
   <DomainSetting/>
</DomainSettings>
```

 <span data-ttu-id="4e3ad-105">**DomainSettings**</span><span class="sxs-lookup"><span data-stu-id="4e3ad-105">**DomainSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e3ad-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4e3ad-106">Attributes and elements</span></span>

<span data-ttu-id="4e3ad-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e3ad-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4e3ad-108">Attributes</span></span>

<span data-ttu-id="4e3ad-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e3ad-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4e3ad-110">Child elements</span></span>

|<span data-ttu-id="4e3ad-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e3ad-111">**Element**</span></span>|<span data-ttu-id="4e3ad-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e3ad-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e3ad-113">DomainSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4e3ad-113">DomainSetting (SOAP)</span></span>](domainsetting-soap.md) <br/> |<span data-ttu-id="4e3ad-114">Содержит параметры домена, возвращенных по запросу [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="4e3ad-114">Contains domain settings that are returned by a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e3ad-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4e3ad-115">Parent elements</span></span>

|<span data-ttu-id="4e3ad-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4e3ad-116">**Element**</span></span>|<span data-ttu-id="4e3ad-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4e3ad-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e3ad-118">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4e3ad-118">DomainResponse (SOAP)</span></span>](domainresponse-soap.md) <br/> |<span data-ttu-id="4e3ad-119">Содержит запрошенные параметры для конкретного домена.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-119">Contains the requested settings for the specified domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e3ad-120">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="4e3ad-120">Text value</span></span>

<span data-ttu-id="4e3ad-121">Нет.</span><span class="sxs-lookup"><span data-stu-id="4e3ad-121">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e3ad-122">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4e3ad-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e3ad-123">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4e3ad-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4e3ad-124">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4e3ad-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4e3ad-125">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="4e3ad-125">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4e3ad-126">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4e3ad-126">Validation File</span></span>  <br/> |<span data-ttu-id="4e3ad-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4e3ad-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e3ad-128">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4e3ad-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="4e3ad-129">True</span><span class="sxs-lookup"><span data-stu-id="4e3ad-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e3ad-130">См. также</span><span class="sxs-lookup"><span data-stu-id="4e3ad-130">See also</span></span>

- [<span data-ttu-id="4e3ad-131">Операция GetDomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4e3ad-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

