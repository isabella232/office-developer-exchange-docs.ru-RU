---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: Элемент EndTime представляет конец интервала времени.
ms.openlocfilehash: 5a30b32ecfeafe582cd07dd662aacb0a960257c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462994"
---
# <a name="endtime"></a><span data-ttu-id="646fe-103">EndTime</span><span class="sxs-lookup"><span data-stu-id="646fe-103">EndTime</span></span>

<span data-ttu-id="646fe-104">Элемент **EndTime** представляет конец интервала времени.</span><span class="sxs-lookup"><span data-stu-id="646fe-104">The **EndTime** element represents the end of a time span.</span></span> 
  
```xml
<EndTime>dateTime</EndTime>
```

 <span data-ttu-id="646fe-105">**дата и время**</span><span class="sxs-lookup"><span data-stu-id="646fe-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="646fe-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="646fe-106">Attributes and elements</span></span>

<span data-ttu-id="646fe-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="646fe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="646fe-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="646fe-108">Attributes</span></span>

<span data-ttu-id="646fe-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="646fe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="646fe-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="646fe-110">Child elements</span></span>

<span data-ttu-id="646fe-111">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="646fe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="646fe-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="646fe-112">Parent elements</span></span>

|<span data-ttu-id="646fe-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="646fe-113">**Element**</span></span>|<span data-ttu-id="646fe-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="646fe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="646fe-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="646fe-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="646fe-116">Определяет интервал времени, запрошенный для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="646fe-116">Identifies the time span queried for the user availability information.</span></span><br/><br/> <span data-ttu-id="646fe-117">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="646fe-117">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="646fe-118">детаиледсугжестионсвиндов</span><span class="sxs-lookup"><span data-stu-id="646fe-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="646fe-119">Определяет интервал времени, на который запрашивается подробная информация о предложенном времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="646fe-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span><br/><br/> <span data-ttu-id="646fe-120">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="646fe-120">The following is the XPath expression to this element:</span></span><br/><br/>  <span data-ttu-id="646fe-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span><span class="sxs-lookup"><span data-stu-id="646fe-121">`/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.</span></span>  <br/> |
|[<span data-ttu-id="646fe-122">Продолжительность (Усеруфсеттингс)</span><span class="sxs-lookup"><span data-stu-id="646fe-122">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="646fe-123">Указывает срок, в течение которого состояние отсутствия на работе (отсутствие на работе) включается, если для элемента [уфстате](oofstate.md) задано значение " **запланировано**".</span><span class="sxs-lookup"><span data-stu-id="646fe-123">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="646fe-124">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="646fe-124">The following are the possible XPath expressions to this element:</span></span><br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="646fe-125">Экземпляр</span><span class="sxs-lookup"><span data-stu-id="646fe-125">Occurrence</span></span>](occurrence.md) <br/> |<span data-ttu-id="646fe-126">Представляет один измененный экземпляр повторяющегося элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="646fe-126">Represents a single modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="646fe-127">календаревент</span><span class="sxs-lookup"><span data-stu-id="646fe-127">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="646fe-128">Представляет уникальное вхождение элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="646fe-128">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="646fe-129">Используется для запросов о доступности.</span><span class="sxs-lookup"><span data-stu-id="646fe-129">This is used for Availability inquiries.</span></span> <span data-ttu-id="646fe-130">Элемент **EndTime** необходим в элементе **календаревент** .</span><span class="sxs-lookup"><span data-stu-id="646fe-130">The **EndTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="646fe-131">Элемент **EndTime** в элементе **календаревент** уникален для типа **календаревент** .</span><span class="sxs-lookup"><span data-stu-id="646fe-131">The **EndTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type.</span></span><br/><br/> <span data-ttu-id="646fe-132">Ниже приведено выражение XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="646fe-132">The following is the XPath expression to this element:</span></span><br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="646fe-133">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="646fe-133">Text value</span></span>

<span data-ttu-id="646fe-134">Необходимо указать текстовое значение.</span><span class="sxs-lookup"><span data-stu-id="646fe-134">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="646fe-135">Примечания</span><span class="sxs-lookup"><span data-stu-id="646fe-135">Remarks</span></span>

<span data-ttu-id="646fe-136">Элемент [StartTime](starttime.md) представляет начало интервала времени.</span><span class="sxs-lookup"><span data-stu-id="646fe-136">The [StartTime](starttime.md) element represents the beginning of a time span.</span></span> 
  
<span data-ttu-id="646fe-137">Время окончания представляет время клиента.</span><span class="sxs-lookup"><span data-stu-id="646fe-137">The end time represents the client's time.</span></span>
  
<span data-ttu-id="646fe-138">Схема включает множество элементов [EndTime](endtime.md) .</span><span class="sxs-lookup"><span data-stu-id="646fe-138">The schema includes many [EndTime](endtime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="646fe-139">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="646fe-139">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="646fe-140">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="646fe-140">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="646fe-141">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="646fe-141">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="646fe-142">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="646fe-142">Schema Name</span></span>  <br/> |<span data-ttu-id="646fe-143">Схема Types</span><span class="sxs-lookup"><span data-stu-id="646fe-143">Types schema</span></span>  <br/> |
|<span data-ttu-id="646fe-144">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="646fe-144">Validation File</span></span>  <br/> |<span data-ttu-id="646fe-145">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="646fe-145">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="646fe-146">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="646fe-146">Can be Empty</span></span>  <br/> |<span data-ttu-id="646fe-147">False</span><span class="sxs-lookup"><span data-stu-id="646fe-147">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="646fe-148">См. также</span><span class="sxs-lookup"><span data-stu-id="646fe-148">See also</span></span>

- [<span data-ttu-id="646fe-149">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="646fe-149">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="646fe-150">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="646fe-150">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

