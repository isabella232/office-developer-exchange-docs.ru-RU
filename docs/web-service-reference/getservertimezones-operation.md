---
title: Операция GetServerTimeZones
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 680173e1-e916-466b-b573-5a3182316345
description: Операция GetServerTimeZones возвращает сведения из определений часовых поясов, доступных на сервере Exchange.
ms.openlocfilehash: 9b202d510a599c9082d075228be4c479a2086753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762918"
---
# <a name="getservertimezones-operation"></a><span data-ttu-id="00cd9-103">Операция GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="00cd9-103">GetServerTimeZones operation</span></span>

<span data-ttu-id="00cd9-104">Операция **GetServerTimeZones** возвращает сведения из определений часовых поясов, доступных на сервере Exchange.</span><span class="sxs-lookup"><span data-stu-id="00cd9-104">The **GetServerTimeZones** operation returns information from time zone definitions that are available on an Exchange server.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="00cd9-105">Заголовки SOAP</span><span class="sxs-lookup"><span data-stu-id="00cd9-105">SOAP Headers</span></span>

<span data-ttu-id="00cd9-106">Операция **GetServerTimeZones** может использовать заголовки SOAP, указанные в приведенной ниже таблице и описанные в следующей таблице.</span><span class="sxs-lookup"><span data-stu-id="00cd9-106">The **GetServerTimeZones** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="00cd9-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="00cd9-107">**Header**</span></span>|<span data-ttu-id="00cd9-108">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="00cd9-108">**Element**</span></span>|<span data-ttu-id="00cd9-109">**Описание**</span><span class="sxs-lookup"><span data-stu-id="00cd9-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="00cd9-110">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="00cd9-110">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="00cd9-111">маилбокскултуре</span><span class="sxs-lookup"><span data-stu-id="00cd9-111">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="00cd9-112">Определяет язык и региональные параметры RFC3066, которые будут использоваться для доступа к почтовому ящику.</span><span class="sxs-lookup"><span data-stu-id="00cd9-112">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="00cd9-113">рекуестверсион</span><span class="sxs-lookup"><span data-stu-id="00cd9-113">RequestVersion</span></span>  <br/> |[<span data-ttu-id="00cd9-114">рекуестсерверверсион</span><span class="sxs-lookup"><span data-stu-id="00cd9-114">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="00cd9-115">Определяет версию схемы для запроса операции.</span><span class="sxs-lookup"><span data-stu-id="00cd9-115">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="00cd9-116">серверверсион</span><span class="sxs-lookup"><span data-stu-id="00cd9-116">ServerVersion</span></span>  <br/> |[<span data-ttu-id="00cd9-117">серверверсионинфо</span><span class="sxs-lookup"><span data-stu-id="00cd9-117">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="00cd9-118">Определяет версию сервера, который ответил на запрос.</span><span class="sxs-lookup"><span data-stu-id="00cd9-118">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getservertimezones-request-examples"></a><span data-ttu-id="00cd9-119">Примеры запросов GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="00cd9-119">GetServerTimeZones request examples</span></span>

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a><span data-ttu-id="00cd9-120">Извлечение имени и идентификатора каждого часового пояса</span><span class="sxs-lookup"><span data-stu-id="00cd9-120">Getting the Name and Identifier of Each Time Zone</span></span>

<span data-ttu-id="00cd9-121">В приведенном ниже примере кода показано, как получить имя и идентификатор для часовых поясов стандартного времени и тихоокеанского стандартного времени США.</span><span class="sxs-lookup"><span data-stu-id="00cd9-121">The following code example shows how to retrieve the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="00cd9-122">Код</span><span class="sxs-lookup"><span data-stu-id="00cd9-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="false">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
        <t:Id>Pacific Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="00cd9-123">Comments</span><span class="sxs-lookup"><span data-stu-id="00cd9-123">Comments</span></span>

<span data-ttu-id="00cd9-124">Каждый элемент [ID (TimeZone)](id-timezone.md) содержит идентификатор запрашиваемого определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="00cd9-124">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="00cd9-125">Чтобы запросить сведения для всех часовых поясов, исключите из запроса элемент [ID](ids.md) .</span><span class="sxs-lookup"><span data-stu-id="00cd9-125">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a><span data-ttu-id="00cd9-126">Полное определение каждого часового пояса</span><span class="sxs-lookup"><span data-stu-id="00cd9-126">Getting the Full Definition of Each Time Zone</span></span>

<span data-ttu-id="00cd9-127">В приведенном ниже примере кода показано, как получить полное определение часового пояса для восточного стандартного часового пояса.</span><span class="sxs-lookup"><span data-stu-id="00cd9-127">The following code example shows how to retrieve the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="00cd9-128">Код</span><span class="sxs-lookup"><span data-stu-id="00cd9-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="true">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="00cd9-129">Comments</span><span class="sxs-lookup"><span data-stu-id="00cd9-129">Comments</span></span>

<span data-ttu-id="00cd9-130">Каждый элемент [ID (TimeZone)](id-timezone.md) содержит идентификатор запрашиваемого определения часового пояса.</span><span class="sxs-lookup"><span data-stu-id="00cd9-130">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="00cd9-131">Чтобы запросить сведения для всех часовых поясов, исключите из запроса элемент [ID](ids.md) .</span><span class="sxs-lookup"><span data-stu-id="00cd9-131">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
## <a name="getservertimezones-response-examples"></a><span data-ttu-id="00cd9-132">Примеры ответа GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="00cd9-132">GetServerTimeZones response examples</span></span>

### <a name="receiving-the-time-zone-name-and-identifier-only"></a><span data-ttu-id="00cd9-133">Получение только имени и идентификатора часового пояса</span><span class="sxs-lookup"><span data-stu-id="00cd9-133">Receiving the Time Zone Name and Identifier Only</span></span>

<span data-ttu-id="00cd9-134">В приведенном ниже примере ответа **GetServerTimeZones** показан успешный ответ на запрос **GetServerTimeZones** , в котором для атрибута **ретурнфуллтимезонедата** задано значение **false**.</span><span class="sxs-lookup"><span data-stu-id="00cd9-134">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **false**.</span></span> <span data-ttu-id="00cd9-135">Ответ содержит имя и идентификатор для часовых поясов стандартного времени и тихоокеанского стандартного времени США.</span><span class="sxs-lookup"><span data-stu-id="00cd9-135">The response contains the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="00cd9-136">Код</span><span class="sxs-lookup"><span data-stu-id="00cd9-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)" />
            <t:TimeZoneDefinition Id="Pacific Standard Time" Name="(GMT-08:00) Pacific Time (US &amp;amp; Canada)" />
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="receiving-a-full-time-zone-definition"></a><span data-ttu-id="00cd9-137">Получение определения полного часового пояса</span><span class="sxs-lookup"><span data-stu-id="00cd9-137">Receiving a Full Time Zone Definition</span></span>

<span data-ttu-id="00cd9-138">В приведенном ниже примере ответа **GetServerTimeZones** показан успешный ответ на запрос **GetServerTimeZones** , в котором для атрибута **ретурнфуллтимезонедата** задано **значение true**.</span><span class="sxs-lookup"><span data-stu-id="00cd9-138">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **true**.</span></span> <span data-ttu-id="00cd9-139">Ответ содержит полное определение часового пояса для восточного стандартного часового пояса.</span><span class="sxs-lookup"><span data-stu-id="00cd9-139">The response contains the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="00cd9-140">Код</span><span class="sxs-lookup"><span data-stu-id="00cd9-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)">
              <t:Periods>
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Daylight" />
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Daylight" />
              </t:Periods>
              <t:TransitionsGroups>
                <t:TransitionsGroup Id="0">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>4</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>10</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>-1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
                <t:TransitionsGroup Id="1">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>3</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>2</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>11</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
              </t:TransitionsGroups>
              <t:Transitions>
                <t:Transition>
                  <t:To Kind="Group">0</t:To>
                </t:Transition>
                <t:AbsoluteDateTransition>
                  <t:To Kind="Group">1</t:To>
                  <t:DateTime>2007-01-01T00:00:00</t:DateTime>
                </t:AbsoluteDateTransition>
              </t:Transitions>
            </t:TimeZoneDefinition>
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="00cd9-141">См. также</span><span class="sxs-lookup"><span data-stu-id="00cd9-141">See also</span></span>



[<span data-ttu-id="00cd9-142">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="00cd9-142">GetServerTimeZones</span></span>](getservertimezones.md)
  
[<span data-ttu-id="00cd9-143">жетсервертимезонесреспонсе</span><span class="sxs-lookup"><span data-stu-id="00cd9-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)
  
 <span data-ttu-id="00cd9-144">**жетсервертимезонестипе**</span><span class="sxs-lookup"><span data-stu-id="00cd9-144">**GetServerTimeZonesType**</span></span>


[<span data-ttu-id="00cd9-145">Операции EWS в Exchange</span><span class="sxs-lookup"><span data-stu-id="00cd9-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="00cd9-146">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="00cd9-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

