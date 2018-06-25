---
title: GetOrganizationRelationshipSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: Элемент GetOrganizationRelationshipSettingsResponse содержит ответа GetOrganizationRelationshipSettings операции (SOAP). Элемент GetOrganizationRelationshipSettingsResponse — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762866"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="c0146-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0146-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="c0146-106">Элемент **GetOrganizationRelationshipSettingsResponse** содержит ответа [GetOrganizationRelationshipSettings операции (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="c0146-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="c0146-107">Элемент **GetOrganizationRelationshipSettingsResponse** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="c0146-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="c0146-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="c0146-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="c0146-109">**GetOrganizationRelationshipSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="c0146-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0146-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c0146-110">Attributes and elements</span></span>

<span data-ttu-id="c0146-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="c0146-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0146-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c0146-112">Attributes</span></span>

<span data-ttu-id="c0146-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0146-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c0146-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c0146-114">Child elements</span></span>

|<span data-ttu-id="c0146-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c0146-115">**Element**</span></span>|<span data-ttu-id="c0146-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c0146-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0146-117">Код ошибки (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0146-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="c0146-118">Представляет код ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="c0146-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="c0146-119">Сообщение об ошибке (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0146-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="c0146-120">Представляет сообщение, связанное с кодом ошибки, возвращаемые службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="c0146-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="c0146-121">OrganizationRelationshipSettingsCollection (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0146-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="c0146-122">Представляет коллекцию связи организации, которые соответствуют запроса.</span><span class="sxs-lookup"><span data-stu-id="c0146-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0146-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c0146-123">Parent elements</span></span>

<span data-ttu-id="c0146-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0146-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c0146-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c0146-125">Text value</span></span>

<span data-ttu-id="c0146-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="c0146-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0146-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c0146-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0146-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c0146-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c0146-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c0146-129">Schema Name</span></span>  <br/> |<span data-ttu-id="c0146-130">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="c0146-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c0146-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c0146-131">Validation File</span></span>  <br/> |<span data-ttu-id="c0146-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0146-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0146-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c0146-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="c0146-134">True</span><span class="sxs-lookup"><span data-stu-id="c0146-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0146-135">См. также</span><span class="sxs-lookup"><span data-stu-id="c0146-135">See also</span></span>



[<span data-ttu-id="c0146-136">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c0146-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

