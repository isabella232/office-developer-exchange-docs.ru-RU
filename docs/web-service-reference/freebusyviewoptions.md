---
title: FreeBusyViewOptions
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
description: Элемент FreeBusyViewOptions указывает тип сведений о доступности, возвращаемого в ответе.
ms.openlocfilehash: 703fc6a3625d24cf874a785600e13ee4505b506f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762663"
---
# <a name="freebusyviewoptions"></a><span data-ttu-id="d4d40-103">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="d4d40-103">FreeBusyViewOptions</span></span>

<span data-ttu-id="d4d40-104">Элемент **FreeBusyViewOptions** указывает тип сведений о доступности, возвращаемого в ответе.</span><span class="sxs-lookup"><span data-stu-id="d4d40-104">The **FreeBusyViewOptions** element specifies the type of free/busy information returned in the response.</span></span> 
  
[<span data-ttu-id="d4d40-105">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d4d40-105">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)
  
[<span data-ttu-id="d4d40-106">FreeBusyViewOptions</span><span class="sxs-lookup"><span data-stu-id="d4d40-106">FreeBusyViewOptions</span></span>](freebusyviewoptions.md)
  
```xml
<FreeBusyViewOptions>
   <TimeWindow>...</TimeWindow>
   <MergedFreeBusyIntervalInMinutes>...</MergedFreeBusyIntervalInMinutes>
<RequestedView>...</RequestedView>
</FreeBusyViewOptions>

```

 <span data-ttu-id="d4d40-107">**FreeBusyViewOptionsType**</span><span class="sxs-lookup"><span data-stu-id="d4d40-107">**FreeBusyViewOptionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d4d40-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d4d40-108">Attributes and elements</span></span>

<span data-ttu-id="d4d40-109">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d4d40-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4d40-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d4d40-110">Attributes</span></span>

<span data-ttu-id="d4d40-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="d4d40-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d4d40-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d4d40-112">Child elements</span></span>

|<span data-ttu-id="d4d40-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4d40-113">**Element**</span></span>|<span data-ttu-id="d4d40-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4d40-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4d40-115">Значение TimeWindow</span><span class="sxs-lookup"><span data-stu-id="d4d40-115">TimeWindow</span></span>](timewindow.md) <br/> |<span data-ttu-id="d4d40-116">Определяет период времени, запрос пользователя сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="d4d40-116">Identifies the time span queried for the user availability information.</span></span>  <br/> |
|[<span data-ttu-id="d4d40-117">MergedFreeBusyIntervalInMinutes</span><span class="sxs-lookup"><span data-stu-id="d4d40-117">MergedFreeBusyIntervalInMinutes</span></span>](mergedfreebusyintervalinminutes.md) <br/> |<span data-ttu-id="d4d40-118">Представляет разницу между двумя последовательными разъемов **FreeBusyMerged** представления.</span><span class="sxs-lookup"><span data-stu-id="d4d40-118">Represents the time difference between two successive slots in the **FreeBusyMerged** view.</span></span>  <br/> |
|[<span data-ttu-id="d4d40-119">RequestedView</span><span class="sxs-lookup"><span data-stu-id="d4d40-119">RequestedView</span></span>](requestedview.md) <br/> |<span data-ttu-id="d4d40-120">Задает тип данных календаря, для которого запрашивается клиента.</span><span class="sxs-lookup"><span data-stu-id="d4d40-120">Defines the type of calendar information that a client requests.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d4d40-121">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d4d40-121">Parent elements</span></span>

|<span data-ttu-id="d4d40-122">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d4d40-122">**Element**</span></span>|<span data-ttu-id="d4d40-123">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d4d40-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4d40-124">GetUserAvailabilityRequest</span><span class="sxs-lookup"><span data-stu-id="d4d40-124">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md) <br/> |<span data-ttu-id="d4d40-125">Содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="d4d40-125">Contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="d4d40-126">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="d4d40-126">This is a root element.</span></span>  <br/> <span data-ttu-id="d4d40-127">XPath для этого элемента:</span><span class="sxs-lookup"><span data-stu-id="d4d40-127">The following is the XPath to this element:</span></span>  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4d40-128">Замечания</span><span class="sxs-lookup"><span data-stu-id="d4d40-128">Remarks</span></span>

<span data-ttu-id="d4d40-129">Этот элемент не является обязательным и можно только один раз при использовании.</span><span class="sxs-lookup"><span data-stu-id="d4d40-129">This element is not required and can only occur once if used.</span></span> <span data-ttu-id="d4d40-130">Это значение может быть null, если значение элемента [SuggestionsViewOptions](suggestionsviewoptions.md) не равно null.</span><span class="sxs-lookup"><span data-stu-id="d4d40-130">This value can be null if the value of the [SuggestionsViewOptions](suggestionsviewoptions.md) element is not null.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d4d40-131">Схема, описывающая этот элемент находится в каталоге /epi/ компьютера, на котором выполняется Microsoft® Exchange Server 2007 с установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d4d40-131">The schema that describes this element is located in the /epi/ directory of the computer that is running Microsoft® Exchange Server 2007 that has the Client Access server role installed.</span></span> 
  
## <a name="example"></a><span data-ttu-id="d4d40-132">Пример</span><span class="sxs-lookup"><span data-stu-id="d4d40-132">Example</span></span>

<span data-ttu-id="d4d40-133">В следующем примере извлекается список собраний и потока сведений о доступности в интервалы — 60 минут.</span><span class="sxs-lookup"><span data-stu-id="d4d40-133">The following example obtains a list of meetings and a free/busy stream in 60-minute intervals.</span></span>
  
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

## <a name="element-information"></a><span data-ttu-id="d4d40-134">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d4d40-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4d40-135">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d4d40-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4d40-136">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d4d40-136">Schema Name</span></span>  <br/> |<span data-ttu-id="d4d40-137">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d4d40-137">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4d40-138">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d4d40-138">Validation File</span></span>  <br/> |<span data-ttu-id="d4d40-139">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4d40-139">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4d40-140">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d4d40-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="d4d40-141">False</span><span class="sxs-lookup"><span data-stu-id="d4d40-141">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4d40-142">См. также</span><span class="sxs-lookup"><span data-stu-id="d4d40-142">See also</span></span>



[<span data-ttu-id="d4d40-143">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="d4d40-143">GetUserAvailability operation</span></span>](getuseravailability-operation.md)


[<span data-ttu-id="d4d40-144">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="d4d40-144">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

