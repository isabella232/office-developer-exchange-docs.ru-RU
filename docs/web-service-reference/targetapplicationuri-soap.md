---
title: TargetApplicationUri (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: Элемент TargetApplicationUri определяет конечное приложение URI. Элемент TargetApplicationUri — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: fa401d4c1e8c1460804f116d840fe21129957852
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840133"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="6e1da-105">TargetApplicationUri (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e1da-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="6e1da-106">Элемент **TargetApplicationUri** определяет конечное приложение URI.</span><span class="sxs-lookup"><span data-stu-id="6e1da-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="6e1da-107">Элемент **TargetApplicationUri** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="6e1da-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="6e1da-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="6e1da-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="6e1da-109">**anyURI**</span><span class="sxs-lookup"><span data-stu-id="6e1da-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6e1da-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="6e1da-110">Attributes and elements</span></span>

<span data-ttu-id="6e1da-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="6e1da-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6e1da-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="6e1da-112">Attributes</span></span>

<span data-ttu-id="6e1da-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e1da-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6e1da-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="6e1da-114">Child elements</span></span>

<span data-ttu-id="6e1da-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="6e1da-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6e1da-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="6e1da-116">Parent elements</span></span>

|<span data-ttu-id="6e1da-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="6e1da-117">**Element**</span></span>|<span data-ttu-id="6e1da-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="6e1da-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6e1da-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e1da-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="6e1da-120">Представляет список отношений организации для одной организации</span><span class="sxs-lookup"><span data-stu-id="6e1da-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6e1da-121">Замечания</span><span class="sxs-lookup"><span data-stu-id="6e1da-121">Remarks</span></span>

<span data-ttu-id="6e1da-122">Этот элемент определяет целевой URI-адрес внешней организации.</span><span class="sxs-lookup"><span data-stu-id="6e1da-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6e1da-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="6e1da-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6e1da-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="6e1da-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6e1da-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="6e1da-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6e1da-126">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="6e1da-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6e1da-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="6e1da-127">Validation File</span></span>  <br/> |<span data-ttu-id="6e1da-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6e1da-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6e1da-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="6e1da-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6e1da-130">True</span><span class="sxs-lookup"><span data-stu-id="6e1da-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6e1da-131">См. также</span><span class="sxs-lookup"><span data-stu-id="6e1da-131">See also</span></span>



[<span data-ttu-id="6e1da-132">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6e1da-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

