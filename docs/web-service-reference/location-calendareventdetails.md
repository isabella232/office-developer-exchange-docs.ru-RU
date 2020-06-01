---
title: Местоположение (Календаревентдетаилс)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Location
api_type:
- schema
ms.assetid: 883cce6e-66b8-4dbc-935c-83ef5100a953
description: Элемент Location представляет поле расположения элемента календаря.
ms.openlocfilehash: 4a590c315d2211ce9128305a514e68f1c785596c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468000"
---
# <a name="location-calendareventdetails"></a><span data-ttu-id="00268-103">Местоположение (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="00268-103">Location (CalendarEventDetails)</span></span>

<span data-ttu-id="00268-104">Элемент **Location** представляет поле расположения элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="00268-104">The **Location** element represents the location field of the calendar item.</span></span> 
  
[<span data-ttu-id="00268-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="00268-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="00268-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="00268-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="00268-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="00268-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="00268-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="00268-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="00268-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="00268-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="00268-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="00268-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="00268-111">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="00268-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="00268-112">Местоположение (Календаревентдетаилс)</span><span class="sxs-lookup"><span data-stu-id="00268-112">Location (CalendarEventDetails)</span></span>](location-calendareventdetails.md)
  
```xml
<Location/>
```

 <span data-ttu-id="00268-113">**строка**</span><span class="sxs-lookup"><span data-stu-id="00268-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00268-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="00268-114">Attributes and elements</span></span>

<span data-ttu-id="00268-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="00268-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00268-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="00268-116">Attributes</span></span>

<span data-ttu-id="00268-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="00268-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00268-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="00268-118">Child elements</span></span>

<span data-ttu-id="00268-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="00268-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00268-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="00268-120">Parent elements</span></span>

|<span data-ttu-id="00268-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="00268-121">**Element**</span></span>|<span data-ttu-id="00268-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00268-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00268-123">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="00268-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="00268-124">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="00268-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="00268-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="00268-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00268-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="00268-126">Text value</span></span>

<span data-ttu-id="00268-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="00268-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="00268-128">Этот элемент может содержать пустую строку.</span><span class="sxs-lookup"><span data-stu-id="00268-128">This element can contain an empty string.</span></span> <span data-ttu-id="00268-129">Этот элемент является необязательным, если используется элемент [календаревентдетаилс](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="00268-129">This element is optional if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="00268-130">Примечания</span><span class="sxs-lookup"><span data-stu-id="00268-130">Remarks</span></span>

<span data-ttu-id="00268-131">Этот элемент сопоставлен с именованным свойством PR_Location MAPI.</span><span class="sxs-lookup"><span data-stu-id="00268-131">This element maps to a PR_Location MAPI named property.</span></span>
  
<span data-ttu-id="00268-132">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="00268-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00268-133">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="00268-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00268-134">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="00268-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="00268-135">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="00268-135">Schema Name</span></span>  <br/> |<span data-ttu-id="00268-136">Схема Types</span><span class="sxs-lookup"><span data-stu-id="00268-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="00268-137">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="00268-137">Validation File</span></span>  <br/> |<span data-ttu-id="00268-138">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="00268-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="00268-139">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="00268-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="00268-140">False</span><span class="sxs-lookup"><span data-stu-id="00268-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00268-141">См. также</span><span class="sxs-lookup"><span data-stu-id="00268-141">See also</span></span>



[<span data-ttu-id="00268-142">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="00268-142">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="00268-143">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="00268-143">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="00268-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="00268-144">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

