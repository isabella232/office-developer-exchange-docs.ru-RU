---
title: ендтимеинминутес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTimeInMinutes
api_type:
- schema
ms.assetid: ef05bdda-7a66-44db-bb73-a2ce8316c257
description: Элемент Ендтимеинминутес представляет конец рабочего дня пользователя почтового ящика.
ms.openlocfilehash: cb564f9de944848734749a30c813a94d6b5c4187
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459653"
---
# <a name="endtimeinminutes"></a><span data-ttu-id="a1d91-103">ендтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="a1d91-103">EndTimeInMinutes</span></span>

<span data-ttu-id="a1d91-104">Элемент **ендтимеинминутес** представляет конец рабочего дня пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a1d91-104">The **EndTimeInMinutes** element represents the end of the working day for a mailbox user.</span></span> 
  
[<span data-ttu-id="a1d91-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1d91-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="a1d91-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="a1d91-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="a1d91-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1d91-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="a1d91-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="a1d91-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="a1d91-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="a1d91-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
[<span data-ttu-id="a1d91-110">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="a1d91-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
[<span data-ttu-id="a1d91-111">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="a1d91-111">WorkingPeriod</span></span>](workingperiod.md)
  
[<span data-ttu-id="a1d91-112">ендтимеинминутес</span><span class="sxs-lookup"><span data-stu-id="a1d91-112">EndTimeInMinutes</span></span>](endtimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

 <span data-ttu-id="a1d91-113">**int**</span><span class="sxs-lookup"><span data-stu-id="a1d91-113">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a1d91-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a1d91-114">Attributes and elements</span></span>

<span data-ttu-id="a1d91-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="a1d91-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a1d91-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a1d91-116">Attributes</span></span>

<span data-ttu-id="a1d91-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1d91-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a1d91-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a1d91-118">Child elements</span></span>

<span data-ttu-id="a1d91-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="a1d91-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a1d91-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a1d91-120">Parent elements</span></span>

|<span data-ttu-id="a1d91-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a1d91-121">**Element**</span></span>|<span data-ttu-id="a1d91-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a1d91-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a1d91-123">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="a1d91-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="a1d91-124">Содержит рабочие недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="a1d91-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="a1d91-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="a1d91-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a1d91-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a1d91-126">Text value</span></span>

<span data-ttu-id="a1d91-127">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="a1d91-127">A text value is required.</span></span> <span data-ttu-id="a1d91-128">Текстовое значение представляет конец рабочего дня, в течение которого прошло несколько минут с момента начала дня.</span><span class="sxs-lookup"><span data-stu-id="a1d91-128">The text value represents the end of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="a1d91-129">Например, время окончания — 6 часов</span><span class="sxs-lookup"><span data-stu-id="a1d91-129">For example, an end time of 6 P.M.</span></span> <span data-ttu-id="a1d91-130">представляется в виде 1080 минут.</span><span class="sxs-lookup"><span data-stu-id="a1d91-130">is represented by 1080 minutes.</span></span>
  
<span data-ttu-id="a1d91-131">Диапазон допустимых значений для этого элемента — от 0 до 1440.</span><span class="sxs-lookup"><span data-stu-id="a1d91-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a1d91-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="a1d91-132">Remarks</span></span>

<span data-ttu-id="a1d91-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a1d91-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a1d91-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a1d91-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a1d91-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a1d91-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a1d91-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a1d91-136">Schema Name</span></span>  <br/> |<span data-ttu-id="a1d91-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a1d91-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="a1d91-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a1d91-138">Validation File</span></span>  <br/> |<span data-ttu-id="a1d91-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="a1d91-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a1d91-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a1d91-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="a1d91-141">False</span><span class="sxs-lookup"><span data-stu-id="a1d91-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a1d91-142">См. также</span><span class="sxs-lookup"><span data-stu-id="a1d91-142">See also</span></span>



[<span data-ttu-id="a1d91-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a1d91-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="a1d91-144">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="a1d91-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="a1d91-145">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a1d91-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

