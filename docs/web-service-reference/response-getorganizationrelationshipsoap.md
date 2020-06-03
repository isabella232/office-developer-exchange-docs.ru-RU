---
title: Отклик (Жеторганизатионрелатионшип) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e6bbe800-3cbc-48b2-87b3-2043f575e88b
description: Элемент Response содержит сведения об отклике операции Жеторганизатионрелатионшипсеттингс (SOAP). Элемент Response предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 55f8cd549f40b780b2e7438634a851a2c3854f40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467944"
---
# <a name="response-getorganizationrelationship-soap"></a><span data-ttu-id="11be1-105">Отклик (Жеторганизатионрелатионшип) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="11be1-105">Response (GetOrganizationRelationship) (SOAP)</span></span>

<span data-ttu-id="11be1-106">Элемент **Response** содержит сведения об отклике [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="11be1-106">The **Response** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response information.</span></span> <span data-ttu-id="11be1-107">Элемент **Response** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="11be1-107">The **Response** element is for internal use only.</span></span> <span data-ttu-id="11be1-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="11be1-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="11be1-109">**жеторганизатионрелатионшипсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="11be1-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="11be1-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="11be1-110">Attributes and elements</span></span>

<span data-ttu-id="11be1-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="11be1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="11be1-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="11be1-112">Attributes</span></span>

<span data-ttu-id="11be1-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11be1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="11be1-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="11be1-114">Child elements</span></span>

|<span data-ttu-id="11be1-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="11be1-115">**Element**</span></span>|<span data-ttu-id="11be1-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="11be1-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="11be1-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="11be1-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="11be1-118">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="11be1-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="11be1-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="11be1-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="11be1-120">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="11be1-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="11be1-121">Организатионрелатионшипсеттингсколлектион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="11be1-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="11be1-122">Представляет список отношений Организации, которые совпадают с запросом.</span><span class="sxs-lookup"><span data-stu-id="11be1-122">Represents a list of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="11be1-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="11be1-123">Parent elements</span></span>

<span data-ttu-id="11be1-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11be1-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="11be1-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="11be1-125">Text value</span></span>

<span data-ttu-id="11be1-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="11be1-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="11be1-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="11be1-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="11be1-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="11be1-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="11be1-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="11be1-129">Schema Name</span></span>  <br/> |<span data-ttu-id="11be1-130">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="11be1-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="11be1-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="11be1-131">Validation File</span></span>  <br/> |<span data-ttu-id="11be1-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="11be1-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="11be1-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="11be1-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="11be1-134">True</span><span class="sxs-lookup"><span data-stu-id="11be1-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="11be1-135">См. также</span><span class="sxs-lookup"><span data-stu-id="11be1-135">See also</span></span>



[<span data-ttu-id="11be1-136">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="11be1-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

