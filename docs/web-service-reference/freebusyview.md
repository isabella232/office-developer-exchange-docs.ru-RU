---
title: фрибусивиев
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyView
api_type:
- schema
ms.assetid: cb18434f-5f41-4e05-a5ce-d921b2721a8c
description: Элемент Фрибусивиев содержит сведения о доступности для определенного пользователя.
ms.openlocfilehash: e5cc3bea6b57d5c400dd9be44bf9f9aaf9e43eb9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456103"
---
# <a name="freebusyview"></a><span data-ttu-id="d230f-103">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="d230f-103">FreeBusyView</span></span>

<span data-ttu-id="d230f-104">Элемент **фрибусивиев** содержит сведения о доступности для определенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d230f-104">The **FreeBusyView** element contains availability information for a specific user.</span></span> 
  
[<span data-ttu-id="d230f-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d230f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="d230f-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="d230f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="d230f-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d230f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="d230f-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="d230f-108">FreeBusyView</span></span>](freebusyview.md)
  
```xml
<FreeBusyView>
   <FreeBusyViewType>...</FreeBusyViewType>
   <MergedFreeBusy>...</MergedFreeBusy>
   <CalendarEventArray>...</CalendarEventArray>
   <WorkingHours>...</WorkingHours>
</FreeBusyView>
```

 <span data-ttu-id="d230f-109">**фрибусивиев**</span><span class="sxs-lookup"><span data-stu-id="d230f-109">**FreeBusyView**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d230f-110">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d230f-110">Attributes and elements</span></span>

<span data-ttu-id="d230f-111">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="d230f-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d230f-112">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d230f-112">Attributes</span></span>

<span data-ttu-id="d230f-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="d230f-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d230f-114">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d230f-114">Child elements</span></span>

|<span data-ttu-id="d230f-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d230f-115">**Element**</span></span>|<span data-ttu-id="d230f-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d230f-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d230f-117">фрибусивиевтипе</span><span class="sxs-lookup"><span data-stu-id="d230f-117">FreeBusyViewType</span></span>](freebusyviewtype.md) <br/> |<span data-ttu-id="d230f-118">Представляет тип запрошенных сведений о доступности, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="d230f-118">Represents the type of requested free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="d230f-119">мержедфрибуси</span><span class="sxs-lookup"><span data-stu-id="d230f-119">MergedFreeBusy</span></span>](mergedfreebusy.md) <br/> |<span data-ttu-id="d230f-120">Содержит Объединенный поток данных о занятости.</span><span class="sxs-lookup"><span data-stu-id="d230f-120">Contains the merged free/busy stream of data.</span></span>  <br/> |
|[<span data-ttu-id="d230f-121">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="d230f-121">CalendarEventArray</span></span>](calendareventarray.md) <br/> |<span data-ttu-id="d230f-122">Содержит набор уникальных экземпляров элемента календаря, представляющих доступность запрошенного пользователя.</span><span class="sxs-lookup"><span data-stu-id="d230f-122">Contains a set of unique calendar item occurrences that represent the requested user's availability.</span></span>  <br/> |
|[<span data-ttu-id="d230f-123">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="d230f-123">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md) <br/> |<span data-ttu-id="d230f-124">Представляет параметры часового пояса и рабочие часы для запрошенного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d230f-124">Represents the time zone settings and working hours for the requested mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d230f-125">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d230f-125">Parent elements</span></span>

|<span data-ttu-id="d230f-126">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d230f-126">**Element**</span></span>|<span data-ttu-id="d230f-127">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d230f-127">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d230f-128">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d230f-128">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="d230f-129">Содержит сведения о доступности для одного пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="d230f-129">Contains the free/busy information for a single mailbox user.</span></span>  <br/> <span data-ttu-id="d230f-130">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d230f-130">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d230f-131">Примечания</span><span class="sxs-lookup"><span data-stu-id="d230f-131">Remarks</span></span>

<span data-ttu-id="d230f-132">Все дочерние элементы перечислены в той последовательности, в которой они выполняются.</span><span class="sxs-lookup"><span data-stu-id="d230f-132">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="d230f-133">Уровень детализации, предоставляемый этим элементом, зависит от разрешений, предоставленных запрашивающему участнику.</span><span class="sxs-lookup"><span data-stu-id="d230f-133">The level of detail provided by this element depends on the permissions granted to the requestor.</span></span>
  
<span data-ttu-id="d230f-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d230f-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d230f-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d230f-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d230f-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d230f-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d230f-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d230f-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d230f-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d230f-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d230f-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d230f-139">Validation File</span></span>  <br/> |<span data-ttu-id="d230f-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="d230f-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d230f-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d230f-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="d230f-142">False</span><span class="sxs-lookup"><span data-stu-id="d230f-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d230f-143">См. также</span><span class="sxs-lookup"><span data-stu-id="d230f-143">See also</span></span>



[<span data-ttu-id="d230f-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d230f-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="d230f-145">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="d230f-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="d230f-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d230f-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

