---
title: Продолжительность (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: Элемент длительность указывает продолжительность ожидания сообщения об отсутствии на состояние доступен, если элемент OofState задано значение запланировано.
ms.openlocfilehash: 62a5492372fd80173d58e965376b7c8c466825a6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19762235"
---
# <a name="duration-useroofsettings"></a><span data-ttu-id="7a084-103">Продолжительность (UserOofSettings)</span><span class="sxs-lookup"><span data-stu-id="7a084-103">Duration (UserOofSettings)</span></span>

<span data-ttu-id="7a084-104">Элемент **длительность** указывает продолжительность ожидания сообщения об отсутствии на состояние доступен, если элемент [OofState](oofstate.md) задано значение **Запланировано**.</span><span class="sxs-lookup"><span data-stu-id="7a084-104">The **Duration** element specifies the duration that the out of office (OOF) status is enabled if the [OofState](oofstate.md) element is set to **Scheduled**.</span></span>
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 <span data-ttu-id="7a084-105">**Срок действия**</span><span class="sxs-lookup"><span data-stu-id="7a084-105">**Duration**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a084-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="7a084-106">Attributes and elements</span></span>

<span data-ttu-id="7a084-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="7a084-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a084-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="7a084-108">Attributes</span></span>

<span data-ttu-id="7a084-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="7a084-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7a084-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="7a084-110">Child elements</span></span>

|<span data-ttu-id="7a084-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a084-111">**Element**</span></span>|<span data-ttu-id="7a084-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a084-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a084-113">Время начала</span><span class="sxs-lookup"><span data-stu-id="7a084-113">StartTime</span></span>](starttime.md) <br/> |<span data-ttu-id="7a084-114">Представляет начало интервала времени задайте со статусом об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="7a084-114">Represents the start of the time span set with an OOF status.</span></span> <span data-ttu-id="7a084-115">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a084-115">This element is required.</span></span>  <br/> |
|[<span data-ttu-id="7a084-116">Время окончания</span><span class="sxs-lookup"><span data-stu-id="7a084-116">EndTime</span></span>](endtime.md) <br/> |<span data-ttu-id="7a084-117">Представляет окончания интервала времени задайте со статусом об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="7a084-117">Represents the end of the time span set with an OOF status.</span></span> <span data-ttu-id="7a084-118">Этот элемент обязательный.</span><span class="sxs-lookup"><span data-stu-id="7a084-118">This element is required.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a084-119">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="7a084-119">Parent elements</span></span>

|<span data-ttu-id="7a084-120">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="7a084-120">**Element**</span></span>|<span data-ttu-id="7a084-121">**Описание**</span><span class="sxs-lookup"><span data-stu-id="7a084-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a084-122">UserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7a084-122">UserOofSettings</span></span>](useroofsettings.md) <br/> |<span data-ttu-id="7a084-123">Задает параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="7a084-123">Specifies the OOF settings.</span></span>  <br/><br/><span data-ttu-id="7a084-124">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7a084-124">The following is the XPath expression to this element:</span></span><br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[<span data-ttu-id="7a084-125">OofSettings</span><span class="sxs-lookup"><span data-stu-id="7a084-125">OofSettings</span></span>](oofsettings.md) <br/> |<span data-ttu-id="7a084-126">Содержит параметры об отсутствии на работе.</span><span class="sxs-lookup"><span data-stu-id="7a084-126">Contains the OOF settings.</span></span><br/><br/><span data-ttu-id="7a084-127">Ниже приведен выражение XPath для этого элемента.</span><span class="sxs-lookup"><span data-stu-id="7a084-127">The following is the XPath expression to this element:</span></span><br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[<span data-ttu-id="7a084-128">Нет на месте</span><span class="sxs-lookup"><span data-stu-id="7a084-128">OutOfOffice</span></span>](outofoffice.md) <br/> |<span data-ttu-id="7a084-129">Определяет ответное сообщение об отсутствии на работе Office (OOF) и время для отправки сообщения ответа для почтового ящика.</span><span class="sxs-lookup"><span data-stu-id="7a084-129">Defines the Out of Office (OOF) response message and a duration time for sending the response message for a mailbox.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a084-130">Замечания</span><span class="sxs-lookup"><span data-stu-id="7a084-130">Remarks</span></span>

<span data-ttu-id="7a084-131">Тип **длительность** также является типом элементов [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [значение TimeWindow](timewindow.md)и [Нет на месте](outofoffice.md) .</span><span class="sxs-lookup"><span data-stu-id="7a084-131">The **Duration** type is also the type for the [DetailedSuggestionsWindow](detailedsuggestionswindow.md), [TimeWindow](timewindow.md), and [OutOfOffice](outofoffice.md) elements.</span></span> 
  
<span data-ttu-id="7a084-132">Схема, описывающая этот элемент, находится в виртуальном каталоге IIS, в котором размещены веб-службы Exchange.</span><span class="sxs-lookup"><span data-stu-id="7a084-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="example"></a><span data-ttu-id="7a084-133">Пример</span><span class="sxs-lookup"><span data-stu-id="7a084-133">Example</span></span>

<span data-ttu-id="7a084-134">В следующем примере [SetUserOofSettings операция](setuseroofsettings-operation.md) запроса задает [OofState](oofstate.md) **включено**, внешних и внутренних сообщений об отсутствии на работе и задает длительность об отсутствии на работе для 10 дней.</span><span class="sxs-lookup"><span data-stu-id="7a084-134">The following example of a [SetUserOofSettings operation](setuseroofsettings-operation.md) request sets the [OofState](oofstate.md) to **Enabled**, the internal and external OOF messages, and sets the duration of OOF for 10 days.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a><span data-ttu-id="7a084-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="7a084-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a084-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="7a084-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7a084-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="7a084-137">Schema Name</span></span>  <br/> |<span data-ttu-id="7a084-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="7a084-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="7a084-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="7a084-139">Validation File</span></span>  <br/> |<span data-ttu-id="7a084-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7a084-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7a084-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="7a084-141">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a084-142">False</span><span class="sxs-lookup"><span data-stu-id="7a084-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a084-143">См. также</span><span class="sxs-lookup"><span data-stu-id="7a084-143">See also</span></span>

- [<span data-ttu-id="7a084-144">Операция GetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7a084-144">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)  
- [<span data-ttu-id="7a084-145">Операция SetUserOofSettings</span><span class="sxs-lookup"><span data-stu-id="7a084-145">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)

