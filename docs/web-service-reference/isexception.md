---
title: Исключение
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsException
api_type:
- schema
ms.assetid: e7bd8ae2-2643-411e-ae08-358bac445800
description: Элемент "-EXCEPT" указывает, изменяется ли экземпляр повторяющегося элемента календаря с основного.
ms.openlocfilehash: f2e45e0f1010449d4a494f5e15ecd0b22dc598e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457587"
---
# <a name="isexception"></a><span data-ttu-id="ad3f7-103">Исключение</span><span class="sxs-lookup"><span data-stu-id="ad3f7-103">IsException</span></span>

<span data-ttu-id="ad3f7-104">Элемент "- **except** " указывает, изменяется ли экземпляр повторяющегося элемента календаря с основного.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-104">The **IsException** element indicates whether an instance of a recurring calendar item is changed from the master.</span></span> 
  
[<span data-ttu-id="ad3f7-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ad3f7-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="ad3f7-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="ad3f7-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="ad3f7-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ad3f7-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="ad3f7-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="ad3f7-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="ad3f7-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="ad3f7-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="ad3f7-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="ad3f7-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="ad3f7-111">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="ad3f7-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="ad3f7-112">Исключение</span><span class="sxs-lookup"><span data-stu-id="ad3f7-112">IsException</span></span>](isexception.md)
  
```xml
<IsException/>
```

 <span data-ttu-id="ad3f7-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="ad3f7-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ad3f7-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="ad3f7-114">Attributes and elements</span></span>

<span data-ttu-id="ad3f7-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ad3f7-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="ad3f7-116">Attributes</span></span>

<span data-ttu-id="ad3f7-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ad3f7-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="ad3f7-118">Child elements</span></span>

<span data-ttu-id="ad3f7-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ad3f7-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="ad3f7-120">Parent elements</span></span>

|<span data-ttu-id="ad3f7-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="ad3f7-121">**Element**</span></span>|<span data-ttu-id="ad3f7-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="ad3f7-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ad3f7-123">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="ad3f7-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="ad3f7-124">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="ad3f7-125">Ниже приведено выражение XPath 2,0 для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="ad3f7-125">The following is the XPath 2.0 expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ad3f7-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="ad3f7-126">Text value</span></span>

<span data-ttu-id="ad3f7-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="ad3f7-128">Этот элемент является обязательным, если используется элемент [календаревентдетаилс](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="ad3f7-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ad3f7-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="ad3f7-129">Remarks</span></span>

<span data-ttu-id="ad3f7-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="ad3f7-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ad3f7-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="ad3f7-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ad3f7-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="ad3f7-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ad3f7-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="ad3f7-133">Schema Name</span></span>  <br/> |<span data-ttu-id="ad3f7-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="ad3f7-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="ad3f7-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="ad3f7-135">Validation File</span></span>  <br/> |<span data-ttu-id="ad3f7-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="ad3f7-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ad3f7-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="ad3f7-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="ad3f7-138">False</span><span class="sxs-lookup"><span data-stu-id="ad3f7-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ad3f7-139">См. также</span><span class="sxs-lookup"><span data-stu-id="ad3f7-139">See also</span></span>



[<span data-ttu-id="ad3f7-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="ad3f7-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="ad3f7-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="ad3f7-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="ad3f7-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="ad3f7-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

