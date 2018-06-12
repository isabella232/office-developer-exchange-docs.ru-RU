---
title: OrganizationRelationshipSettings (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: Элемент OrganizationRelationshipSettings представляет список отношений организации для одной организации. Элемент OrganizationRelationshipSettings — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: ed6cc0ef1891cd92c02a8e088e913886048623ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19834660"
---
# <a name="organizationrelationshipsettings-soap"></a><span data-ttu-id="8bcdc-105">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-105">OrganizationRelationshipSettings (SOAP)</span></span>

<span data-ttu-id="8bcdc-106">Элемент **OrganizationRelationshipSettings** представляет список отношений организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-106">The **OrganizationRelationshipSettings** element represents a list of organization relationships for a single organization.</span></span> <span data-ttu-id="8bcdc-107">Элемент **OrganizationRelationshipSettings** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-107">The **OrganizationRelationshipSettings** element is for internal use only.</span></span> <span data-ttu-id="8bcdc-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-108">This element is not used by clients.</span></span> 
  
```XML
<OrganizationRelationshipSettings>
    <DeliveryReportEnabled/>
    <DomainNames/>
    <FreeBusyAccessEnabled/>
    <FreeBusyAccessLevel/>
    <MailTipsAccessEnabled/>
    <MailTipsAccessLevel/>
    <MailboxMoveEnabled/>
    <Name/>
    <TargetApplicationUri/>
    <TargetAudodiscoverEpr/>
    <TargetSharingEpr/>
</OrganizationRelationshipSettings>
```

 <span data-ttu-id="8bcdc-109">**OrganizationRelationshipSettings**</span><span class="sxs-lookup"><span data-stu-id="8bcdc-109">**OrganizationRelationshipSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8bcdc-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="8bcdc-110">Attributes and elements</span></span>

<span data-ttu-id="8bcdc-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bcdc-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="8bcdc-112">Attributes</span></span>

<span data-ttu-id="8bcdc-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8bcdc-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="8bcdc-114">Child elements</span></span>

|<span data-ttu-id="8bcdc-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8bcdc-115">**Element**</span></span>|<span data-ttu-id="8bcdc-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8bcdc-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bcdc-117">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-117">DeliveryReportEnabled (SOAP)</span></span>](deliveryreportenabled-soap.md) <br/> |<span data-ttu-id="8bcdc-118">Представляет флаг [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-118">Represents the [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-119">DomainNames (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-119">DomainNames (SOAP)</span></span>](domainnames-soap.md) <br/> |<span data-ttu-id="8bcdc-120">Представляет коллекцию имен домена.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-120">Represents the domain names collection.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-121">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-121">FreeBusyAccessEnabled (SOAP)</span></span>](freebusyaccessenabled-soap.md) <br/> |<span data-ttu-id="8bcdc-122">Представляет флаг [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-122">Represents the [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-123">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-123">FreeBusyAccessLevel (SOAP)</span></span>](freebusyaccesslevel-soap.md) <br/> |<span data-ttu-id="8bcdc-124">Представляет свойство [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-124">Represents the [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-125">MailTipsAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-125">MailTipsAccessEnabled (SOAP)</span></span>](mailtipsaccessenabled-soap.md) <br/> |<span data-ttu-id="8bcdc-126">Представляет флаг [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-126">Represents the [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-127">MailTipsAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-127">MailTipsAccessLevel (SOAP)</span></span>](mailtipsaccesslevel-soap.md) <br/> |<span data-ttu-id="8bcdc-128">Представляет свойство [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-128">Represents the [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-129">MailboxMoveEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-129">MailboxMoveEnabled (SOAP)</span></span>](mailboxmoveenabled-soap.md) <br/> |<span data-ttu-id="8bcdc-130">Представляет флаг [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-130">Represents the [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-131">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-131">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="8bcdc-132">Представляет имя связи организации.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-132">Represents the name of the organization relationship.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-133">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-133">TargetApplicationUri (SOAP)</span></span>](targetapplicationuri-soap.md) <br/> |<span data-ttu-id="8bcdc-134">Задает URI конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-134">Defines the target application URI.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-135">TargetAutodiscoverEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-135">TargetAutodiscoverEpr (SOAP)</span></span>](targetautodiscoverepr-soap.md) <br/> |<span data-ttu-id="8bcdc-136">Представляет свойство [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-136">Represents the [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="8bcdc-137">TargetSharingEpr (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-137">TargetSharingEpr (SOAP)</span></span>](targetsharingepr-soap.md) <br/> |<span data-ttu-id="8bcdc-138">Представляет свойство [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="8bcdc-138">Represents the [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8bcdc-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="8bcdc-139">Parent elements</span></span>

|<span data-ttu-id="8bcdc-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="8bcdc-140">**Element**</span></span>|<span data-ttu-id="8bcdc-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="8bcdc-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bcdc-142">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8bcdc-142">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="8bcdc-143">Представляет список отношений организации, которые соответствуют запроса.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-143">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8bcdc-144">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="8bcdc-144">Text value</span></span>

<span data-ttu-id="8bcdc-145">Нет.</span><span class="sxs-lookup"><span data-stu-id="8bcdc-145">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bcdc-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="8bcdc-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bcdc-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="8bcdc-147">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8bcdc-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="8bcdc-148">Schema Name</span></span>  <br/> |<span data-ttu-id="8bcdc-149">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="8bcdc-149">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8bcdc-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="8bcdc-150">Validation File</span></span>  <br/> |<span data-ttu-id="8bcdc-151">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8bcdc-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8bcdc-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="8bcdc-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="8bcdc-153">True</span><span class="sxs-lookup"><span data-stu-id="8bcdc-153">True</span></span>  <br/> |
   

