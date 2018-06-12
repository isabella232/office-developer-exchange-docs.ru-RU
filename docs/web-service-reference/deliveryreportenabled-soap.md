---
title: DeliveryReportEnabled (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: 2ab522bc-40ea-4e43-aa57-6d2562db35e9
description: Элемент DeliveryReportEnabled представляет флаг DeliveryReportEnabled(). Элемент DeliveryReportEnabled — только для внутреннего использования. Этот элемент не используется с клиентами.
ms.openlocfilehash: 089256a5f75ad92a4f11c5aaf3d175382eeee456
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762065"
---
# <a name="deliveryreportenabled-soap"></a><span data-ttu-id="a967b-105">DeliveryReportEnabled (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a967b-105">DeliveryReportEnabled (SOAP)</span></span>

<span data-ttu-id="a967b-106">Элемент **DeliveryReportEnabled** представляет флаг **DeliveryReportEnabled()** .</span><span class="sxs-lookup"><span data-stu-id="a967b-106">The **DeliveryReportEnabled** element represents the **DeliveryReportEnabled()** flag.</span></span> <span data-ttu-id="a967b-107">Элемент **DeliveryReportEnabled** — только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="a967b-107">The **DeliveryReportEnabled** element is for internal use only.</span></span> <span data-ttu-id="a967b-108">Этот элемент не используется с клиентами.</span><span class="sxs-lookup"><span data-stu-id="a967b-108">This element is not used by clients.</span></span> 
  
```XML
<DeliveryReportEnabled>true | false</DeliveryReportEnabled>
```

 <span data-ttu-id="a967b-109">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a967b-109">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a967b-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a967b-110">Attributes and elements</span></span>

<span data-ttu-id="a967b-111">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a967b-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a967b-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a967b-112">Attributes</span></span>

<span data-ttu-id="a967b-113">Нет.</span><span class="sxs-lookup"><span data-stu-id="a967b-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a967b-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a967b-114">Child elements</span></span>

<span data-ttu-id="a967b-115">Нет.</span><span class="sxs-lookup"><span data-stu-id="a967b-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a967b-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a967b-116">Parent elements</span></span>

|<span data-ttu-id="a967b-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a967b-117">**Element**</span></span>|<span data-ttu-id="a967b-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a967b-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a967b-119">OrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a967b-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="a967b-120">Представляет список отношений организации для одной организации.</span><span class="sxs-lookup"><span data-stu-id="a967b-120">Represents a list of organization relationships for a single organization.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a967b-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a967b-121">Text value</span></span>

<span data-ttu-id="a967b-122">Текстовое значение true для элемента DeliveryReportEnabled указывает, можно ли использовать отчеты о доставке от пользователей в организации.</span><span class="sxs-lookup"><span data-stu-id="a967b-122">A text value of true for the DeliveryReportEnabled element indicates that the delivery reports from users in the organization can be used.</span></span> <span data-ttu-id="a967b-123">Значение false указывает, что отчеты о доставке необходимо было отменено.</span><span class="sxs-lookup"><span data-stu-id="a967b-123">A value of false indicates that the delivery reports should suppressed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a967b-124">Замечания</span><span class="sxs-lookup"><span data-stu-id="a967b-124">Remarks</span></span>

<span data-ttu-id="a967b-125">Используйте этот элемент, чтобы разрешить или отключить отчеты о доставке с сервера.</span><span class="sxs-lookup"><span data-stu-id="a967b-125">Use this element to allow or suppress delivery reports from the server.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a967b-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a967b-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a967b-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a967b-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="a967b-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a967b-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a967b-129">Схема службы автообнаружения</span><span class="sxs-lookup"><span data-stu-id="a967b-129">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="a967b-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a967b-130">Validation File</span></span>  <br/> |<span data-ttu-id="a967b-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a967b-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a967b-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a967b-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a967b-133">True</span><span class="sxs-lookup"><span data-stu-id="a967b-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a967b-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a967b-134">See also</span></span>

- [<span data-ttu-id="a967b-135">Операция GetOrganizationRelationshipSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="a967b-135">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

