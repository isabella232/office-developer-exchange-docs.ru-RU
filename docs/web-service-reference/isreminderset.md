---
title: Попамятка
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsReminderSet
api_type:
- schema
ms.assetid: 6aea4cb7-ca14-4949-8e7f-660b565f6556
description: Элемент "набор напоминаний" указывает, задано ли напоминание для события календаря.
ms.openlocfilehash: 589178072baca652bff2779e64a212fb90478247
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19834100"
---
# <a name="isreminderset"></a><span data-ttu-id="da4b6-103">Попамятка</span><span class="sxs-lookup"><span data-stu-id="da4b6-103">IsReminderSet</span></span>

<span data-ttu-id="da4b6-104">Элемент "набор **напоминаний** " указывает, задано ли напоминание для события календаря.</span><span class="sxs-lookup"><span data-stu-id="da4b6-104">The **IsReminderSet** element indicates whether a reminder has been set for the calendar event.</span></span> 
  
[<span data-ttu-id="da4b6-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="da4b6-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="da4b6-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="da4b6-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="da4b6-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="da4b6-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="da4b6-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="da4b6-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="da4b6-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="da4b6-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="da4b6-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="da4b6-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="da4b6-111">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="da4b6-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="da4b6-112">Попамятка</span><span class="sxs-lookup"><span data-stu-id="da4b6-112">IsReminderSet</span></span>](isreminderset.md)
  
```xml
<IsReminderSet>true or false</IsReminderSet>
```

 <span data-ttu-id="da4b6-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="da4b6-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="da4b6-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da4b6-114">Attributes and elements</span></span>

<span data-ttu-id="da4b6-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="da4b6-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da4b6-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da4b6-116">Attributes</span></span>

<span data-ttu-id="da4b6-117">Нет.</span><span class="sxs-lookup"><span data-stu-id="da4b6-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da4b6-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da4b6-118">Child elements</span></span>

<span data-ttu-id="da4b6-119">Нет.</span><span class="sxs-lookup"><span data-stu-id="da4b6-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da4b6-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da4b6-120">Parent elements</span></span>

|<span data-ttu-id="da4b6-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da4b6-121">**Element**</span></span>|<span data-ttu-id="da4b6-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da4b6-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da4b6-123">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="da4b6-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="da4b6-124">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="da4b6-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="da4b6-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="da4b6-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da4b6-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="da4b6-126">Text value</span></span>

<span data-ttu-id="da4b6-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="da4b6-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="da4b6-128">Этот элемент является обязательным, если используется элемент [календаревентдетаилс](calendareventdetails.md) , если для элемента- [частного](isprivate.md) задано значение **true**.</span><span class="sxs-lookup"><span data-stu-id="da4b6-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used unless the [IsPrivate](isprivate.md) element is set to **true**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da4b6-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="da4b6-129">Remarks</span></span>

<span data-ttu-id="da4b6-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="da4b6-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="da4b6-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da4b6-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da4b6-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da4b6-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da4b6-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da4b6-133">Schema Name</span></span>  <br/> |<span data-ttu-id="da4b6-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da4b6-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="da4b6-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da4b6-135">Validation File</span></span>  <br/> |<span data-ttu-id="da4b6-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="da4b6-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da4b6-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da4b6-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="da4b6-138">False</span><span class="sxs-lookup"><span data-stu-id="da4b6-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da4b6-139">См. также</span><span class="sxs-lookup"><span data-stu-id="da4b6-139">See also</span></span>



[<span data-ttu-id="da4b6-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="da4b6-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="da4b6-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="da4b6-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="da4b6-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="da4b6-142">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

