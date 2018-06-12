---
title: FreeBusyResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyResponse
api_type:
- schema
ms.assetid: 3038d106-9ac9-4ac7-bb43-96c783edbef5
description: Элемент FreeBusyResponse содержит сведения о доступности для одного почтового ящика пользователя.
ms.openlocfilehash: 73e3972bb53d6bf59e5156098bad06bcde5f0155
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762655"
---
# <a name="freebusyresponse"></a><span data-ttu-id="fedc2-103">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="fedc2-103">FreeBusyResponse</span></span>

<span data-ttu-id="fedc2-104">Элемент **FreeBusyResponse** содержит сведения о доступности для одного почтового ящика пользователя.</span><span class="sxs-lookup"><span data-stu-id="fedc2-104">The **FreeBusyResponse** element contains the free/busy information for a single mailbox user.</span></span> 
  
[<span data-ttu-id="fedc2-105">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fedc2-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="fedc2-106">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="fedc2-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="fedc2-107">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="fedc2-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
```xml
<FreeBusyResponse>
   <ResponseMessage>...</ResponseMessage>
   <FreeBusyView>...</FreeBusyView>
</FreeBusyResponse>
```

 <span data-ttu-id="fedc2-108">**FreeBusyResponseType**</span><span class="sxs-lookup"><span data-stu-id="fedc2-108">**FreeBusyResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fedc2-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="fedc2-109">Attributes and elements</span></span>

<span data-ttu-id="fedc2-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="fedc2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fedc2-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="fedc2-111">Attributes</span></span>

<span data-ttu-id="fedc2-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="fedc2-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fedc2-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="fedc2-113">Child elements</span></span>

|<span data-ttu-id="fedc2-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fedc2-114">**Element**</span></span>|<span data-ttu-id="fedc2-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fedc2-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fedc2-116">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fedc2-116">ResponseMessage</span></span>](responsemessage.md) <br/> |<span data-ttu-id="fedc2-117">Содержит описательные сведения о состоянии ответа.</span><span class="sxs-lookup"><span data-stu-id="fedc2-117">Provides descriptive information about the response status.</span></span>  <br/> |
|[<span data-ttu-id="fedc2-118">FreeBusyView</span><span class="sxs-lookup"><span data-stu-id="fedc2-118">FreeBusyView</span></span>](freebusyview.md) <br/> |<span data-ttu-id="fedc2-119">Содержит сведения о доступности для конкретного пользователя.</span><span class="sxs-lookup"><span data-stu-id="fedc2-119">Contains availability information for a specific user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fedc2-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="fedc2-120">Parent elements</span></span>

|<span data-ttu-id="fedc2-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="fedc2-121">**Element**</span></span>|<span data-ttu-id="fedc2-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="fedc2-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fedc2-123">FreeBusyResponseArray</span><span class="sxs-lookup"><span data-stu-id="fedc2-123">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="fedc2-124">Содержит сведения о доступности запрошенного пользователей и состояния ответа.</span><span class="sxs-lookup"><span data-stu-id="fedc2-124">Contains the requested users' availability information and the response status.</span></span>  <br/> <span data-ttu-id="fedc2-125">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="fedc2-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fedc2-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="fedc2-126">Remarks</span></span>

<span data-ttu-id="fedc2-127">Этот элемент не включен в GetUserAvailability ответа, если сведения о доступности не запрашивается.</span><span class="sxs-lookup"><span data-stu-id="fedc2-127">This element is not included in a GetUserAvailability response if free/busy information is not requested.</span></span>
  
<span data-ttu-id="fedc2-128">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="fedc2-128">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fedc2-129">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="fedc2-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fedc2-130">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="fedc2-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fedc2-131">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="fedc2-131">Schema Name</span></span>  <br/> |<span data-ttu-id="fedc2-132">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="fedc2-132">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fedc2-133">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="fedc2-133">Validation File</span></span>  <br/> |<span data-ttu-id="fedc2-134">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fedc2-134">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fedc2-135">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="fedc2-135">Can be Empty</span></span>  <br/> |<span data-ttu-id="fedc2-136">False</span><span class="sxs-lookup"><span data-stu-id="fedc2-136">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fedc2-137">См. также</span><span class="sxs-lookup"><span data-stu-id="fedc2-137">See also</span></span>



[<span data-ttu-id="fedc2-138">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="fedc2-138">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="fedc2-139">GetUserAvailabilityResponse</span><span class="sxs-lookup"><span data-stu-id="fedc2-139">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="fedc2-140">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="fedc2-140">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

