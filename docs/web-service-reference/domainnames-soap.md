---
title: Имя_домена (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 79ffc3f9-25c4-40b5-84ce-09a3c5f892fa
description: Элемент DomainNames представляет коллекцию доменных имен. Элемент DomainNames предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 0b425b3cd4c0e7cb2427920d61feb04010a3b123
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458420"
---
# <a name="domainnames-soap"></a><span data-ttu-id="63864-105">Имя_домена (SOAP)</span><span class="sxs-lookup"><span data-stu-id="63864-105">DomainNames (SOAP)</span></span>

<span data-ttu-id="63864-106">Элемент **domainnames** представляет коллекцию доменных имен.</span><span class="sxs-lookup"><span data-stu-id="63864-106">The **DomainNames** element represents the domain names collection.</span></span> <span data-ttu-id="63864-107">Элемент **domainnames** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="63864-107">The **DomainNames** element is for internal use only.</span></span> <span data-ttu-id="63864-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="63864-108">This element is not used by clients.</span></span> 
  
```XML
<DomainNames>
    <Domains/>
</DomainNames>
```

 <span data-ttu-id="63864-109">**Имя_домена**</span><span class="sxs-lookup"><span data-stu-id="63864-109">**DomainNames**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="63864-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="63864-110">Attributes and elements</span></span>

<span data-ttu-id="63864-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="63864-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="63864-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="63864-112">Attributes</span></span>

<span data-ttu-id="63864-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="63864-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="63864-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="63864-114">Child elements</span></span>

|<span data-ttu-id="63864-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63864-115">**Element**</span></span>|<span data-ttu-id="63864-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63864-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63864-117">Домены (SOAP)</span><span class="sxs-lookup"><span data-stu-id="63864-117">Domains (SOAP)</span></span>](domains-soap.md) <br/> |<span data-ttu-id="63864-118">Представляет коллекцию доменов, которые возвращаются из [операции жетдомаинсеттингс (SOAP)](getdomainsettings-operation-soap.md), [операции жетфедератионинформатион (SOAP)](getfederationinformation-operation-soap.md)или [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span><span class="sxs-lookup"><span data-stu-id="63864-118">Represents a collection of domains that are returned from the [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), [GetFederationInformation operation (SOAP)](getfederationinformation-operation-soap.md), or the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="63864-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="63864-119">Parent elements</span></span>

|<span data-ttu-id="63864-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="63864-120">**Element**</span></span>|<span data-ttu-id="63864-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="63864-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="63864-122">Организатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="63864-122">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="63864-123">Представляет список отношений Организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="63864-123">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="63864-124">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="63864-124">Text value</span></span>

<span data-ttu-id="63864-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="63864-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="63864-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="63864-126">Remarks</span></span>

<span data-ttu-id="63864-127">Этот элемент представляет домены SMTP внешних организаций.</span><span class="sxs-lookup"><span data-stu-id="63864-127">This element represents the SMTP domains of the external organizations.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="63864-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="63864-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="63864-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="63864-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="63864-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="63864-130">Schema Name</span></span>  <br/> |<span data-ttu-id="63864-131">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="63864-131">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="63864-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="63864-132">Validation File</span></span>  <br/> |<span data-ttu-id="63864-133">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="63864-133">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="63864-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="63864-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="63864-135">True</span><span class="sxs-lookup"><span data-stu-id="63864-135">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="63864-136">См. также</span><span class="sxs-lookup"><span data-stu-id="63864-136">See also</span></span>

- [<span data-ttu-id="63864-137">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="63864-137">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

