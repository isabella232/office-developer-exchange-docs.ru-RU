---
title: жетусераваилабилитиреспонсе
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserAvailabilityResponse
api_type:
- schema
ms.assetid: 6999510a-d60e-43da-8964-57b5fb3e9d11
description: Элемент Жетусераваилабилитиреспонсе является корневым элементом, содержащим свойства, которые определяют сведения о доступности пользователей или сведения о предложенном времени проведения собрания.
ms.openlocfilehash: 0a30dc8ebc11b1f818b2c27b0ea68fc135ec0925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833684"
---
# <a name="getuseravailabilityresponse"></a><span data-ttu-id="60fdb-103">жетусераваилабилитиреспонсе</span><span class="sxs-lookup"><span data-stu-id="60fdb-103">GetUserAvailabilityResponse</span></span>

<span data-ttu-id="60fdb-104">Элемент **жетусераваилабилитиреспонсе** является корневым элементом, содержащим свойства, которые определяют сведения о доступности пользователей или сведения о предложенном времени проведения собрания.</span><span class="sxs-lookup"><span data-stu-id="60fdb-104">The **GetUserAvailabilityResponse** element is the root element that contains the properties that define user availability information or suggested meeting time information.</span></span> 
  
```xml
<GetUserAvailabilityResponse>
   <FreeBusyResponseArray>...</FreeBusyResponseArray>
   <SuggestionsResponse>...</SuggestionsResponse>
</GetUserAvailabilityResponse>
```

 <span data-ttu-id="60fdb-105">**жетусераваилабилитиреспонсетипе**</span><span class="sxs-lookup"><span data-stu-id="60fdb-105">**GetUserAvailabilityResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60fdb-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="60fdb-106">Attributes and elements</span></span>

<span data-ttu-id="60fdb-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="60fdb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60fdb-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="60fdb-108">Attributes</span></span>

<span data-ttu-id="60fdb-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="60fdb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60fdb-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="60fdb-110">Child elements</span></span>

|<span data-ttu-id="60fdb-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="60fdb-111">**Element**</span></span>|<span data-ttu-id="60fdb-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="60fdb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60fdb-113">фрибусиреспонсеаррай</span><span class="sxs-lookup"><span data-stu-id="60fdb-113">FreeBusyResponseArray</span></span>](freebusyresponsearray.md) <br/> |<span data-ttu-id="60fdb-114">Содержит сведения о доступности запрошенных пользователей и состояние отклика.</span><span class="sxs-lookup"><span data-stu-id="60fdb-114">Contains the requested users' availability information and the response status.</span></span>  <br/> |
|[<span data-ttu-id="60fdb-115">сугжестионсреспонсе</span><span class="sxs-lookup"><span data-stu-id="60fdb-115">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="60fdb-116">Содержит сведения о состоянии отклика и сведения о предложении для запрошенных предложений о собрании.</span><span class="sxs-lookup"><span data-stu-id="60fdb-116">Contains response status information and suggestion data for requested meeting suggestions.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60fdb-117">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="60fdb-117">Parent elements</span></span>

<span data-ttu-id="60fdb-118">Нет.</span><span class="sxs-lookup"><span data-stu-id="60fdb-118">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="60fdb-119">Примечания</span><span class="sxs-lookup"><span data-stu-id="60fdb-119">Remarks</span></span>

<span data-ttu-id="60fdb-120">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="60fdb-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="example"></a><span data-ttu-id="60fdb-121">Пример</span><span class="sxs-lookup"><span data-stu-id="60fdb-121">Example</span></span>

<span data-ttu-id="60fdb-122">В приведенном ниже примере ответа GetUserAvailability показан ответ на запрос GetUserAvailability.</span><span class="sxs-lookup"><span data-stu-id="60fdb-122">The following example of a GetUserAvailability response shows a response to a GetUserAvailability request.</span></span>
  
```
<?xml version="1.0" encoding="utf-8" ?>
<GetUserAvailabilityResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <FreeBusyResponseArray xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <FreeBusyResponse>
      <ResponseMessage ResponseClass="Success">
        <Path select="/m:GetUserAvailabilityRequest/MailboxDataArray[0]" />
      </ResponseMessage>
      <FreeBusyView>
        <FreeBusyViewType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Detailed</FreeBusyViewType>
        <CalendarEventArray xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <CalendarEvent>
            <StartTime>2006-02-28T19:00:00-08:00</StartTime>
            <EndTime>2006-02-28T23:30:00-08:00</EndTime>
            <BusyType>OOF</BusyType>
            <IsPrivate>false</IsPrivate>
            <CalendarEventDetails>
              <ID>00000</ID>
              <Subject>Exercise</Subject>
              <Location>the gym</Location>
              <IsMeeting>false</IsMeeting>
              <IsRecurring>false</IsRecurring>
              <IsException>false</IsException>
              <IsReminderSet>true</IsReminderSet>
            </CalendarEventDetails>
          </CalendarEvent>
        </CalendarEventArray>
        <WorkingHours xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <TimeZone>
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
          <WorkingPeriodArray>
            <WorkingPeriod>
              <DayOfWeek>Monday Tuesday Wednesday Thursday Friday</DayOfWeek>
              <StartTimeInMinutes>480</StartTimeInMinutes>
              <EndTimeInMinutes>1020</EndTimeInMinutes>
            </WorkingPeriod>
          </WorkingPeriodArray>
        </WorkingHours>
      </FreeBusyView>
    </FreeBusyResponse>
  </FreeBusyResponseArray>
</GetUserAvailabilityResponse>
```

<span data-ttu-id="60fdb-123">Содержимое элемента [ID](id.md) было сокращено, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="60fdb-123">The [ID](id.md) element contents were shortened to preserve readability.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="60fdb-124">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="60fdb-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60fdb-125">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="60fdb-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="60fdb-126">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="60fdb-126">Schema Name</span></span>  <br/> |<span data-ttu-id="60fdb-127">Схема Messages</span><span class="sxs-lookup"><span data-stu-id="60fdb-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="60fdb-128">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="60fdb-128">Validation File</span></span>  <br/> |<span data-ttu-id="60fdb-129">Messages. xsd</span><span class="sxs-lookup"><span data-stu-id="60fdb-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="60fdb-130">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="60fdb-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="60fdb-131">False</span><span class="sxs-lookup"><span data-stu-id="60fdb-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="60fdb-132">См. также</span><span class="sxs-lookup"><span data-stu-id="60fdb-132">See also</span></span>



[<span data-ttu-id="60fdb-133">жетусераваилабилитирекуест</span><span class="sxs-lookup"><span data-stu-id="60fdb-133">GetUserAvailabilityRequest</span></span>](getuseravailabilityrequest.md)


[<span data-ttu-id="60fdb-134">Getting User Availability</span><span class="sxs-lookup"><span data-stu-id="60fdb-134">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

