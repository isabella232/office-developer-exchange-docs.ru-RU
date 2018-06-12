---
title: Значение TimeWindow
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeWindow
api_type:
- schema
ms.assetid: 49c79266-353a-4036-a8e2-8a4660d0d8ea
description: Элемент значение TimeWindow указывает промежуток времени, запрос пользователя сведений о доступности.
ms.openlocfilehash: 05858b4d62b72b3ff9904c90652bb1bff78ceb41
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840189"
---
# <a name="timewindow"></a><span data-ttu-id="d3dc4-103">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="d3dc4-103">TimeWindow</span></span>

<span data-ttu-id="d3dc4-104">Элемент **значение TimeWindow** указывает промежуток времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="d3dc4-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d3dc4-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="d3dc4-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="d3dc4-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="d3dc4-107">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="d3dc4-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="d3dc4-108">**Срок действия**</span><span class="sxs-lookup"><span data-stu-id="d3dc4-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3dc4-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc4-109">Attributes and elements</span></span>

<span data-ttu-id="d3dc4-110">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3dc4-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3dc4-111">Attributes</span></span>

<span data-ttu-id="d3dc4-112">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3dc4-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc4-113">Child elements</span></span>

|<span data-ttu-id="d3dc4-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3dc4-114">**Element**</span></span>|<span data-ttu-id="d3dc4-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3dc4-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3dc4-116">Время начала</span><span class="sxs-lookup"><span data-stu-id="d3dc4-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="d3dc4-117">Представляет начало промежуток времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="d3dc4-118">Время окончания</span><span class="sxs-lookup"><span data-stu-id="d3dc4-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="d3dc4-119">Представляет конец промежуток времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3dc4-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3dc4-120">Parent elements</span></span>

|<span data-ttu-id="d3dc4-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3dc4-121">**Element**</span></span>|<span data-ttu-id="d3dc4-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3dc4-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3dc4-123">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="d3dc4-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="d3dc4-124">Указывает тип сведений о доступности, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="d3dc4-125">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d3dc4-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3dc4-126">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3dc4-126">Remarks</span></span>

<span data-ttu-id="d3dc4-127">Максимальное значение для этого периода времени — 42 дня.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="d3dc4-128">Это максимальное значение может быть изменено.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-128">This maximum value can be modified.</span></span> <span data-ttu-id="d3dc4-129">Все запросы на сведения о доступности пользователя за пределы максимальное значение возвращает ошибку.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="d3dc4-130">Если встречи, частично в промежуток времени, определенные в элементы [StartTime](starttime.md) и [EndTime](endtime.md) встречи включается целиком.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d3dc4-131">Схема, описывающая этот элемент находится в каталоге /EWS/ компьютера, на котором выполняется Microsoft® Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d3dc4-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="d3dc4-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3dc4-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3dc4-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3dc4-133">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3dc4-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3dc4-134">Schema Name</span></span>  <br/> |<span data-ttu-id="d3dc4-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3dc4-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3dc4-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3dc4-136">Validation File</span></span>  <br/> |<span data-ttu-id="d3dc4-137">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3dc4-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3dc4-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3dc4-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3dc4-139">False</span><span class="sxs-lookup"><span data-stu-id="d3dc4-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3dc4-140">См. также</span><span class="sxs-lookup"><span data-stu-id="d3dc4-140">See also</span></span>



[<span data-ttu-id="d3dc4-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d3dc4-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="d3dc4-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d3dc4-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

