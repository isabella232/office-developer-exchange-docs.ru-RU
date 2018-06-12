---
title: Время начала
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
description: Элемент StartTime представляет Пуск промежуток времени.
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19835560"
---
# <a name="starttime"></a><span data-ttu-id="a6198-103">Время начала</span><span class="sxs-lookup"><span data-stu-id="a6198-103">StartTime</span></span>

<span data-ttu-id="a6198-104">Элемент **StartTime** представляет Пуск промежуток времени.</span><span class="sxs-lookup"><span data-stu-id="a6198-104">The **StartTime** element represents the start of a time span.</span></span> 
  
```xml
<StartTime/
```

<span data-ttu-id="a6198-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="a6198-105">**dateTime**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a6198-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="a6198-106">Attributes and elements</span></span>

<span data-ttu-id="a6198-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="a6198-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6198-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="a6198-108">Attributes</span></span>

<span data-ttu-id="a6198-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="a6198-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6198-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="a6198-110">Child elements</span></span>

<span data-ttu-id="a6198-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="a6198-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6198-112">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="a6198-112">Parent elements</span></span>

|<span data-ttu-id="a6198-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="a6198-113">**Element**</span></span>|<span data-ttu-id="a6198-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="a6198-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6198-115">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="a6198-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="a6198-116">Определяет период времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="a6198-116">Identifies the time span queried for the user availability information.</span></span>  <br/><br/> <span data-ttu-id="a6198-117">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a6198-117">The following is the XPath expression to this element:</span></span>  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[<span data-ttu-id="a6198-118">DetailedSuggestionsWindow</span><span class="sxs-lookup"><span data-stu-id="a6198-118">DetailedSuggestionsWindow</span></span>](detailedsuggestionswindow.md) <br/> |<span data-ttu-id="a6198-119">Определяет период времени, который будет опрошен на наличие подробные сведения о времени предложенного собрания.</span><span class="sxs-lookup"><span data-stu-id="a6198-119">Identifies the time span that is queried for detailed information about suggested meeting times.</span></span>  <br/><br/> <span data-ttu-id="a6198-120">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a6198-120">The following is the XPath expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[<span data-ttu-id="a6198-121">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="a6198-121">Duration (UserOofSettings)</span></span>](duration-useroofsettings.md) <br/> | <span data-ttu-id="a6198-122">Указывает, во время выполнения, для которого включен состояние об отсутствии на работе Office (OOF), если элемент [OofState](oofstate.md) задано значение **расписанию**.</span><span class="sxs-lookup"><span data-stu-id="a6198-122">Specifies the duration for which the Out of Office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>  <br/><br/>  <span data-ttu-id="a6198-123">Ниже приведены возможные выражения XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a6198-123">The following are the possible XPath expressions to this element:</span></span> <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[<span data-ttu-id="a6198-124">CalendarEvent</span><span class="sxs-lookup"><span data-stu-id="a6198-124">CalendarEvent</span></span>](calendarevent.md) <br/> |<span data-ttu-id="a6198-125">Представляет вхождение элемента уникальный календаря.</span><span class="sxs-lookup"><span data-stu-id="a6198-125">Represents a unique calendar item occurrence.</span></span> <span data-ttu-id="a6198-126">Используется для обеспечения доступности запросы.</span><span class="sxs-lookup"><span data-stu-id="a6198-126">This is used for Availability inquiries.</span></span> <span data-ttu-id="a6198-127">Элемент **StartTime** является обязательным в элементе **CalendarEvent** .</span><span class="sxs-lookup"><span data-stu-id="a6198-127">The **StartTime** element is required in the **CalendarEvent** element.</span></span> <span data-ttu-id="a6198-128">**Время начала** элемент в элементе **CalendarEvent** является уникальным для типа **CalendarEvent** , несмотря на то, что он содержит те же значения аспекта, которые содержат элементы **StartTime** в тип **длительность** .</span><span class="sxs-lookup"><span data-stu-id="a6198-128">The **StartTime** element in the **CalendarEvent** element is unique to the **CalendarEvent** type although it contains the same facet values that the **StartTime** elements in the **Duration** type contain.</span></span>  <br/><br/> <span data-ttu-id="a6198-129">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="a6198-129">The following is the XPath expression to this element:</span></span>  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6198-130">Текстовое значение</span><span class="sxs-lookup"><span data-stu-id="a6198-130">Text value</span></span>

<span data-ttu-id="a6198-131">Текстовое значение является обязательным.</span><span class="sxs-lookup"><span data-stu-id="a6198-131">A text value is required.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a6198-132">Замечания</span><span class="sxs-lookup"><span data-stu-id="a6198-132">Remarks</span></span>

<span data-ttu-id="a6198-133">Элемент [EndTime](endtime.md) представляет конец периода времени.</span><span class="sxs-lookup"><span data-stu-id="a6198-133">The [EndTime](endtime.md) element represents the end of the time span.</span></span> 
  
<span data-ttu-id="a6198-134">Схема включает в себя многие [StartTime](starttime.md) элементы.</span><span class="sxs-lookup"><span data-stu-id="a6198-134">The schema includes many [StartTime](starttime.md) elements.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a6198-135">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="a6198-135">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="a6198-136">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="a6198-136">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6198-137">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="a6198-137">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a6198-138">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="a6198-138">Schema Name</span></span>  <br/> |<span data-ttu-id="a6198-139">Схема Types</span><span class="sxs-lookup"><span data-stu-id="a6198-139">Types schema</span></span>  <br/> |
|<span data-ttu-id="a6198-140">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="a6198-140">Validation File</span></span>  <br/> |<span data-ttu-id="a6198-141">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a6198-141">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a6198-142">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="a6198-142">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6198-143">False</span><span class="sxs-lookup"><span data-stu-id="a6198-143">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6198-144">См. также</span><span class="sxs-lookup"><span data-stu-id="a6198-144">See also</span></span>

- [<span data-ttu-id="a6198-145">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="a6198-145">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="a6198-146">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="a6198-146">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

