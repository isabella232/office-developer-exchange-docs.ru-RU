---
title: FreeBusyResponseArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponseArray
api_type:
- schema
ms.assetid: 5592a37e-cf4b-4643-8a2a-fa58c40345b9
description: Элемент FreeBusyResponseArray содержит сведения о доступности запрошенного пользователей, а также состояние ответа.
ms.openlocfilehash: cc6022c28213667c40dc00b5627ed88c4f78e2f2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762658"
---
# <a name="freebusyresponsearray"></a><span data-ttu-id="a1611-103">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a1611-103">FreeBusyResponseArray</span></span>

<span data-ttu-id="a1611-104">Элемент **FreeBusyResponseArray** содержит сведения о доступности запрошенного пользователей, а также состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="a1611-104">The **FreeBusyResponseArray** element contains the requested users' availability information and the response status.</span></span> 
  
[<span data-ttu-id="a1611-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a1611-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a1611-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="a1611-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
```xml
<FreeBusyResponseArray>
   <FreeBusyResponse>...</FreeBusyResponse>
</FreeBusyResponseArray>
```

 <span data-ttu-id="a1611-107">**ArrayOfFreeBusyResponse**</span><span class="sxs-lookup"><span data-stu-id="a1611-107">**ArrayOfFreeBusyResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1611-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1611-108">Attributes and elements</span></span>

<span data-ttu-id="a1611-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a1611-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1611-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1611-110">Attributes</span></span>

<span data-ttu-id="a1611-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a1611-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1611-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1611-112">Child elements</span></span>

|<span data-ttu-id="a1611-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1611-113">**Element**</span></span>|<span data-ttu-id="a1611-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1611-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1611-115">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="a1611-115">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="a1611-116">Содержит сведения о доступности для одного почтового ящика пользователя, а также состояние ответа.</span><span class="sxs-lookup"><span data-stu-id="a1611-116">Contains the free/busy information for a single mailbox user and the response status.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a1611-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1611-117">Parent elements</span></span>

|<span data-ttu-id="a1611-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1611-118">**Element**</span></span>|<span data-ttu-id="a1611-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1611-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1611-120">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a1611-120">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md) <br/> |<span data-ttu-id="a1611-121">Содержит свойства, которые определяют сведения о доступности пользователя или предложенных собраний сведения о времени.</span><span class="sxs-lookup"><span data-stu-id="a1611-121">Contains the properties that define user availability information or suggested meeting time information.</span></span>  <br/> <span data-ttu-id="a1611-122">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a1611-122">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a1611-123">Замечания</span><span class="sxs-lookup"><span data-stu-id="a1611-123">Remarks</span></span>

<span data-ttu-id="a1611-124">Этот элемент не включен в GetUserAvailability ответа, если сведения о доступности не запрашивается.</span><span class="sxs-lookup"><span data-stu-id="a1611-124">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="a1611-125">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1611-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1611-126">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1611-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1611-127">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1611-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a1611-128">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1611-128">Schema Name</span></span>  <br/> |<span data-ttu-id="a1611-129">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="a1611-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a1611-130">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1611-130">Validation File</span></span>  <br/> |<span data-ttu-id="a1611-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a1611-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a1611-132">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1611-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1611-133">False</span><span class="sxs-lookup"><span data-stu-id="a1611-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1611-134">См. также</span><span class="sxs-lookup"><span data-stu-id="a1611-134">See also</span></span>



[<span data-ttu-id="a1611-135">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a1611-135">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a1611-136">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="a1611-136">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a1611-137">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a1611-137">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

