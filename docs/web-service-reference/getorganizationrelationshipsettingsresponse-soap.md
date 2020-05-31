---
title: Жеторганизатионрелатионшипсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: Элемент Жеторганизатионрелатионшипсеттингсреспонсе содержит ответ операции Жеторганизатионрелатионшипсеттингс (SOAP). Элемент Жеторганизатионрелатионшипсеттингсреспонсе предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 907113df2186a93345c6e0bc7dd470909508bd38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762866"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="db386-105">Жеторганизатионрелатионшипсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db386-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="db386-106">Элемент **жеторганизатионрелатионшипсеттингсреспонсе** содержит ответ [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="db386-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="db386-107">Элемент **жеторганизатионрелатионшипсеттингсреспонсе** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="db386-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="db386-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="db386-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="db386-109">**жеторганизатионрелатионшипсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="db386-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="db386-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="db386-110">Attributes and elements</span></span>

<span data-ttu-id="db386-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="db386-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="db386-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="db386-112">Attributes</span></span>

<span data-ttu-id="db386-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="db386-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="db386-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="db386-114">Child elements</span></span>

|<span data-ttu-id="db386-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="db386-115">**Element**</span></span>|<span data-ttu-id="db386-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="db386-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="db386-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db386-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="db386-118">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="db386-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="db386-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db386-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="db386-120">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="db386-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="db386-121">Организатионрелатионшипсеттингсколлектион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db386-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="db386-122">Представляет коллекцию отношений Организации, которые совпадают с запросом.</span><span class="sxs-lookup"><span data-stu-id="db386-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="db386-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="db386-123">Parent elements</span></span>

<span data-ttu-id="db386-124">Нет.</span><span class="sxs-lookup"><span data-stu-id="db386-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="db386-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="db386-125">Text value</span></span>

<span data-ttu-id="db386-126">Нет.</span><span class="sxs-lookup"><span data-stu-id="db386-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="db386-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="db386-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="db386-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="db386-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="db386-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="db386-129">Schema Name</span></span>  <br/> |<span data-ttu-id="db386-130">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="db386-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="db386-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="db386-131">Validation File</span></span>  <br/> |<span data-ttu-id="db386-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="db386-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="db386-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="db386-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="db386-134">True</span><span class="sxs-lookup"><span data-stu-id="db386-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="db386-135">См. также</span><span class="sxs-lookup"><span data-stu-id="db386-135">See also</span></span>



[<span data-ttu-id="db386-136">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="db386-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

