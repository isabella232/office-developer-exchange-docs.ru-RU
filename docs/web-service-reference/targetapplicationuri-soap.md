---
title: Таржетаппликатионури (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
ms.assetid: e13c0edd-2ab1-49bb-a993-54a8db2dfbb9
description: Элемент Таржетаппликатионури определяет универсальный код ресурса (URI) конечного приложения. Элемент Таржетаппликатионури предназначен только для внутреннего использования. Этот элемент не используется клиентами.
ms.openlocfilehash: 88968aac604b77cd057dbc69c396227a489ac9a8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457090"
---
# <a name="targetapplicationuri-soap"></a><span data-ttu-id="bc748-105">Таржетаппликатионури (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc748-105">TargetApplicationUri (SOAP)</span></span>

<span data-ttu-id="bc748-106">Элемент **таржетаппликатионури** определяет универсальный код ресурса (URI) конечного приложения.</span><span class="sxs-lookup"><span data-stu-id="bc748-106">The **TargetApplicationUri** element defines the target application URI.</span></span> <span data-ttu-id="bc748-107">Элемент **таржетаппликатионури** предназначен только для внутреннего использования.</span><span class="sxs-lookup"><span data-stu-id="bc748-107">The **TargetApplicationUri** element is for internal use only.</span></span> <span data-ttu-id="bc748-108">Этот элемент не используется клиентами.</span><span class="sxs-lookup"><span data-stu-id="bc748-108">This element is not used by clients.</span></span> 
  
```XML
<TargetApplicationUri/>
```

 <span data-ttu-id="bc748-109">**анюри**</span><span class="sxs-lookup"><span data-stu-id="bc748-109">**anyURI**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc748-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="bc748-110">Attributes and elements</span></span>

<span data-ttu-id="bc748-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="bc748-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc748-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="bc748-112">Attributes</span></span>

<span data-ttu-id="bc748-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc748-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc748-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="bc748-114">Child elements</span></span>

<span data-ttu-id="bc748-115">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="bc748-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="bc748-116">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="bc748-116">Parent elements</span></span>

|<span data-ttu-id="bc748-117">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="bc748-117">**Element**</span></span>|<span data-ttu-id="bc748-118">**Описание**</span><span class="sxs-lookup"><span data-stu-id="bc748-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc748-119">Организатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc748-119">OrganizationRelationshipSettings (SOAP)</span></span>](organizationrelationshipsettings-soap.md) <br/> |<span data-ttu-id="bc748-120">Представляет список отношений Организации для одной организации</span><span class="sxs-lookup"><span data-stu-id="bc748-120">Represents a list of organization relationships for a single organization</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="bc748-121">Примечания</span><span class="sxs-lookup"><span data-stu-id="bc748-121">Remarks</span></span>

<span data-ttu-id="bc748-122">Этот элемент определяет целевой универсальный код ресурса (URI) внешней организации.</span><span class="sxs-lookup"><span data-stu-id="bc748-122">This element defines the target URI of the external organization.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc748-123">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="bc748-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc748-124">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="bc748-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bc748-125">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="bc748-125">Schema Name</span></span>  <br/> |<span data-ttu-id="bc748-126">Схема автообнаружения</span><span class="sxs-lookup"><span data-stu-id="bc748-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bc748-127">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="bc748-127">Validation File</span></span>  <br/> |<span data-ttu-id="bc748-128">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="bc748-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc748-129">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="bc748-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc748-130">True</span><span class="sxs-lookup"><span data-stu-id="bc748-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc748-131">См. также</span><span class="sxs-lookup"><span data-stu-id="bc748-131">See also</span></span>



[<span data-ttu-id="bc748-132">Операция Жеторганизатионрелатионшипсеттингс (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc748-132">GetOrganizationRelationshipSettings operation (SOAP)</span></span>](getorganizationrelationshipsettings-operation-soap.md)

