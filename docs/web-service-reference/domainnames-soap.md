---
title: DomainNames (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: Элемент DomainNames представляет коллекцию имен домена. Элемент DomainNames — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 45d256f3d5a57028a04572ad67d4be0786ca39e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762205"
---
# <a name="domainnames-soap"></a><span data-ttu-id="01dd0-105">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01dd0-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="01dd0-106">Элемент **DomainNames** представляет коллекцию имен домена.</span><span class="sxs-lookup"><span data-stu-id="01dd0-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="01dd0-107">Элемент **DomainNames** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="01dd0-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="01dd0-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="01dd0-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="01dd0-109">**DomainNames**</span><span class="sxs-lookup"><span data-stu-id="01dd0-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01dd0-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="01dd0-110">Attributes and elements</span></span>

<span data-ttu-id="01dd0-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="01dd0-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01dd0-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="01dd0-112">Attributes</span></span>

<span data-ttu-id="01dd0-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="01dd0-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01dd0-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="01dd0-114">Child elements</span></span>

|<span data-ttu-id="01dd0-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01dd0-115">**Element**</span></span>|<span data-ttu-id="01dd0-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01dd0-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01dd0-117">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01dd0-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="01dd0-118">Представляет коллекцию доменов, возвращенных из [GetDomainSettings операции (SOAP)](getdomainsettings-operation-soap.md), [операция GetFederationInformation (SOAP)](getfederationinformation-operation-soap.md)или [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="01dd0-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01dd0-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="01dd0-119">Parent elements</span></span>

|<span data-ttu-id="01dd0-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="01dd0-120">**Element**</span></span>|<span data-ttu-id="01dd0-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="01dd0-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01dd0-122">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01dd0-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="01dd0-123">Представляет список отношений организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="01dd0-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01dd0-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="01dd0-124">Text value</span></span>

<span data-ttu-id="01dd0-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="01dd0-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01dd0-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="01dd0-126">Remarks</span></span>

<span data-ttu-id="01dd0-127">Этот элемент представляет доменов SMTP внешними организациями.</span><span class="sxs-lookup"><span data-stu-id="01dd0-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01dd0-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="01dd0-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01dd0-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="01dd0-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="01dd0-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="01dd0-130">Schema Name</span></span>  <br/> |<span data-ttu-id="01dd0-131">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="01dd0-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="01dd0-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="01dd0-132">Validation File</span></span>  <br/> |<span data-ttu-id="01dd0-133">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="01dd0-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01dd0-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="01dd0-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="01dd0-135">True</span><span class="sxs-lookup"><span data-stu-id="01dd0-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01dd0-136">См. также</span><span class="sxs-lookup"><span data-stu-id="01dd0-136">See also</span></span>

- [<span data-ttu-id="01dd0-137">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="01dd0-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

