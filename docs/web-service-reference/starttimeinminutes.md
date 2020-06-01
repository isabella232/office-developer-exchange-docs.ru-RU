---
title: старттимеинминутес
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTimeInMinutes
api_type:
- schema
ms.assetid: 0fb60a78-6e79-4601-8e2f-5bd245c46d69
description: Элемент Старттимеинминутес представляет начало рабочего дня пользователя почтового ящика.
ms.openlocfilehash: b33cb12299a146b577dd17939a0585a15d50fb07
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458532"
---
# <a name="starttimeinminutes"></a><span data-ttu-id="c616f-103">старттимеинминутес</span><span class="sxs-lookup"><span data-stu-id="c616f-103">StartTimeInMinutes</span></span>

<span data-ttu-id="c616f-104">Элемент **старттимеинминутес** представляет начало рабочего дня пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c616f-104">The **StartTimeInMinutes** element represents the start of the working day for a mailbox user.</span></span> 
  
- [<span data-ttu-id="c616f-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c616f-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
- [<span data-ttu-id="c616f-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="c616f-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
- [<span data-ttu-id="c616f-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c616f-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
- [<span data-ttu-id="c616f-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="c616f-108">FreeBusyView</span></span>](freebusyview.md)
  
- [<span data-ttu-id="c616f-109">воркингхаурс</span><span class="sxs-lookup"><span data-stu-id="c616f-109">WorkingHours</span></span>](workinghours-ex15websvcsotherref.md)
  
- [<span data-ttu-id="c616f-110">воркингпериодаррай</span><span class="sxs-lookup"><span data-stu-id="c616f-110">WorkingPeriodArray</span></span>](workingperiodarray.md)
  
- [<span data-ttu-id="c616f-111">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="c616f-111">WorkingPeriod</span></span>](workingperiod.md)
  
- [<span data-ttu-id="c616f-112">старттимеинминутес</span><span class="sxs-lookup"><span data-stu-id="c616f-112">StartTimeInMinutes</span></span>](starttimeinminutes.md)
  
```xml
<StartTimeInMinutes>...</StartTimeInMinutes>
```

<span data-ttu-id="c616f-113">**int**</span><span class="sxs-lookup"><span data-stu-id="c616f-113">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="c616f-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="c616f-114">Attributes and elements</span></span>

<span data-ttu-id="c616f-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="c616f-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c616f-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="c616f-116">Attributes</span></span>

<span data-ttu-id="c616f-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c616f-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c616f-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="c616f-118">Child elements</span></span>

<span data-ttu-id="c616f-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="c616f-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c616f-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="c616f-120">Parent elements</span></span>

|<span data-ttu-id="c616f-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="c616f-121">**Element**</span></span>|<span data-ttu-id="c616f-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="c616f-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c616f-123">воркингпериод</span><span class="sxs-lookup"><span data-stu-id="c616f-123">WorkingPeriod</span></span>](workingperiod.md) <br/> |<span data-ttu-id="c616f-124">Содержит рабочие недели, дни и часы пользователя почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="c616f-124">Contains the work week days and hours of the mailbox user.</span></span>  <br/> <span data-ttu-id="c616f-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="c616f-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c616f-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="c616f-126">Text value</span></span>

<span data-ttu-id="c616f-127">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="c616f-127">A text value is required.</span></span> <span data-ttu-id="c616f-128">Текстовое значение обозначает начало рабочего дня, сколько минут прошло с начала дня.</span><span class="sxs-lookup"><span data-stu-id="c616f-128">The text value represents the start of the working day by how many minutes have elapsed since the day began.</span></span> <span data-ttu-id="c616f-129">Например, время начала 8 часов утра</span><span class="sxs-lookup"><span data-stu-id="c616f-129">For example, a start time of 8 A.M.</span></span> <span data-ttu-id="c616f-130">представляется в виде 480 минут.</span><span class="sxs-lookup"><span data-stu-id="c616f-130">is represented by 480 minutes.</span></span>
  
<span data-ttu-id="c616f-131">Диапазон допустимых значений для этого элемента — от 0 до 1440.</span><span class="sxs-lookup"><span data-stu-id="c616f-131">The range of possible values for this element is 0 to 1440.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c616f-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="c616f-132">Remarks</span></span>

<span data-ttu-id="c616f-133">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="c616f-133">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c616f-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="c616f-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c616f-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="c616f-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c616f-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="c616f-136">Schema Name</span></span>  <br/> |<span data-ttu-id="c616f-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="c616f-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="c616f-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="c616f-138">Validation File</span></span>  <br/> |<span data-ttu-id="c616f-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="c616f-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c616f-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="c616f-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="c616f-141">False</span><span class="sxs-lookup"><span data-stu-id="c616f-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c616f-142">См. также</span><span class="sxs-lookup"><span data-stu-id="c616f-142">See also</span></span>

- [<span data-ttu-id="c616f-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="c616f-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="c616f-144">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="c616f-144">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
- [<span data-ttu-id="c616f-145">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="c616f-145">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

