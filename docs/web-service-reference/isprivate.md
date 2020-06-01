---
title: Частный
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsPrivate
api_type:
- schema
ms.assetid: 1712bc94-9789-4507-8521-bde1be51e331
description: Элемент ". Private" указывает, является ли элемент календаря частным.
ms.openlocfilehash: c36c659414700439436cd2ca903e443164c1473b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457804"
---
# <a name="isprivate"></a><span data-ttu-id="b803b-103">Частный</span><span class="sxs-lookup"><span data-stu-id="b803b-103">IsPrivate</span></span>

<span data-ttu-id="b803b-104">Элемент ". **Private** " указывает, является ли элемент календаря частным.</span><span class="sxs-lookup"><span data-stu-id="b803b-104">The **IsPrivate** element indicates whether the calendar item is private.</span></span> 
  
[<span data-ttu-id="b803b-105">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b803b-105">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)
  
[<span data-ttu-id="b803b-106">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="b803b-106">FreeBusyResponseArray</span></span>](freebusyresponsearray.md)
  
[<span data-ttu-id="b803b-107">фрибусиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b803b-107">FreeBusyResponse</span></span>](freebusyresponse.md)
  
[<span data-ttu-id="b803b-108">фрибусивиев</span><span class="sxs-lookup"><span data-stu-id="b803b-108">FreeBusyView</span></span>](freebusyview.md)
  
[<span data-ttu-id="b803b-109">календаревентаррай</span><span class="sxs-lookup"><span data-stu-id="b803b-109">CalendarEventArray</span></span>](calendareventarray.md)
  
[<span data-ttu-id="b803b-110">календаревент</span><span class="sxs-lookup"><span data-stu-id="b803b-110">CalendarEvent</span></span>](calendarevent.md)
  
[<span data-ttu-id="b803b-111">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="b803b-111">CalendarEventDetails</span></span>](calendareventdetails.md)
  
[<span data-ttu-id="b803b-112">Частный</span><span class="sxs-lookup"><span data-stu-id="b803b-112">IsPrivate</span></span>](isprivate.md)
  
```xml
<IsPrivate>true or false</IsPrivate>
```

 <span data-ttu-id="b803b-113">**boolean**</span><span class="sxs-lookup"><span data-stu-id="b803b-113">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b803b-114">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="b803b-114">Attributes and elements</span></span>

<span data-ttu-id="b803b-115">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="b803b-115">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b803b-116">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="b803b-116">Attributes</span></span>

<span data-ttu-id="b803b-117">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b803b-117">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b803b-118">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="b803b-118">Child elements</span></span>

<span data-ttu-id="b803b-119">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="b803b-119">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b803b-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="b803b-120">Parent elements</span></span>

|<span data-ttu-id="b803b-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="b803b-121">**Element**</span></span>|<span data-ttu-id="b803b-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="b803b-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b803b-123">календаревентдетаилс</span><span class="sxs-lookup"><span data-stu-id="b803b-123">CalendarEventDetails</span></span>](calendareventdetails.md) <br/> |<span data-ttu-id="b803b-124">Предоставляет дополнительные сведения о событии календаря.</span><span class="sxs-lookup"><span data-stu-id="b803b-124">Provides additional information about a calendar event.</span></span>  <br/> <span data-ttu-id="b803b-125">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="b803b-125">The following is the XPath expression to this element:</span></span>  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]/CalendarEventDetails` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b803b-126">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="b803b-126">Text value</span></span>

<span data-ttu-id="b803b-127">Текстовое значение, представляющее логическое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="b803b-127">A text value that represents a Boolean value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b803b-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="b803b-128">Remarks</span></span>

<span data-ttu-id="b803b-129">При использовании этого элемента другие элементы в элементе [календаревентдетаилс](calendareventdetails.md) не будут включены в ответ.</span><span class="sxs-lookup"><span data-stu-id="b803b-129">If this element is used, the other elements in the [CalendarEventDetails](calendareventdetails.md) element will not be included in the response.</span></span> 
  
<span data-ttu-id="b803b-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="b803b-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b803b-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="b803b-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b803b-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="b803b-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b803b-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="b803b-133">Schema Name</span></span>  <br/> |<span data-ttu-id="b803b-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="b803b-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="b803b-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="b803b-135">Validation File</span></span>  <br/> |<span data-ttu-id="b803b-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="b803b-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b803b-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="b803b-137">Can be Empty</span></span>  <br/> |<span data-ttu-id="b803b-138">False</span><span class="sxs-lookup"><span data-stu-id="b803b-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b803b-139">См. также</span><span class="sxs-lookup"><span data-stu-id="b803b-139">See also</span></span>



[<span data-ttu-id="b803b-140">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="b803b-140">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="b803b-141">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="b803b-141">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="b803b-142">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="b803b-142">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

