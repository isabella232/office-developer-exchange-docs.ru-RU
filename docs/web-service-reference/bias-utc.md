---
title: Сдвиг (UTC)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: 15790d5a-5134-457b-8f2b-d9dee1f807a2
description: Элемент сдвига представляет общее смещение от времени в формате UTC. Это значение представлено в минутах.
ms.openlocfilehash: d95284aa28e59542d1a1ee40686163138b015702
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460248"
---
# <a name="bias-utc"></a><span data-ttu-id="da35a-104">Сдвиг (UTC)</span><span class="sxs-lookup"><span data-stu-id="da35a-104">Bias (UTC)</span></span>

<span data-ttu-id="da35a-105">Элемент **сдвига** представляет общее смещение от времени в формате UTC.</span><span class="sxs-lookup"><span data-stu-id="da35a-105">The **Bias** element represents the general offset from Coordinated Universal Time (UTC).</span></span> <span data-ttu-id="da35a-106">Это значение представлено в минутах.</span><span class="sxs-lookup"><span data-stu-id="da35a-106">This value is in minutes.</span></span> 
  
```xml
<TimeZone>
   <Bias>int</Bias>
</TimeZone>
```

<span data-ttu-id="da35a-107">**int**</span><span class="sxs-lookup"><span data-stu-id="da35a-107">**int**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="da35a-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="da35a-108">Attributes and elements</span></span>

<span data-ttu-id="da35a-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="da35a-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="da35a-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="da35a-110">Attributes</span></span>

<span data-ttu-id="da35a-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da35a-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="da35a-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="da35a-112">Child elements</span></span>

<span data-ttu-id="da35a-113">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="da35a-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="da35a-114">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="da35a-114">Parent elements</span></span>

|<span data-ttu-id="da35a-115">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="da35a-115">**Element**</span></span>|<span data-ttu-id="da35a-116">**Описание**</span><span class="sxs-lookup"><span data-stu-id="da35a-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="da35a-117">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="da35a-117">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> | <span data-ttu-id="da35a-118">Контейнер, который определяет сведения о дате и времени для запроса.</span><span class="sxs-lookup"><span data-stu-id="da35a-118">The container that identifies the date-time information of the request.</span></span> <span data-ttu-id="da35a-119">Этот элемент содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="da35a-119">This element contains information about the transition between standard time and daylight saving time.</span></span>  <br/><br/><span data-ttu-id="da35a-120">Ниже приведены выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="da35a-120">The following are the XPath expressions to this element:</span></span><br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="da35a-121">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="da35a-121">Text value</span></span>

<span data-ttu-id="da35a-122">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="da35a-122">A text value is required.</span></span> <span data-ttu-id="da35a-123">Текстовое значение представляет целое число.</span><span class="sxs-lookup"><span data-stu-id="da35a-123">The text value represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="da35a-124">Примечания</span><span class="sxs-lookup"><span data-stu-id="da35a-124">Remarks</span></span>

<span data-ttu-id="da35a-125">Второй элемент [сдвига](bias.md) в схеме представляет смещение от смещения относительно всеобщего скоординированного времени (UTC).</span><span class="sxs-lookup"><span data-stu-id="da35a-125">A second [Bias](bias.md) element in the schema represents the offset from the Coordinated Universal Time (UTC) offset.</span></span> 
  
## <a name="example"></a><span data-ttu-id="da35a-126">Пример</span><span class="sxs-lookup"><span data-stu-id="da35a-126">Example</span></span>

<span data-ttu-id="da35a-127">В приведенном ниже примере показана часть XML-запроса, которая определяет смещение в 8 часов от времени в формате UTC для клиентского приложения.</span><span class="sxs-lookup"><span data-stu-id="da35a-127">The following example shows part of an XML request that identifies an offset of 8 hours from UTC on the client application.</span></span>
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a><span data-ttu-id="da35a-128">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="da35a-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="da35a-129">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="da35a-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="da35a-130">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="da35a-130">Schema Name</span></span>  <br/> |<span data-ttu-id="da35a-131">Схема Types</span><span class="sxs-lookup"><span data-stu-id="da35a-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="da35a-132">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="da35a-132">Validation File</span></span>  <br/> |<span data-ttu-id="da35a-133">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="da35a-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="da35a-134">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="da35a-134">Can be Empty</span></span>  <br/> |<span data-ttu-id="da35a-135">False</span><span class="sxs-lookup"><span data-stu-id="da35a-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="da35a-136">См. также</span><span class="sxs-lookup"><span data-stu-id="da35a-136">See also</span></span>

- [<span data-ttu-id="da35a-137">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="da35a-137">GetUserAvailability operation</span></span>](getuseravailability-operation.md)  
- [<span data-ttu-id="da35a-138">Bias</span><span class="sxs-lookup"><span data-stu-id="da35a-138">Bias</span></span>](bias.md)
- [<span data-ttu-id="da35a-139">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="da35a-139">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

