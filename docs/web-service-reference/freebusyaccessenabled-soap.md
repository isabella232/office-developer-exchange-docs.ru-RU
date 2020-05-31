---
title: Фрибусякцессенаблед (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 8d2d3276-b180-424e-a707-7256d14a1776
description: Элемент Фрибусякцессенаблед представляет флаг Фрибусякцессенаблед (). Элемент Фрибусякцессенаблед предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 4727e7054c02a4b5d454cb880691ecc01a075327
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762657"
---
# <a name="freebusyaccessenabled-soap"></a><span data-ttu-id="727aa-105">Фрибусякцессенаблед (SOAP)</span><span class="sxs-lookup"><span data-stu-id="727aa-105">FreeBusyAccessEnabled (SOAP)</span></span>

<span data-ttu-id="727aa-106">Элемент **фрибусякцессенаблед** представляет флаг **фрибусякцессенаблед ()** .</span><span class="sxs-lookup"><span data-stu-id="727aa-106">The **FreeBusyAccessEnabled** element represents the **FreeBusyAccessEnabled()** flag.</span></span> <span data-ttu-id="727aa-107">Элемент **фрибусякцессенаблед** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="727aa-107">The **FreeBusyAccessEnabled** element is for internal use only.</span></span> <span data-ttu-id="727aa-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="727aa-108">This element is not used by clients.</span></span> 
  
```XML
<FreeBusyAccessEnabled>true | false</FreeBusyAccessEnabled>
```

 <span data-ttu-id="727aa-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="727aa-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="727aa-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="727aa-110">Attributes and elements</span></span>

<span data-ttu-id="727aa-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="727aa-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="727aa-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="727aa-112">Attributes</span></span>

<span data-ttu-id="727aa-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="727aa-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="727aa-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="727aa-114">Child elements</span></span>

<span data-ttu-id="727aa-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="727aa-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="727aa-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="727aa-116">Parent elements</span></span>

|<span data-ttu-id="727aa-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="727aa-117">**Element**</span></span>|<span data-ttu-id="727aa-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="727aa-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="727aa-119">Организатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="727aa-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="727aa-120">Представляет список отношений Организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="727aa-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="727aa-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="727aa-121">Text value</span></span>

<span data-ttu-id="727aa-122">Текстовое значение **true** для элемента **фрибусякцессенаблед** указывает, что отношение общего доступа должно использоваться для получения сведений о занятости от пользователей в Организации.</span><span class="sxs-lookup"><span data-stu-id="727aa-122">A text value of **true** for the **FreeBusyAccessEnabled** element indicates that the sharing relationship should be used to retrieve free busy information from users in the organization.</span></span> <span data-ttu-id="727aa-123">Значение **false** указывает, что отношение совместного доступа должно подавляться.</span><span class="sxs-lookup"><span data-stu-id="727aa-123">A value of **false** indicates that the sharing relationship should be suppressed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="727aa-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="727aa-124">Remarks</span></span>

<span data-ttu-id="727aa-125">Используйте этот элемент, чтобы разрешить или запретить отправку сведений о доступности с сервера.</span><span class="sxs-lookup"><span data-stu-id="727aa-125">Use this element to allow or suppress free/busy information from the server.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="727aa-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="727aa-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="727aa-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="727aa-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="727aa-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="727aa-128">Schema Name</span></span>  <br/> |<span data-ttu-id="727aa-129">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="727aa-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="727aa-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="727aa-130">Validation File</span></span>  <br/> |<span data-ttu-id="727aa-131">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="727aa-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="727aa-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="727aa-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="727aa-133">True</span><span class="sxs-lookup"><span data-stu-id="727aa-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="727aa-134">См. также</span><span class="sxs-lookup"><span data-stu-id="727aa-134">See also</span></span>



[<span data-ttu-id="727aa-135">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="727aa-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

