---
title: жетусераваилабилитирекуест
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityRequest
api_type:
- schema
ms.assetid: 7906711b-80a1-42ae-8b33-26eeac036a5a
description: Элемент Жетусераваилабилитирекуест содержит аргументы, используемые для получения сведений о доступности пользователя. Это корневой элемент.
ms.openlocfilehash: 5440f739b09bfbe27ad97cba99c08756686594f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833683"
---
# <a name="getuseravailabilityrequest"></a><span data-ttu-id="57410-104">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="57410-104">GetUserAvailabilityRequest</span></span>

<span data-ttu-id="57410-105">Элемент **жетусераваилабилитирекуест** содержит аргументы, используемые для получения сведений о доступности пользователя.</span><span class="sxs-lookup"><span data-stu-id="57410-105">The **GetUserAvailabilityRequest** element contains the arguments used to obtain user availability information.</span></span> <span data-ttu-id="57410-106">Это корневой элемент.</span><span class="sxs-lookup"><span data-stu-id="57410-106">This is a root element.</span></span> 
  
```xml
<GetUserAvailabilityRequest>
   <TimeZone>...</TimeZone>
   <MailboxDataArray>...</MailboxDataArray>
   <FreeBusyViewOptions>...</FreeBusyViewOptions>
   <SuggestionsViewOptions>...</SuggestionsViewOptions>
</GetUserAvailabilityRequest>
```

 <span data-ttu-id="57410-107">**жетусераваилабилитирекуесттипе**</span><span class="sxs-lookup"><span data-stu-id="57410-107">**GetUserAvailabilityRequestType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57410-108">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="57410-108">Attributes and elements</span></span>

<span data-ttu-id="57410-109">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="57410-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57410-110">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="57410-110">Attributes</span></span>

<span data-ttu-id="57410-111">Нет.</span><span class="sxs-lookup"><span data-stu-id="57410-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57410-112">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="57410-112">Child elements</span></span>

|<span data-ttu-id="57410-113">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="57410-113">**Element**</span></span>|<span data-ttu-id="57410-114">**Описание**</span><span class="sxs-lookup"><span data-stu-id="57410-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57410-115">Часовой пояс (доступность)</span><span class="sxs-lookup"><span data-stu-id="57410-115">TimeZone (Availability)</span></span>](timezone-availability.md) <br/> |<span data-ttu-id="57410-116">Содержит элементы, определяющие сведения о часовом поясе.</span><span class="sxs-lookup"><span data-stu-id="57410-116">Contains elements that identify time zone information.</span></span> <span data-ttu-id="57410-117">Этот элемент также содержит сведения о переходе со стандартного времени на летнее время.</span><span class="sxs-lookup"><span data-stu-id="57410-117">This element also contains information about the transition between standard time and daylight saving time.</span></span>  <br/> |
|[<span data-ttu-id="57410-118">маилбоксдатааррай</span><span class="sxs-lookup"><span data-stu-id="57410-118">MailboxDataArray</span></span>](mailboxdataarray.md) <br/> |<span data-ttu-id="57410-119">Содержит список почтовых ящиков, в которых запрашиваются сведения о доступности.</span><span class="sxs-lookup"><span data-stu-id="57410-119">Contains a list of mailboxes to query for availability information.</span></span>  <br/> |
|[<span data-ttu-id="57410-120">фрибусивиевоптионс</span><span class="sxs-lookup"><span data-stu-id="57410-120">FreeBusyViewOptions</span></span>](freebusyviewoptions.md) <br/> |<span data-ttu-id="57410-121">Указывает тип сведений о доступности, возвращаемых в ответе.</span><span class="sxs-lookup"><span data-stu-id="57410-121">Specifies the type of free/busy information returned in the response.</span></span>  <br/> |
|[<span data-ttu-id="57410-122">сугжестионсвиевоптионс</span><span class="sxs-lookup"><span data-stu-id="57410-122">SuggestionsViewOptions</span></span>](suggestionsviewoptions.md) <br/> |<span data-ttu-id="57410-123">Содержит параметры для получения сведений о предложении собрания.</span><span class="sxs-lookup"><span data-stu-id="57410-123">Contains the options for obtaining meeting suggestion information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57410-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="57410-124">Parent elements</span></span>

<span data-ttu-id="57410-125">Нет.</span><span class="sxs-lookup"><span data-stu-id="57410-125">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57410-126">Примечания</span><span class="sxs-lookup"><span data-stu-id="57410-126">Remarks</span></span>

<span data-ttu-id="57410-127">Схема, описывающая этот элемент, находится в каталоге/ЕВС/компьютера под управлением Microsoft Exchange Server 2007, на котором установлена роль сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="57410-127">The schema that describes this element is located in the /EWS/ directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="57410-128">Пример</span><span class="sxs-lookup"><span data-stu-id="57410-128">Example</span></span>

<span data-ttu-id="57410-129">В приведенном ниже примере показан запрос сведений о доступности.</span><span class="sxs-lookup"><span data-stu-id="57410-129">The following example shows a request for free/busy information.</span></span>
  
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
            <Address>someone@exchangeserver.example.com</Address>
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
          <EndTime>2006-02-30T23:59:59</EndTime>
        </TimeWindow>
        <MergedFreeBusyIntervalInMinutes>60</MergedFreeBusyIntervalInMinutes>
        <RequestedView>FreeBusyMerged</RequestedView>
      </FreeBusyViewOptions>
    </GetUserAvailabilityRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="57410-130">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="57410-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57410-131">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="57410-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57410-132">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="57410-132">Schema Name</span></span>  <br/> |<span data-ttu-id="57410-133">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="57410-133">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57410-134">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="57410-134">Validation File</span></span>  <br/> |<span data-ttu-id="57410-135">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="57410-135">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57410-136">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="57410-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="57410-137">False</span><span class="sxs-lookup"><span data-stu-id="57410-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57410-138">См. также</span><span class="sxs-lookup"><span data-stu-id="57410-138">See also</span></span>



[<span data-ttu-id="57410-139">Операция GetUserAvailability</span><span class="sxs-lookup"><span data-stu-id="57410-139">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
  
[<span data-ttu-id="57410-140">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="57410-140">GetUserAvailabilityResponse</span></span>](getuseravailabilityresponse.md)


[<span data-ttu-id="57410-141">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="57410-141">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

