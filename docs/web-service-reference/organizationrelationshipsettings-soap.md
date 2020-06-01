---
title: Организатионрелатионшипсеттингс (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 917481bb-46fc-4b88-8683-4cf812dcb0ab
description: Элемент Организатионрелатионшипсеттингс представляет список отношений Организации для одной организации. Элемент Организатионрелатионшипсеттингс предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 383b3635e1435c6597ccf793a7990c411c02d36d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462460"
---
# <a name="organizationrelationshipsettings-soap"></a><span data-ttu-id="f7d42-105">Организатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-105">OrganizationRelationshipSettings (SOAP)</span></span>

<span data-ttu-id="f7d42-106">Элемент **организатионрелатионшипсеттингс** представляет список отношений Организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="f7d42-106">The **OrganizationRelationshipSettings** element represents a list of organization relationships for a single organization.</span></span> <span data-ttu-id="f7d42-107">Элемент **организатионрелатионшипсеттингс** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="f7d42-107">The **OrganizationRelationshipSettings** element is for internal use only.</span></span> <span data-ttu-id="f7d42-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="f7d42-108">This element is not used by clients.</span></span> 
  
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

 <span data-ttu-id="f7d42-109">**организатионрелатионшипсеттингс**</span><span class="sxs-lookup"><span data-stu-id="f7d42-109">**OrganizationRelationshipSettings**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f7d42-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f7d42-110">Attributes and elements</span></span>

<span data-ttu-id="f7d42-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f7d42-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f7d42-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f7d42-112">Attributes</span></span>

<span data-ttu-id="f7d42-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f7d42-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f7d42-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f7d42-114">Child elements</span></span>

|<span data-ttu-id="f7d42-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f7d42-115">**Element**</span></span>|<span data-ttu-id="f7d42-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f7d42-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7d42-117">Деливерирепортенаблед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-117">DeliveryReportEnabled (SOAP)</span></span>](deliveryreportenabled-soap.md) <br/> |<span data-ttu-id="f7d42-118">Представляет флаг [деливерирепортенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-118">Represents the [DeliveryReportEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.DeliveryReportEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-119">Имя_домена (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-119">DomainNames (SOAP)</span></span>](domainnames-soap.md) <br/> |<span data-ttu-id="f7d42-120">Представляет коллекцию доменных имен.</span><span class="sxs-lookup"><span data-stu-id="f7d42-120">Represents the domain names collection.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-121">Фрибусякцессенаблед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-121">FreeBusyAccessEnabled (SOAP)</span></span>](freebusyaccessenabled-soap.md) <br/> |<span data-ttu-id="f7d42-122">Представляет флаг [фрибусякцессенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-122">Represents the [FreeBusyAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.FreeBusyAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-123">FreeBusyAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-123">FreeBusyAccessLevel (SOAP)</span></span>](freebusyaccesslevel-soap.md) <br/> |<span data-ttu-id="f7d42-124">Представляет свойство [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-124">Represents the [FreeBusyAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.FreeBusyAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-125">Маилтипсакцессенаблед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-125">MailTipsAccessEnabled (SOAP)</span></span>](mailtipsaccessenabled-soap.md) <br/> |<span data-ttu-id="f7d42-126">Представляет флаг [маилтипсакцессенаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-126">Represents the [MailTipsAccessEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailTipsAccessEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-127">MailTipsAccessLevel (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-127">MailTipsAccessLevel (SOAP)</span></span>](mailtipsaccesslevel-soap.md) <br/> |<span data-ttu-id="f7d42-128">Представляет свойство [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-128">Represents the [MailTipsAccessLevel](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.MailTipsAccessLevel.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-129">Маилбоксмовинаблед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-129">MailboxMoveEnabled (SOAP)</span></span>](mailboxmoveenabled-soap.md) <br/> |<span data-ttu-id="f7d42-130">Представляет флаг [маилбоксмовинаблед ()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-130">Represents the [MailboxMoveEnabled()](https://msdn.microsoft.com/library/Microsoft.Exchange.SoapWebClient.AutoDiscover.OrganizationRelationshipSettings.MailboxMoveEnabled.aspx) flag.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-131">Имя (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-131">Name (SOAP)</span></span>](name-soap.md) <br/> |<span data-ttu-id="f7d42-132">Представляет имя связи Организации.</span><span class="sxs-lookup"><span data-stu-id="f7d42-132">Represents the name of the organization relationship.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-133">Таржетаппликатионури (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-133">TargetApplicationUri (SOAP)</span></span>](targetapplicationuri-soap.md) <br/> |<span data-ttu-id="f7d42-134">Определяет универсальный код ресурса (URI) конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="f7d42-134">Defines the target application URI.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-135">Таржетаутодисковерепр (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-135">TargetAutodiscoverEpr (SOAP)</span></span>](targetautodiscoverepr-soap.md) <br/> |<span data-ttu-id="f7d42-136">Представляет свойство [таржетаутодисковерепр](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-136">Represents the [TargetAutodiscoverEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetAutodiscoverEpr.aspx) property.</span></span>  <br/> |
|[<span data-ttu-id="f7d42-137">Таржетшаринжепр (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-137">TargetSharingEpr (SOAP)</span></span>](targetsharingepr-soap.md) <br/> |<span data-ttu-id="f7d42-138">Представляет свойство [таржетшаринжепр](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) .</span><span class="sxs-lookup"><span data-stu-id="f7d42-138">Represents the [TargetSharingEpr](https://msdn.microsoft.com/library/Microsoft.Exchange.Data.Directory.SystemConfiguration.OrganizationRelationship.TargetSharingEpr.aspx) property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f7d42-139">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f7d42-139">Parent elements</span></span>

|<span data-ttu-id="f7d42-140">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f7d42-140">**Element**</span></span>|<span data-ttu-id="f7d42-141">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f7d42-141">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f7d42-142">Организатионрелатионшипсеттингсколлектион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f7d42-142">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="f7d42-143">Представляет список отношений Организации, которые совпадают с запросом.</span><span class="sxs-lookup"><span data-stu-id="f7d42-143">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f7d42-144">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="f7d42-144">Text value</span></span>

<span data-ttu-id="f7d42-145">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f7d42-145">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f7d42-146">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f7d42-146">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f7d42-147">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f7d42-147">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f7d42-148">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f7d42-148">Schema Name</span></span>  <br/> |<span data-ttu-id="f7d42-149">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="f7d42-149">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f7d42-150">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f7d42-150">Validation File</span></span>  <br/> |<span data-ttu-id="f7d42-151">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="f7d42-151">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f7d42-152">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f7d42-152">Can be Empty</span></span>  <br/> |<span data-ttu-id="f7d42-153">True</span><span class="sxs-lookup"><span data-stu-id="f7d42-153">True</span></span>  <br/> |
   

