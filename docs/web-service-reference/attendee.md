---
title: Attendee
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
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/25/2018
ms.locfileid: "19761515"
---
# <a name="attendee"></a><span data-ttu-id="3cf1a-103">Attendee</span><span class="sxs-lookup"><span data-stu-id="3cf1a-103">Attendee</span></span>

<span data-ttu-id="3cf1a-104">Элемент " **участник** " представляет участников и ресурсы собрания.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="3cf1a-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="3cf1a-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3cf1a-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="3cf1a-106">Attributes and elements</span></span>

<span data-ttu-id="3cf1a-107">В следующих разделах описываются атрибуты, дочерние и родительские элементы.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3cf1a-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="3cf1a-108">Attributes</span></span>

<span data-ttu-id="3cf1a-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3cf1a-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="3cf1a-110">Child elements</span></span>

|<span data-ttu-id="3cf1a-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3cf1a-111">**Element**</span></span>|<span data-ttu-id="3cf1a-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3cf1a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cf1a-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="3cf1a-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="3cf1a-114">Определяет полностью разрешенный адрес электронной почты.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="3cf1a-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="3cf1a-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="3cf1a-116">Представляет тип ответа получателя, полученный для собрания.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="3cf1a-117">Это свойство относится только к элементу календаря организатора собрания.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="3cf1a-118">ластреспонсетиме</span><span class="sxs-lookup"><span data-stu-id="3cf1a-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="3cf1a-119">Представляет дату и время последнего полученного ответа.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3cf1a-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="3cf1a-120">Parent elements</span></span>

|<span data-ttu-id="3cf1a-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="3cf1a-121">**Element**</span></span>|<span data-ttu-id="3cf1a-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="3cf1a-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3cf1a-123">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="3cf1a-123">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="3cf1a-124">Представляет участников, которые необходимы для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-124">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3cf1a-125">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="3cf1a-125">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="3cf1a-126">Представляет участников, которые не являются обязательными для участия в собрании.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-126">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="3cf1a-127">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="3cf1a-127">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="3cf1a-128">Представляет запланированный ресурс для собрания.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-128">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3cf1a-129">Примечания</span><span class="sxs-lookup"><span data-stu-id="3cf1a-129">Remarks</span></span>

<span data-ttu-id="3cf1a-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="3cf1a-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3cf1a-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="3cf1a-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3cf1a-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="3cf1a-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3cf1a-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="3cf1a-133">Schema name</span></span>  <br/> |<span data-ttu-id="3cf1a-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="3cf1a-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="3cf1a-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="3cf1a-135">Validation file</span></span>  <br/> |<span data-ttu-id="3cf1a-136">Types. xsd</span><span class="sxs-lookup"><span data-stu-id="3cf1a-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3cf1a-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="3cf1a-137">Can be empty</span></span>  <br/> |<span data-ttu-id="3cf1a-138">False</span><span class="sxs-lookup"><span data-stu-id="3cf1a-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3cf1a-139">См. также</span><span class="sxs-lookup"><span data-stu-id="3cf1a-139">See also</span></span>

- [<span data-ttu-id="3cf1a-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="3cf1a-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

