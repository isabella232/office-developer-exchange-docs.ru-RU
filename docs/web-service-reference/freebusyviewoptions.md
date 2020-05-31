---
title: фрибусивиевоптионс
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FreeBusyViewOptions
api_type:
- schema
ms.assetid: c07f3ddb-874b-4d30-a60e-7e5c7793bb6f
description: Элемент Фрибусивиевоптионс указывает тип сведений о занятости, возвращаемых в ответе.
ms.openlocfilehash: 703fc6a3625d24cf874a785600e13ee4505b506f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762663"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="aff63-103">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="aff63-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="aff63-104">Элемент **фрибусивиевоптионс** указывает тип сведений о занятости, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="aff63-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="aff63-105">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="aff63-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="aff63-106">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="aff63-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="aff63-107">**фрибусивиевоптионстипе**</span><span class="sxs-lookup"><span data-stu-id="aff63-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aff63-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="aff63-108">Attributes and elements</span></span>

<span data-ttu-id="aff63-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="aff63-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aff63-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="aff63-110">Attributes</span></span>

<span data-ttu-id="aff63-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="aff63-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aff63-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="aff63-112">Child elements</span></span>

|<span data-ttu-id="aff63-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aff63-113">**Element**</span></span>|<span data-ttu-id="aff63-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aff63-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aff63-115">TimeWindow</span><span class="sxs-lookup"><span data-stu-id="aff63-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="aff63-116">Определяет интервал времени, запрошенный для сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff63-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="aff63-117">мержедфрибусинтервалинминутес</span><span class="sxs-lookup"><span data-stu-id="aff63-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="aff63-118">Представляет разное время между двумя последовательными слотами в представлении **фрибусимержед** .</span><span class="sxs-lookup"><span data-stu-id="aff63-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="aff63-119">рекуестедвиев</span><span class="sxs-lookup"><span data-stu-id="aff63-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="aff63-120">Определяет тип данных календаря, запрашиваемых клиентом.</span><span class="sxs-lookup"><span data-stu-id="aff63-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="aff63-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="aff63-121">Parent elements</span></span>

|<span data-ttu-id="aff63-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="aff63-122">**Element**</span></span>|<span data-ttu-id="aff63-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="aff63-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aff63-124">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="aff63-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="aff63-125">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="aff63-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="aff63-126">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="aff63-126">This is a root element.</span></span>  <br/> <span data-ttu-id="aff63-127">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="aff63-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="aff63-128">Примечания</span><span class="sxs-lookup"><span data-stu-id="aff63-128">Remarks</span></span>

<span data-ttu-id="aff63-129">Этот элемент не является обязательным и может быть использован только один раз.</span><span class="sxs-lookup"><span data-stu-id="aff63-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="aff63-130">Это значение может быть равно null, если значение элемента [сугжестионсвиевоптионс](suggestionsviewoptions.md) отлично от NULL.</span><span class="sxs-lookup"><span data-stu-id="aff63-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="aff63-131">Схема, описывающая этот элемент, находится в каталоге/ЕПИ/компьютера, на котором работает Microsoft® Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="aff63-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="aff63-132">Пример</span><span class="sxs-lookup"><span data-stu-id="aff63-132">Example</span></span>

<span data-ttu-id="aff63-133">В следующем примере показано получение списка собраний и потока сведений о занятости в 60-минутных интервалах.</span><span class="sxs-lookup"><span data-stu-id="aff63-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
```
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <GetUserAvailabilityRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
      <MailboxDataArray>
        <MailboxData xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Email>
            <Name></Name>
            <Address>someone@ExServer.example.com</Address>
            <RoutingType>SMTP</RoutingType>
          </Email>
          <AttendeeType>Organizer</AttendeeType>
          <ExcludeConflicts>false</ExcludeConflicts>
          <ExcludeNonWorkingHours>false</ExcludeNonWorkingHours>
        </MailboxData>
      </MailboxDataArray>
      <FreeBusyViewOptions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <TimeWindow>
          <StartTime>2006-02-06T00:00:00</StartTime>
          <EndTime>2006-02-25T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="aff63-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="aff63-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aff63-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="aff63-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="aff63-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="aff63-136">Schema Name</span></span>  <br/> |<span data-ttu-id="aff63-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="aff63-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="aff63-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="aff63-138">Validation File</span></span>  <br/> |<span data-ttu-id="aff63-139">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="aff63-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="aff63-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="aff63-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="aff63-141">False</span><span class="sxs-lookup"><span data-stu-id="aff63-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aff63-142">См. также</span><span class="sxs-lookup"><span data-stu-id="aff63-142">See also</span></span>



[<span data-ttu-id="aff63-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="aff63-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="aff63-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="aff63-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

