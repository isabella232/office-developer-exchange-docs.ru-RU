---
title: Идентификатор
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ID
api_type:
- schema
ms.assetid: 8caf922f-56bd-466a-a68f-d6cb236f2eec
description: Элемент ID представляет идентификатор записи элемента календаря.
ms.openlocfilehash: 429413bbfb0206effc3ea97eb11527449c67211c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456488"
---
# <a name="id"></a><span data-ttu-id="81c34-103">Идентификатор</span><span class="sxs-lookup"><span data-stu-id="81c34-103">ID</span></span>

<span data-ttu-id="81c34-104">Элемент **ID** представляет идентификатор записи элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="81c34-104">The **ID** element represents the entry ID of the calendar item.</span></span> 
  
[<span data-ttu-id="81c34-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="81c34-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="81c34-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="81c34-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="81c34-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="81c34-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="81c34-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="81c34-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="81c34-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="81c34-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="81c34-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="81c34-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="81c34-111">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="81c34-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="81c34-112">ИД</span><span class="sxs-lookup"><span data-stu-id="81c34-112">ID</span></span>](id.md)
  
```xml
<ID>...</ID>
```

 <span data-ttu-id="81c34-113">**строка**</span><span class="sxs-lookup"><span data-stu-id="81c34-113">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="81c34-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="81c34-114">Attributes and elements</span></span>

<span data-ttu-id="81c34-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="81c34-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="81c34-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="81c34-116">Attributes</span></span>

<span data-ttu-id="81c34-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="81c34-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="81c34-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="81c34-118">Child elements</span></span>

<span data-ttu-id="81c34-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="81c34-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="81c34-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="81c34-120">Parent elements</span></span>

|<span data-ttu-id="81c34-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="81c34-121">**Element**</span></span>|<span data-ttu-id="81c34-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="81c34-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="81c34-123">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="81c34-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="81c34-124">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="81c34-124">Provides additional information for a calendar event.</span></span>  <br/> <span data-ttu-id="81c34-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="81c34-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="81c34-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="81c34-126">Text value</span></span>

<span data-ttu-id="81c34-127">Текстовое значение является обязательным, если этот элемент возвращается в ответе.</span><span class="sxs-lookup"><span data-stu-id="81c34-127">A text value is required if this element is returned in the response.</span></span> <span data-ttu-id="81c34-128">Этот элемент является обязательным, если используется элемент [календаревентдетаилс](calendareventdetails.md) .</span><span class="sxs-lookup"><span data-stu-id="81c34-128">This element is required if the [CalendarEventDetails](calendareventdetails.md) element is used.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="81c34-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="81c34-129">Remarks</span></span>

<span data-ttu-id="81c34-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="81c34-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="81c34-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="81c34-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="81c34-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="81c34-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="81c34-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="81c34-133">Schema Name</span></span>  <br/> |<span data-ttu-id="81c34-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="81c34-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="81c34-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="81c34-135">Validation File</span></span>  <br/> |<span data-ttu-id="81c34-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="81c34-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="81c34-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="81c34-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="81c34-138">False</span><span class="sxs-lookup"><span data-stu-id="81c34-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="81c34-139">См. также</span><span class="sxs-lookup"><span data-stu-id="81c34-139">See also</span></span>



[<span data-ttu-id="81c34-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="81c34-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="81c34-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="81c34-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="81c34-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="81c34-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

