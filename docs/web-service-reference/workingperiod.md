---
title: воркингпериод
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- WorkingPeriod
api_type:
- schema
ms.assetid: 3b4e48af-9880-42b9-a0dc-dae7ac43c264
description: Элемент Воркингпериод содержит рабочие недели, дни и часы пользователя почтового ящика.
ms.openlocfilehash: 5c217169fb193d4bb6dae4e18570873d55de6127
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459681"
---
# <a name="workingperiod"></a><span data-ttu-id="f932e-103">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="f932e-103">WorkingPeriod</span></span>

<span data-ttu-id="f932e-104">Элемент **воркингпериод** содержит рабочие недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f932e-104">The **WorkingPeriod** element contains the work week days and hours of the mailbox user.</span></span> 
  
[<span data-ttu-id="f932e-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f932e-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="f932e-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="f932e-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="f932e-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f932e-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="f932e-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="f932e-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="f932e-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="f932e-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="f932e-110">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="f932e-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="f932e-111">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="f932e-111">WorkingPeriod</span></span>](workingperiod.md)
  
```xml
<WorkingPeriod>
   <DayOfWeek>...</DayOfWeek>
   <StartTimeInMinutes>...</StartTimeInMinutes>
   <EndTimeInMinutes>...</EndTimeInMinutes>
</WorkingPeriod>
```

 <span data-ttu-id="f932e-112">**воркингпериод**</span><span class="sxs-lookup"><span data-stu-id="f932e-112">**WorkingPeriod**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f932e-113">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="f932e-113">Attributes and elements</span></span>

<span data-ttu-id="f932e-114">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="f932e-114">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f932e-115">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="f932e-115">Attributes</span></span>

<span data-ttu-id="f932e-116">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="f932e-116">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f932e-117">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="f932e-117">Child elements</span></span>

|<span data-ttu-id="f932e-118">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f932e-118">**Element**</span></span>|<span data-ttu-id="f932e-119">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f932e-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f932e-120">DayOfWeek (Воркингпериод)</span><span class="sxs-lookup"><span data-stu-id="f932e-120">DayOfWeek (WorkingPeriod)</span></span>](dayofweek-workingperiod.md) <br/> |<span data-ttu-id="f932e-121">Содержит список рабочих дней, запланированных для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f932e-121">Contains the list of working days scheduled for the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="f932e-122">старттимеинминутес</span><span class="sxs-lookup"><span data-stu-id="f932e-122">StartTimeInMinutes</span></span>](starttimeinminutes.md) <br/> |<span data-ttu-id="f932e-123">Представляет начало рабочего дня для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f932e-123">Represents the start of the working day for a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="f932e-124">ендтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="f932e-124">EndTimeInMinutes</span></span>](endtimeinminutes.md) <br/> |<span data-ttu-id="f932e-125">Представляет конец рабочего дня пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f932e-125">Represents the end of the working day for a mailbox user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f932e-126">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="f932e-126">Parent elements</span></span>

|<span data-ttu-id="f932e-127">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="f932e-127">**Element**</span></span>|<span data-ttu-id="f932e-128">**Описание**</span><span class="sxs-lookup"><span data-stu-id="f932e-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f932e-129">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="f932e-129">WorkingPeriodArray</span></span>](workingperiodarray.md) <br/> |<span data-ttu-id="f932e-130">Содержит сведения о рабочем периоде для пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="f932e-130">Contains working period information for the mailbox user.</span></span>  <br/> <span data-ttu-id="f932e-131">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="f932e-131">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f932e-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="f932e-132">Remarks</span></span>

<span data-ttu-id="f932e-133">Все дочерние элементы перечислены в той последовательности, в которой они выполняются.</span><span class="sxs-lookup"><span data-stu-id="f932e-133">All the child elements are listed in the sequence in which they occur.</span></span> <span data-ttu-id="f932e-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="f932e-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f932e-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="f932e-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f932e-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="f932e-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f932e-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="f932e-137">Schema Name</span></span>  <br/> |<span data-ttu-id="f932e-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="f932e-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="f932e-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="f932e-139">Validation File</span></span>  <br/> |<span data-ttu-id="f932e-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="f932e-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f932e-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="f932e-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="f932e-142">False</span><span class="sxs-lookup"><span data-stu-id="f932e-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f932e-143">См. также</span><span class="sxs-lookup"><span data-stu-id="f932e-143">See also</span></span>



[<span data-ttu-id="f932e-144">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="f932e-144">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="f932e-145">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="f932e-145">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="f932e-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="f932e-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

