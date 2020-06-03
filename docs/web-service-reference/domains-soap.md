---
title: Домены (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 5f81d1b7-c6a4-456f-9935-13d04a3d92d7
description: Элемент Domains представляет коллекцию доменов, которая возвращается в операции Жетдомаинсеттингс (SOAP), домены, для которых в организации используется операция Жетфедератионинформатион (SOAP), или домены с отношением Организации, возвращенные операцией Жеторганизатионрелатионшипсеттингс (SOAP).
ms.openlocfilehash: c56fb72841776c0060c1300b52b2f6a06b1ec0ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526307"
---
# <a name="domains-soap"></a><span data-ttu-id="0dfaf-103">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-103">Domains (SOAP)</span></span>

<span data-ttu-id="0dfaf-104">Элемент **Domains** представляет коллекцию доменов, которая возвращается в [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), домены, для которых в организации используется [Операция жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md), или домены с отношением Организации, возвращенные [операцией жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="0dfaf-104">The **Domains** element represents the domain collection that is returned in a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), the domains that the organization has federated in a [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the domains with an organization relationship as returned by [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>
  
```XML
<Domains>
   <Domain/>
</Domains>
```

 <span data-ttu-id="0dfaf-105">**Домены**</span><span class="sxs-lookup"><span data-stu-id="0dfaf-105">**Domains**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0dfaf-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="0dfaf-106">Attributes and elements</span></span>

<span data-ttu-id="0dfaf-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="0dfaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0dfaf-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="0dfaf-108">Attributes</span></span>

<span data-ttu-id="0dfaf-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0dfaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0dfaf-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="0dfaf-110">Child elements</span></span>

|<span data-ttu-id="0dfaf-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0dfaf-111">**Element**</span></span>|<span data-ttu-id="0dfaf-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dfaf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dfaf-113">Домен (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-113">Domain (SOAP)</span></span>](domain-soap.md) <br/> |<span data-ttu-id="0dfaf-114">Представляет один домен.</span><span class="sxs-lookup"><span data-stu-id="0dfaf-114">Represents a single domain.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0dfaf-115">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="0dfaf-115">Parent elements</span></span>

|<span data-ttu-id="0dfaf-116">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="0dfaf-116">**Element**</span></span>|<span data-ttu-id="0dfaf-117">**Описание**</span><span class="sxs-lookup"><span data-stu-id="0dfaf-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0dfaf-118">Жетдомаинсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-118">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md) <br/> |<span data-ttu-id="0dfaf-119">Представляет запрос [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfaf-119">Represents a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md) request.</span></span>  <br/> |
|[<span data-ttu-id="0dfaf-120">Отклик (Жетфедератионинформатион) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-120">Response (GetFederationInformation) (SOAP)</span></span>](response-getfederationinformationsoap.md) <br/> |<span data-ttu-id="0dfaf-121">Содержит данные ответа [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfaf-121">Contains the [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md) response information.</span></span>  <br/> |
|[<span data-ttu-id="0dfaf-122">Жеторганизатионрелатионшипсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-122">GetOrganizationRelationshipSettingsRequest (SOAP)</span></span>](getorganizationrelationshipsettingsrequest-soap.md) <br/> |<span data-ttu-id="0dfaf-123">Представляет запрос [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="0dfaf-123">Represents a [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0dfaf-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="0dfaf-124">Text value</span></span>

<span data-ttu-id="0dfaf-125">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="0dfaf-125">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0dfaf-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="0dfaf-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0dfaf-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="0dfaf-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0dfaf-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="0dfaf-128">Schema Name</span></span>  <br/> |<span data-ttu-id="0dfaf-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="0dfaf-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0dfaf-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="0dfaf-130">Validation File</span></span>  <br/> |<span data-ttu-id="0dfaf-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="0dfaf-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0dfaf-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="0dfaf-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="0dfaf-133">True</span><span class="sxs-lookup"><span data-stu-id="0dfaf-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0dfaf-134">См. также</span><span class="sxs-lookup"><span data-stu-id="0dfaf-134">See also</span></span>

- [<span data-ttu-id="0dfaf-135">Жетдомаинсеттингсрекуест (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-135">GetDomainSettingsRequest (SOAP)</span></span>](getdomainsettingsrequest-soap.md)  
- [<span data-ttu-id="0dfaf-136">Жетфедератионинформатионреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0dfaf-136">GetFederationInformationResponse (SOAP)</span></span>](getfederationinformationresponse-soap.md)

