---
title: FreeBusyAccessEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: Элемент FreeBusyAccessEnabled представляет флаг FreeBusyAccessEnabled(). Элемент FreeBusyAccessEnabled — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762657"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="374de-105">FreeBusyAccessEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="374de-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="374de-106">Элемент **FreeBusyAccessEnabled** представляет флаг **FreeBusyAccessEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="374de-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="374de-107">Элемент **FreeBusyAccessEnabled** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="374de-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="374de-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="374de-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="374de-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="374de-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="374de-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="374de-110">Attributes and elements</span></span>

<span data-ttu-id="374de-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="374de-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="374de-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="374de-112">Attributes</span></span>

<span data-ttu-id="374de-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="374de-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="374de-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="374de-114">Child elements</span></span>

<span data-ttu-id="374de-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="374de-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="374de-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="374de-116">Parent elements</span></span>

|<span data-ttu-id="374de-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="374de-117">**Element**</span></span>|<span data-ttu-id="374de-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="374de-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="374de-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="374de-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="374de-120">Представляет список отношений организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="374de-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="374de-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="374de-121">Text value</span></span>

<span data-ttu-id="374de-122">Текстовое значение **true** для элемента **FreeBusyAccessEnabled** указывает, что общего доступа отношения должен использоваться для извлечения сведений о занятости из пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="374de-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="374de-123">Значение **false** указывает, необходимо было отменено отношения общего доступа.</span><span class="sxs-lookup"><span data-stu-id="374de-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="374de-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="374de-124">Remarks</span></span>

<span data-ttu-id="374de-125">Этот элемент используется для разрешения или не отображать сведения о доступности с сервера.</span><span class="sxs-lookup"><span data-stu-id="374de-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="374de-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="374de-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="374de-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="374de-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="374de-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="374de-128">Schema Name</span></span>  <br/> |<span data-ttu-id="374de-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="374de-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="374de-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="374de-130">Validation File</span></span>  <br/> |<span data-ttu-id="374de-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="374de-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="374de-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="374de-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="374de-133">True</span><span class="sxs-lookup"><span data-stu-id="374de-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="374de-134">См. также</span><span class="sxs-lookup"><span data-stu-id="374de-134">See also</span></span>



[<span data-ttu-id="374de-135">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="374de-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

