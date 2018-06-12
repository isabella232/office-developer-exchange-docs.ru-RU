---
title: Операции GetItem (элемента календаря)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItem
api_type:
- schema
ms.assetid: a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8
description: Операции GetItem получает элементы календаря из хранилища Exchange.
ms.openlocfilehash: 69bce0f0cc7b5c986f9bf4767c3cd429a309e50d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19762820"
---
# <a name="getitem-operation-calendar-item"></a><span data-ttu-id="5b408-103">Операции GetItem (элемента календаря)</span><span class="sxs-lookup"><span data-stu-id="5b408-103">GetItem operation (calendar item)</span></span>

<span data-ttu-id="5b408-104">Операции GetItem получает элементы календаря из хранилища Exchange.</span><span class="sxs-lookup"><span data-stu-id="5b408-104">The GetItem operation gets calendar items from the Exchange store.</span></span>
  
## <a name="getitem-request-example"></a><span data-ttu-id="5b408-105">Пример запроса GetItem</span><span class="sxs-lookup"><span data-stu-id="5b408-105">GetItem request example</span></span>

### <a name="description"></a><span data-ttu-id="5b408-106">Описание</span><span class="sxs-lookup"><span data-stu-id="5b408-106">Description</span></span>

<span data-ttu-id="5b408-107">В следующем примере запрос GetItem показано, как для формирования запроса для получения удостоверения и Тема элемента.</span><span class="sxs-lookup"><span data-stu-id="5b408-107">The following example of a GetItem request shows how to form a request to get the identity and subject of an item.</span></span>
  
### <a name="code"></a><span data-ttu-id="5b408-108">Программа</span><span class="sxs-lookup"><span data-stu-id="5b408-108">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetItem xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <ItemIds>
        <t:ItemId Id="AsdD89=" ChangeKey="Jajs3=="/>
      </ItemIds>
    </GetItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="request-elements"></a><span data-ttu-id="5b408-109">Элементы запроса</span><span class="sxs-lookup"><span data-stu-id="5b408-109">Request elements</span></span>

<span data-ttu-id="5b408-110">В запросе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5b408-110">The following elements are used in the request:</span></span>
  
- [<span data-ttu-id="5b408-111">GetItem</span><span class="sxs-lookup"><span data-stu-id="5b408-111">GetItem</span></span>](getitem.md)
    
- [<span data-ttu-id="5b408-112">ItemShape</span><span class="sxs-lookup"><span data-stu-id="5b408-112">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="5b408-113">BaseShape</span><span class="sxs-lookup"><span data-stu-id="5b408-113">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="5b408-114">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="5b408-114">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="5b408-115">FieldURI</span><span class="sxs-lookup"><span data-stu-id="5b408-115">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="5b408-116">Что ItemID</span><span class="sxs-lookup"><span data-stu-id="5b408-116">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="5b408-117">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5b408-117">ItemId</span></span>](itemid.md)
    
> [!NOTE]
> <span data-ttu-id="5b408-118">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="5b408-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span> 
  
<span data-ttu-id="5b408-119">Чтобы найти другие параметры для сообщения запроса на выполнение операции GetItem, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="5b408-119">To find other options for the request message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5b408-120">Начать с [GetItem](getitem.md) элемента.</span><span class="sxs-lookup"><span data-stu-id="5b408-120">Start at the [GetItem](getitem.md) element.</span></span> 
  
## <a name="successful-getitem-response"></a><span data-ttu-id="5b408-121">Успешные GetItem ответа</span><span class="sxs-lookup"><span data-stu-id="5b408-121">Successful GetItem Response</span></span>

### <a name="description"></a><span data-ttu-id="5b408-122">Описание</span><span class="sxs-lookup"><span data-stu-id="5b408-122">Description</span></span>

<span data-ttu-id="5b408-123">В следующем примере показано успешного ответа на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="5b408-123">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="5b408-124">Запрос, который создан этот ответ используется IdOnly baseshape.</span><span class="sxs-lookup"><span data-stu-id="5b408-124">The request that created this response used the IdOnly baseshape.</span></span> <span data-ttu-id="5b408-125">В этом примере возвращается в ответе только идентификатор элемента.</span><span class="sxs-lookup"><span data-stu-id="5b408-125">In this example, the response returns only the ID of the item.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="5b408-126">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5b408-126">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b408-127">Код</span><span class="sxs-lookup"><span data-stu-id="5b408-127">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                   xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAd" ChangeKey="otlIqB=="/>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="5b408-128">Описание</span><span class="sxs-lookup"><span data-stu-id="5b408-128">Description</span></span>

<span data-ttu-id="5b408-129">В следующем примере показано успешного ответа на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="5b408-129">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="5b408-130">Запрос, который создан этот ответ используется baseshape по умолчанию.</span><span class="sxs-lookup"><span data-stu-id="5b408-130">The request that created this response used the Default baseshape.</span></span> <span data-ttu-id="5b408-131">В этом примере возвращается в ответе фигуры по умолчанию для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="5b408-131">In this example, the response returns the Default shape for a calendar item.</span></span>
  
> [!NOTE]
> <span data-ttu-id="5b408-132">Идентификатор элемента и изменить ключ URL были сокращены, чтобы сохранить удобочитаемость.</span><span class="sxs-lookup"><span data-stu-id="5b408-132">The item ID and the change key have been shortened to preserve readability.</span></span> 
  
### <a name="code"></a><span data-ttu-id="5b408-133">Код</span><span class="sxs-lookup"><span data-stu-id="5b408-133">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwrt=="/>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="description"></a><span data-ttu-id="5b408-134">Описание</span><span class="sxs-lookup"><span data-stu-id="5b408-134">Description</span></span>

<span data-ttu-id="5b408-135">В следующем примере показано успешного ответа на запрос GetItem.</span><span class="sxs-lookup"><span data-stu-id="5b408-135">The following example shows a successful response to the GetItem request.</span></span> <span data-ttu-id="5b408-136">Запрос, который создан этот ответ используется AllProperties baseshape.</span><span class="sxs-lookup"><span data-stu-id="5b408-136">The request that created this response used the AllProperties baseshape.</span></span> <span data-ttu-id="5b408-137">В этом примере возвращается в ответе фигуры AllProperties для элемента календаря.</span><span class="sxs-lookup"><span data-stu-id="5b408-137">In this example, the response returns the AllProperties shape for a calendar item.</span></span>
  
### <a name="code"></a><span data-ttu-id="5b408-138">Программа</span><span class="sxs-lookup"><span data-stu-id="5b408-138">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <GetItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                     xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:CalendarItem>
              <t:ItemId Id="ASUAdT" ChangeKey="otlIqB=="/>
              <t:ParentFolderId Id="ASUAdT=="/>
              <t:ItemClass>IPM.Appointment</t:ItemClass>
              <t:Sensitivity>Normal</t:Sensitivity>
              <t:Body BodyType="Text"/>
              <t:DateTimeReceived>2006-06-16T00:12:41Z</t:DateTimeReceived>
              <t:Size>374</t:Size>
              <t:Importance>Normal</t:Importance>
              <t:IsSubmitted>false</t:IsSubmitted>
              <t:IsDraft>false</t:IsDraft>
              <t:IsFromMe>false</t:IsFromMe>
              <t:IsResend>false</t:IsResend>
              <t:IsUnmodified>false</t:IsUnmodified>
              <t:DateTimeSent>2006-06-16T00:12:41Z</t:DateTimeSent>
              <t:DateTimeCreated>2006-06-16T00:12:41Z</t:DateTimeCreated>
              <t:ResponseObjects>
                <t:ForwardItem/>
              </t:ResponseObjects>
              <t:ReminderDueBy>2006-06-16T00:30:00Z</t:ReminderDueBy>
              <t:ReminderIsSet>true</t:ReminderIsSet>
              <t:ReminderMinutesBeforeStart>15</t:ReminderMinutesBeforeStart>
              <t:DisplayCc/>
              <t:DisplayTo/>
              <t:HasAttachments>false</t:HasAttachments>
              <t:Culture>en-US</t:Culture>
              <t:Start>2006-06-16T00:30:00Z</t:Start>
              <t:End>2006-06-16T01:00:00Z</t:End>
              <t:IsAllDayEvent>false</t:IsAllDayEvent>
              <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
              <t:IsMeeting>false</t:IsMeeting>
              <t:IsCancelled>false</t:IsCancelled>
              <t:IsRecurring>false</t:IsRecurring>
              <t:MeetingRequestWasSent>false</t:MeetingRequestWasSent>
              <t:CalendarItemType>Single</t:CalendarItemType>
              <t:MyResponseType>Organizer</t:MyResponseType>
              <t:Organizer>
                <t:Mailbox>
                  <t:Name>Bob</t:Name>
                  <t:EmailAddress>someone@example.com</t:EmailAddress>
                  <t:RoutingType>SMTP</t:RoutingType>
                </t:Mailbox>
              </t:Organizer>
              <t:ConflictingMeetingCount>2</t:ConflictingMeetingCount>
              <t:AdjacentMeetingCount>0</t:AdjacentMeetingCount>
              <t:ConflictingMeetings>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAdTB" ChangeKey="otlIqBwr=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
                <t:CalendarItem>
                  <t:ItemId Id="ASUAd" ChangeKey="otlIqBw=="/>
                  <t:Subject/>
                  <t:Start>2006-06-16T00:30:00Z</t:Start>
                  <t:End>2006-06-16T01:00:00Z</t:End>
                  <t:LegacyFreeBusyStatus>Busy</t:LegacyFreeBusyStatus>
                  <t:Location/>
                </t:CalendarItem>
              </t:ConflictingMeetings>
              <t:Duration>PT30M</t:Duration>
              <t:TimeZone>Pacific Standard Time</t:TimeZone>
              <t:AppointmentSequenceNumber>0</t:AppointmentSequenceNumber>
              <t:AppointmentState>0</t:AppointmentState>
            </t:CalendarItem>
          </m:Items>
        </m:GetItemResponseMessage>
      </m:ResponseMessages>
    </GetItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="5b408-139">Комментарии</span><span class="sxs-lookup"><span data-stu-id="5b408-139">Comments</span></span>

<span data-ttu-id="5b408-140">Чтобы найти другие параметры в сообщении ответа операции GetItem, изучите иерархия схемы.</span><span class="sxs-lookup"><span data-stu-id="5b408-140">To find other options for the response message of the GetItem operation, explore the schema hierarchy.</span></span> <span data-ttu-id="5b408-141">Запустите в элементе [GetItemResponse](getitemresponse.md) .</span><span class="sxs-lookup"><span data-stu-id="5b408-141">Start at the [GetItemResponse](getitemresponse.md) element.</span></span> 
  
### <a name="successful-response-elements"></a><span data-ttu-id="5b408-142">Элементы успешного ответа</span><span class="sxs-lookup"><span data-stu-id="5b408-142">Successful response elements</span></span>

<span data-ttu-id="5b408-143">В ответе используются следующие элементы:</span><span class="sxs-lookup"><span data-stu-id="5b408-143">The following elements are used in the response:</span></span>
  
- [<span data-ttu-id="5b408-144">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="5b408-144">ServerVersionInfo</span></span>](serverversioninfo.md)
    
- [<span data-ttu-id="5b408-145">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="5b408-145">GetItemResponse</span></span>](getitemresponse.md)
    
- [<span data-ttu-id="5b408-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5b408-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="5b408-147">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5b408-147">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
    
- [<span data-ttu-id="5b408-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5b408-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="5b408-149">Элементы</span><span class="sxs-lookup"><span data-stu-id="5b408-149">Items</span></span>](items.md)
    
- [<span data-ttu-id="5b408-150">Элемента календаря, имеющего</span><span class="sxs-lookup"><span data-stu-id="5b408-150">CalendarItem</span></span>](calendaritem.md)
    
- [<span data-ttu-id="5b408-151">Идентификатор элемента</span><span class="sxs-lookup"><span data-stu-id="5b408-151">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="5b408-152">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="5b408-152">ParentFolderId</span></span>](parentfolderid.md)
    
- [<span data-ttu-id="5b408-153">ItemClass</span><span class="sxs-lookup"><span data-stu-id="5b408-153">ItemClass</span></span>](itemclass.md)
    
- [<span data-ttu-id="5b408-154">Уровень конфиденциальности сообщения</span><span class="sxs-lookup"><span data-stu-id="5b408-154">Sensitivity</span></span>](sensitivity.md)
    
- [<span data-ttu-id="5b408-155">Body</span><span class="sxs-lookup"><span data-stu-id="5b408-155">Body</span></span>](body.md)
    
- [<span data-ttu-id="5b408-156">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="5b408-156">DateTimeReceived</span></span>](datetimereceived.md)
    
- [<span data-ttu-id="5b408-157">Размер</span><span class="sxs-lookup"><span data-stu-id="5b408-157">Size</span></span>](size.md)
    
- [<span data-ttu-id="5b408-158">Важность</span><span class="sxs-lookup"><span data-stu-id="5b408-158">Importance</span></span>](importance.md)
    
- [<span data-ttu-id="5b408-159">IsSubmitted</span><span class="sxs-lookup"><span data-stu-id="5b408-159">IsSubmitted</span></span>](issubmitted.md)
    
- [<span data-ttu-id="5b408-160">IsDraft</span><span class="sxs-lookup"><span data-stu-id="5b408-160">IsDraft</span></span>](isdraft.md)
    
- [<span data-ttu-id="5b408-161">IsFromMe</span><span class="sxs-lookup"><span data-stu-id="5b408-161">IsFromMe</span></span>](isfromme.md)
    
- [<span data-ttu-id="5b408-162">IsResend</span><span class="sxs-lookup"><span data-stu-id="5b408-162">IsResend</span></span>](isresend.md)
    
- [<span data-ttu-id="5b408-163">IsUnmodified</span><span class="sxs-lookup"><span data-stu-id="5b408-163">IsUnmodified</span></span>](isunmodified.md)
    
- [<span data-ttu-id="5b408-164">DateTimeSent</span><span class="sxs-lookup"><span data-stu-id="5b408-164">DateTimeSent</span></span>](datetimesent.md)
    
- [<span data-ttu-id="5b408-165">DateTimeCreated</span><span class="sxs-lookup"><span data-stu-id="5b408-165">DateTimeCreated</span></span>](datetimecreated.md)
    
- [<span data-ttu-id="5b408-166">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="5b408-166">ResponseObjects</span></span>](responseobjects.md)
    
- [<span data-ttu-id="5b408-167">ForwardItem</span><span class="sxs-lookup"><span data-stu-id="5b408-167">ForwardItem</span></span>](forwarditem.md)
    
- [<span data-ttu-id="5b408-168">ReminderDueBy</span><span class="sxs-lookup"><span data-stu-id="5b408-168">ReminderDueBy</span></span>](reminderdueby.md)
    
- [<span data-ttu-id="5b408-169">ReminderIsSet</span><span class="sxs-lookup"><span data-stu-id="5b408-169">ReminderIsSet</span></span>](reminderisset.md)
    
- [<span data-ttu-id="5b408-170">ReminderMinutesBeforeStart</span><span class="sxs-lookup"><span data-stu-id="5b408-170">ReminderMinutesBeforeStart</span></span>](reminderminutesbeforestart.md)
    
- [<span data-ttu-id="5b408-171">DisplayCc</span><span class="sxs-lookup"><span data-stu-id="5b408-171">DisplayCc</span></span>](displaycc.md)
    
- [<span data-ttu-id="5b408-172">DisplayTo</span><span class="sxs-lookup"><span data-stu-id="5b408-172">DisplayTo</span></span>](displayto.md)
    
- [<span data-ttu-id="5b408-173">HasAttachments</span><span class="sxs-lookup"><span data-stu-id="5b408-173">HasAttachments</span></span>](hasattachments.md)
    
- [<span data-ttu-id="5b408-174">Язык и региональные параметры</span><span class="sxs-lookup"><span data-stu-id="5b408-174">Culture</span></span>](culture.md)
    
- [<span data-ttu-id="5b408-175">Start</span><span class="sxs-lookup"><span data-stu-id="5b408-175">Start</span></span>](start.md)
    
- [<span data-ttu-id="5b408-176">End</span><span class="sxs-lookup"><span data-stu-id="5b408-176">End </span></span>](end-ex15websvcsotherref.md)
    
- [<span data-ttu-id="5b408-177">IsAllDayEvent</span><span class="sxs-lookup"><span data-stu-id="5b408-177">IsAllDayEvent</span></span>](isalldayevent.md)
    
- [<span data-ttu-id="5b408-178">LegacyFreeBusyStatus</span><span class="sxs-lookup"><span data-stu-id="5b408-178">LegacyFreeBusyStatus</span></span>](legacyfreebusystatus.md)
    
- [<span data-ttu-id="5b408-179">IsMeeting</span><span class="sxs-lookup"><span data-stu-id="5b408-179">IsMeeting</span></span>](ismeeting.md)
    
- [<span data-ttu-id="5b408-180">IsCancelled</span><span class="sxs-lookup"><span data-stu-id="5b408-180">IsCancelled</span></span>](iscancelled.md)
    
- [<span data-ttu-id="5b408-181">IsRecurring</span><span class="sxs-lookup"><span data-stu-id="5b408-181">IsRecurring</span></span>](isrecurring.md)
    
- [<span data-ttu-id="5b408-182">MeetingRequestWasSent</span><span class="sxs-lookup"><span data-stu-id="5b408-182">MeetingRequestWasSent</span></span>](meetingrequestwassent.md)
    
- [<span data-ttu-id="5b408-183">CalendarItemType</span><span class="sxs-lookup"><span data-stu-id="5b408-183">CalendarItemType</span></span>](calendaritemtype.md)
    
- [<span data-ttu-id="5b408-184">MyResponseType</span><span class="sxs-lookup"><span data-stu-id="5b408-184">MyResponseType</span></span>](myresponsetype.md)
    
- [<span data-ttu-id="5b408-185">Организатор</span><span class="sxs-lookup"><span data-stu-id="5b408-185">Organizer</span></span>](organizer.md)
    
- [<span data-ttu-id="5b408-186">Mailbox</span><span class="sxs-lookup"><span data-stu-id="5b408-186">Mailbox</span></span>](mailbox.md)
    
- [<span data-ttu-id="5b408-187">Имя (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5b408-187">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="5b408-188">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="5b408-188">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="5b408-189">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="5b408-189">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="5b408-190">ConflictingMeetingCount</span><span class="sxs-lookup"><span data-stu-id="5b408-190">ConflictingMeetingCount</span></span>](conflictingmeetingcount.md)
    
- [<span data-ttu-id="5b408-191">AdjacentMeetingCount</span><span class="sxs-lookup"><span data-stu-id="5b408-191">AdjacentMeetingCount</span></span>](adjacentmeetingcount.md)
    
- [<span data-ttu-id="5b408-192">ConflictingMeetings</span><span class="sxs-lookup"><span data-stu-id="5b408-192">ConflictingMeetings</span></span>](conflictingmeetings.md)
    
- [<span data-ttu-id="5b408-193">Location</span><span class="sxs-lookup"><span data-stu-id="5b408-193">Location</span></span>](location.md)
    
- [<span data-ttu-id="5b408-194">Продолжительность (элементы)</span><span class="sxs-lookup"><span data-stu-id="5b408-194">Duration (Items)</span></span>](duration-items.md)
    
- [<span data-ttu-id="5b408-195">Часовой пояс (элемент)</span><span class="sxs-lookup"><span data-stu-id="5b408-195">TimeZone (Item)</span></span>](timezone-item.md)
    
- [<span data-ttu-id="5b408-196">AppointmentSequenceNumber</span><span class="sxs-lookup"><span data-stu-id="5b408-196">AppointmentSequenceNumber</span></span>](appointmentsequencenumber.md)
    
- [<span data-ttu-id="5b408-197">AppointmentState</span><span class="sxs-lookup"><span data-stu-id="5b408-197">AppointmentState</span></span>](appointmentstate.md)
    
## <a name="see-also"></a><span data-ttu-id="5b408-198">См. также</span><span class="sxs-lookup"><span data-stu-id="5b408-198">See also</span></span>



[<span data-ttu-id="5b408-199">GetItem Operation</span><span class="sxs-lookup"><span data-stu-id="5b408-199">GetItem operation</span></span>](getitem-operation.md)

