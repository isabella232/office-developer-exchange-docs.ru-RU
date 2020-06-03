---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: Элемент StartTime представляет начало интервала времени.
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458567"
---
# <a name="starttime"></a><span data-ttu-id="32a1b-103">StartTime</span><span class="sxs-lookup"><span data-stu-id="32a1b-103">StartTime</span></span>

<span data-ttu-id="32a1b-104">Элемент **StartTime** представляет начало интервала времени.</span><span class="sxs-lookup"><span data-stu-id="32a1b-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="32a1b-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="32a1b-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="32a1b-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="32a1b-106">Attributes and elements</span></span>

<span data-ttu-id="32a1b-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="32a1b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32a1b-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="32a1b-108">Attributes</span></span>

<span data-ttu-id="32a1b-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="32a1b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="32a1b-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="32a1b-110">Child elements</span></span>

<span data-ttu-id="32a1b-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="32a1b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="32a1b-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="32a1b-112">Parent elements</span></span>

|<span data-ttu-id="32a1b-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="32a1b-113">**Element**</span></span>|<span data-ttu-id="32a1b-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="32a1b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32a1b-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="32a1b-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="32a1b-116">Определяет интервал времени, запрошенный для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="32a1b-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="32a1b-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="32a1b-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="32a1b-118">детаиледсугжестионсвиндов</span><span class="sxs-lookup"><span data-stu-id="32a1b-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="32a1b-119">Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="32a1b-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="32a1b-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="32a1b-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="32a1b-121">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="32a1b-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="32a1b-122">Указывает срок, в течение которого состояние отсутствия на работе (отсутствие на работе) включается, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".</span><span class="sxs-lookup"><span data-stu-id="32a1b-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="32a1b-123">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="32a1b-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="32a1b-124">календаревент</span><span class="sxs-lookup"><span data-stu-id="32a1b-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="32a1b-125">Представляет уникальное вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="32a1b-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="32a1b-126">Используется для запросов о доступности.</span><span class="sxs-lookup"><span data-stu-id="32a1b-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="32a1b-127">Элемент **StartTime** необходим в элементе **календаревент** .</span><span class="sxs-lookup"><span data-stu-id="32a1b-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="32a1b-128">Элемент **StartTime** в элементе **календаревент** уникален для типа **календаревент** , несмотря на то, что он содержит те же значения аспекта, что и элементы **StartTime** в типе **Duration** .</span><span class="sxs-lookup"><span data-stu-id="32a1b-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="32a1b-129">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="32a1b-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="32a1b-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="32a1b-130">Text value</span></span>

<span data-ttu-id="32a1b-131">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="32a1b-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="32a1b-132">Примечания</span><span class="sxs-lookup"><span data-stu-id="32a1b-132">Remarks</span></span>

<span data-ttu-id="32a1b-133">Элемент [EndTime](endtime.md) представляет конец интервала времени.</span><span class="sxs-lookup"><span data-stu-id="32a1b-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="32a1b-134">Схема включает множество элементов [StartTime](starttime.md) .</span><span class="sxs-lookup"><span data-stu-id="32a1b-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="32a1b-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="32a1b-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="32a1b-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="32a1b-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32a1b-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="32a1b-137">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="32a1b-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="32a1b-138">Schema Name</span></span>  <br/> |<span data-ttu-id="32a1b-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="32a1b-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="32a1b-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="32a1b-140">Validation File</span></span>  <br/> |<span data-ttu-id="32a1b-141">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="32a1b-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="32a1b-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="32a1b-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="32a1b-143">False</span><span class="sxs-lookup"><span data-stu-id="32a1b-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32a1b-144">См. также</span><span class="sxs-lookup"><span data-stu-id="32a1b-144">See also</span></span>

- [<span data-ttu-id="32a1b-145">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="32a1b-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="32a1b-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="32a1b-146">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

