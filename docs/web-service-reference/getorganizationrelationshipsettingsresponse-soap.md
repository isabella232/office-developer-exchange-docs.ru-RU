---
title: Жеторганизатионрелатионшипсеттингсреспонсе (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2f43b817-92c2-4e04-8095-479d790f768c
description: Элемент Жеторганизатионрелатионшипсеттингсреспонсе содержит ответ операции Жеторганизатионрелатионшипсеттингс (SOAP). Элемент Жеторганизатионрелатионшипсеттингсреспонсе предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 0f34fbc6577b379dd0ac379564c5e6bbd940d379
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457923"
---
# <a name="getorganizationrelationshipsettingsresponse-soap"></a><span data-ttu-id="23e23-105">Жеторганизатионрелатионшипсеттингсреспонсе (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e23-105">GetOrganizationRelationshipSettingsResponse (SOAP)</span></span>

<span data-ttu-id="23e23-106">Элемент **жеторганизатионрелатионшипсеттингсреспонсе** содержит ответ [операции жеторганизатионрелатионшипсеттингс (SOAP)](getorganizationrelationshipsettings-operation-soap.md) .</span><span class="sxs-lookup"><span data-stu-id="23e23-106">The **GetOrganizationRelationshipSettingsResponse** element contains the [GetOrganizationRelationshipSettings operation (SOAP)](getorganizationrelationshipsettings-operation-soap.md) response.</span></span> <span data-ttu-id="23e23-107">Элемент **жеторганизатионрелатионшипсеттингсреспонсе** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="23e23-107">The **GetOrganizationRelationshipSettingsResponse** element is for internal use only.</span></span> <span data-ttu-id="23e23-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="23e23-108">This element is not used by clients.</span></span> 
  
```XML
<GetOrganizationRelationshipSettingResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <OrganizationRelationshipSettingsCollection/>
</GetOrganizationRelationshipSettingResponse>
```

 <span data-ttu-id="23e23-109">**жеторганизатионрелатионшипсеттингсреспонсе**</span><span class="sxs-lookup"><span data-stu-id="23e23-109">**GetOrganizationRelationshipSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="23e23-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="23e23-110">Attributes and elements</span></span>

<span data-ttu-id="23e23-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="23e23-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="23e23-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="23e23-112">Attributes</span></span>

<span data-ttu-id="23e23-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e23-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="23e23-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="23e23-114">Child elements</span></span>

|<span data-ttu-id="23e23-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="23e23-115">**Element**</span></span>|<span data-ttu-id="23e23-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="23e23-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="23e23-117">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e23-117">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="23e23-118">Представляет код ошибки, возвращенный службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="23e23-118">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="23e23-119">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e23-119">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="23e23-120">Представляет сообщение, связанное с кодом ошибки, возвращаемым службой автообнаружения.</span><span class="sxs-lookup"><span data-stu-id="23e23-120">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="23e23-121">Организатионрелатионшипсеттингсколлектион (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e23-121">OrganizationRelationshipSettingsCollection (SOAP)</span></span>](organizationrelationshipsettingscollection-soap.md) <br/> |<span data-ttu-id="23e23-122">Представляет коллекцию отношений Организации, которые совпадают с запросом.</span><span class="sxs-lookup"><span data-stu-id="23e23-122">Represents a collection of organization relationships that match the query.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="23e23-123">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="23e23-123">Parent elements</span></span>

<span data-ttu-id="23e23-124">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e23-124">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="23e23-125">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="23e23-125">Text value</span></span>

<span data-ttu-id="23e23-126">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="23e23-126">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="23e23-127">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="23e23-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="23e23-128">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="23e23-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="23e23-129">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="23e23-129">Schema Name</span></span>  <br/> |<span data-ttu-id="23e23-130">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="23e23-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="23e23-131">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="23e23-131">Validation File</span></span>  <br/> |<span data-ttu-id="23e23-132">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="23e23-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="23e23-133">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="23e23-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="23e23-134">True</span><span class="sxs-lookup"><span data-stu-id="23e23-134">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="23e23-135">См. также</span><span class="sxs-lookup"><span data-stu-id="23e23-135">See also</span></span>



[<span data-ttu-id="23e23-136">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="23e23-136">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

