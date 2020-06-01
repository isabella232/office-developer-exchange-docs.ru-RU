---
title: TimeWindow
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
description: Элемент TimeWindow определяет интервал времени, запрошенный для сведений о доступности пользователя.
ms.openlocfilehash: 5c66614520f9d616687d67ad609b3d55d9cf6571
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458931"
---
# <a name="timewindow"></a><span data-ttu-id="64daf-103">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="64daf-103">TimeWindow</span></span>

<span data-ttu-id="64daf-104">Элемент **TimeWindow** определяет интервал времени, запрошенный для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="64daf-104">The **TimeWindow** element identifies the time span queried for the user availability information.</span></span> 
  
[<span data-ttu-id="64daf-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="64daf-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="64daf-106">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="64daf-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
[<span data-ttu-id="64daf-107">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="64daf-107">TimeWindow</span></span>](timewindow.md)
  
```xml
<TimeWindow>
   <StartTime>dateTime</StartTime>
   <EndTime>dateTime</EndTime>
</TimeWindow>
```

 <span data-ttu-id="64daf-108">**Duration**</span><span class="sxs-lookup"><span data-stu-id="64daf-108">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="64daf-109">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="64daf-109">Attributes and elements</span></span>

<span data-ttu-id="64daf-110">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="64daf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="64daf-111">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="64daf-111">Attributes</span></span>

<span data-ttu-id="64daf-112">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="64daf-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="64daf-113">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="64daf-113">Child elements</span></span>

|<span data-ttu-id="64daf-114">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64daf-114">**Element**</span></span>|<span data-ttu-id="64daf-115">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64daf-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64daf-116">StartTime</span><span class="sxs-lookup"><span data-stu-id="64daf-116">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="64daf-117">Представляет начало интервала времени, запрошенного для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="64daf-117">Represents the start of a time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="64daf-118">EndTime</span><span class="sxs-lookup"><span data-stu-id="64daf-118">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="64daf-119">Представляет конец интервала времени, запрошенного для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="64daf-119">Represents the end of a time span queried for the user availability information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="64daf-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="64daf-120">Parent elements</span></span>

|<span data-ttu-id="64daf-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="64daf-121">**Element**</span></span>|<span data-ttu-id="64daf-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="64daf-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="64daf-123">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="64daf-123">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="64daf-124">Указывает тип сведений о доступности, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="64daf-124">Specifies the type of free/busy information returned in the response.</span></span>  <br/> <span data-ttu-id="64daf-125">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="64daf-125">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="64daf-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="64daf-126">Remarks</span></span>

<span data-ttu-id="64daf-127">Максимальное значение для этого периода времени составляет 42 дней.</span><span class="sxs-lookup"><span data-stu-id="64daf-127">The maximum value for this time period is 42 days.</span></span> <span data-ttu-id="64daf-128">Это максимальное значение можно изменить.</span><span class="sxs-lookup"><span data-stu-id="64daf-128">This maximum value can be modified.</span></span> <span data-ttu-id="64daf-129">Все запросы сведений о доступности пользователей за пределами максимального значения будут возвращать ошибку.</span><span class="sxs-lookup"><span data-stu-id="64daf-129">Any requests for user availability information beyond the maximum value will return an error.</span></span> <span data-ttu-id="64daf-130">Если какие-либо встречи частично указаны в диапазоне времени, определенном элементами [StartTime](starttime.md) и [EndTime](endtime.md) , эта встреча включается целиком.</span><span class="sxs-lookup"><span data-stu-id="64daf-130">If any appointments are partially in the time span defined by the [StartTime](starttime.md) and [EndTime](endtime.md) elements, that appointment is included in its entirety.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="64daf-131">Схема, описывающая этот элемент, находится в каталоге/ЕВС/компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="64daf-131">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="64daf-132">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="64daf-132">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="64daf-133">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="64daf-133">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="64daf-134">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="64daf-134">Schema Name</span></span>  <br/> |<span data-ttu-id="64daf-135">Схема Types</span><span class="sxs-lookup"><span data-stu-id="64daf-135">Types schema</span></span>  <br/> |
|<span data-ttu-id="64daf-136">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="64daf-136">Validation File</span></span>  <br/> |<span data-ttu-id="64daf-137">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="64daf-137">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="64daf-138">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="64daf-138">Can be Empty</span></span>  <br/> |<span data-ttu-id="64daf-139">False</span><span class="sxs-lookup"><span data-stu-id="64daf-139">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="64daf-140">См. также</span><span class="sxs-lookup"><span data-stu-id="64daf-140">See also</span></span>



[<span data-ttu-id="64daf-141">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="64daf-141">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="64daf-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="64daf-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

