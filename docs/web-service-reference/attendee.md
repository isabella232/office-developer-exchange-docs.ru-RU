---
title: Участник
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: Элемент "участник" представляет участников и ресурсы собрания.
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457650"
---
# <a name="attendee"></a><span data-ttu-id="4d401-103">Участник</span><span class="sxs-lookup"><span data-stu-id="4d401-103">Attendee</span></span>

<span data-ttu-id="4d401-104">Элемент " **участник** " представляет участников и ресурсы собрания.</span><span class="sxs-lookup"><span data-stu-id="4d401-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="4d401-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="4d401-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4d401-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="4d401-106">Attributes and elements</span></span>

<span data-ttu-id="4d401-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="4d401-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4d401-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="4d401-108">Attributes</span></span>

<span data-ttu-id="4d401-109">Отсутствуют.</span><span class="sxs-lookup"><span data-stu-id="4d401-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4d401-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="4d401-110">Child elements</span></span>

|<span data-ttu-id="4d401-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d401-111">**Element**</span></span>|<span data-ttu-id="4d401-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d401-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d401-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="4d401-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="4d401-114">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="4d401-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="4d401-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="4d401-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="4d401-116">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="4d401-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="4d401-117">Это свойство относится только к элементу календаря организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="4d401-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4d401-118">ластреспонсетиме</span><span class="sxs-lookup"><span data-stu-id="4d401-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="4d401-119">Представляет дату и время последнего полученного ответа.</span><span class="sxs-lookup"><span data-stu-id="4d401-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
|[<span data-ttu-id="4d401-120">ProposedStart</span><span class="sxs-lookup"><span data-stu-id="4d401-120">ProposedStart</span></span>](proposedstart-attendeetype.md) <br/> |<span data-ttu-id="4d401-121">Представляет предполагаемое время начала собрания для участника.</span><span class="sxs-lookup"><span data-stu-id="4d401-121">Represents an attendee's proposed start time for a meeting.</span></span> <br/> |
|[<span data-ttu-id="4d401-122">пропоседенд</span><span class="sxs-lookup"><span data-stu-id="4d401-122">ProposedEnd</span></span>](proposedend-attendeetype.md) <br/> |<span data-ttu-id="4d401-123">Представляет предложенное конечное время участника собрания.</span><span class="sxs-lookup"><span data-stu-id="4d401-123">Represents an attendee's proposed end time for a meeting.</span></span> <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4d401-124">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="4d401-124">Parent elements</span></span>

|<span data-ttu-id="4d401-125">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="4d401-125">**Element**</span></span>|<span data-ttu-id="4d401-126">**Описание**</span><span class="sxs-lookup"><span data-stu-id="4d401-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4d401-127">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="4d401-127">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="4d401-128">Представляет участников, которые необходимы для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="4d401-128">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="4d401-129">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="4d401-129">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="4d401-130">Представляет участников, которые не являются обязательными для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="4d401-130">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="4d401-131">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="4d401-131">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="4d401-132">Представляет запланированный ресурс для собрания.</span><span class="sxs-lookup"><span data-stu-id="4d401-132">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4d401-133">Примечания</span><span class="sxs-lookup"><span data-stu-id="4d401-133">Remarks</span></span>

<span data-ttu-id="4d401-134">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="4d401-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4d401-135">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="4d401-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4d401-136">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="4d401-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4d401-137">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="4d401-137">Schema name</span></span>  <br/> |<span data-ttu-id="4d401-138">Схема Types</span><span class="sxs-lookup"><span data-stu-id="4d401-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="4d401-139">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="4d401-139">Validation file</span></span>  <br/> |<span data-ttu-id="4d401-140">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="4d401-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4d401-141">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="4d401-141">Can be empty</span></span>  <br/> |<span data-ttu-id="4d401-142">False</span><span class="sxs-lookup"><span data-stu-id="4d401-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4d401-143">См. также</span><span class="sxs-lookup"><span data-stu-id="4d401-143">See also</span></span>

- [<span data-ttu-id="4d401-144">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="4d401-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

