---
title: Ответ (GetOrganizationRelationship) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: Элемент Response с информацией GetOrganizationRelationshipSettings операции (SOAP) ответа. Элемент Response — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 97bef9ab9f0b860e62646703c35d539b7922a65a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19835174"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="1fbed-105">Ответ (GetOrganizationRelationship) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1fbed-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="1fbed-106">Элемент **ответа** содержит сведения ответа [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="1fbed-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="1fbed-107">Элемент **Response** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="1fbed-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="1fbed-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="1fbed-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="1fbed-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="1fbed-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1fbed-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="1fbed-110">Attributes and elements</span></span>

<span data-ttu-id="1fbed-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="1fbed-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1fbed-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="1fbed-112">Attributes</span></span>

<span data-ttu-id="1fbed-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="1fbed-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1fbed-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="1fbed-114">Child elements</span></span>

|<span data-ttu-id="1fbed-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="1fbed-115">**Element**</span></span>|<span data-ttu-id="1fbed-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="1fbed-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1fbed-117">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1fbed-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="1fbed-118">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1fbed-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1fbed-119">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1fbed-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="1fbed-120">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="1fbed-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="1fbed-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1fbed-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="1fbed-122">Представляет список отношений организации, которые соответствуют запроса.</span><span class="sxs-lookup"><span data-stu-id="1fbed-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1fbed-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="1fbed-123">Parent elements</span></span>

<span data-ttu-id="1fbed-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="1fbed-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="1fbed-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="1fbed-125">Text value</span></span>

<span data-ttu-id="1fbed-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="1fbed-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1fbed-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="1fbed-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1fbed-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="1fbed-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="1fbed-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="1fbed-129">Schema Name</span></span>  <br/> |<span data-ttu-id="1fbed-130">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="1fbed-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="1fbed-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="1fbed-131">Validation File</span></span>  <br/> |<span data-ttu-id="1fbed-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1fbed-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1fbed-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="1fbed-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="1fbed-134">True</span><span class="sxs-lookup"><span data-stu-id="1fbed-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1fbed-135">См. также</span><span class="sxs-lookup"><span data-stu-id="1fbed-135">See also</span></span>



[<span data-ttu-id="1fbed-136">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="1fbed-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

