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
description: Элемент Attendee представляет участников и ресурсы, необходимые для собрания.
ms.openlocfilehash: 60cb0839c2f6de69b833c11f4594d40c14cd8887
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ru-RU
ms.lasthandoff: 06/11/2018
ms.locfileid: "19761515"
---
# <a name="attendee"></a><span data-ttu-id="d3105-103">Участник</span><span class="sxs-lookup"><span data-stu-id="d3105-103">Attendee</span></span>

<span data-ttu-id="d3105-104">Элемент **Attendee** представляет участников и ресурсы, необходимые для собрания.</span><span class="sxs-lookup"><span data-stu-id="d3105-104">The **Attendee** element represents attendees and resources for a meeting.</span></span> 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 <span data-ttu-id="d3105-105">**AttendeeType**</span><span class="sxs-lookup"><span data-stu-id="d3105-105">**AttendeeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3105-106">Атрибуты и элементы</span><span class="sxs-lookup"><span data-stu-id="d3105-106">Attributes and elements</span></span>

<span data-ttu-id="d3105-107">В разделах ниже приводится описание атрибутов, дочерних и родительских элементов.</span><span class="sxs-lookup"><span data-stu-id="d3105-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3105-108">Атрибуты</span><span class="sxs-lookup"><span data-stu-id="d3105-108">Attributes</span></span>

<span data-ttu-id="d3105-109">Нет.</span><span class="sxs-lookup"><span data-stu-id="d3105-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3105-110">Дочерние элементы</span><span class="sxs-lookup"><span data-stu-id="d3105-110">Child elements</span></span>

|<span data-ttu-id="d3105-111">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3105-111">**Element**</span></span>|<span data-ttu-id="d3105-112">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3105-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3105-113">Mailbox</span><span class="sxs-lookup"><span data-stu-id="d3105-113">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d3105-114">Определяет адрес электронной почты полностью разрешенной.</span><span class="sxs-lookup"><span data-stu-id="d3105-114">Identifies a fully resolved e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="d3105-115">ResponseType</span><span class="sxs-lookup"><span data-stu-id="d3105-115">ResponseType</span></span>](responsetype.md) <br/> |<span data-ttu-id="d3105-116">Представляет тип получателя ответа, полученные на собрание.</span><span class="sxs-lookup"><span data-stu-id="d3105-116">Represents the type of recipient response that is received for a meeting.</span></span> <span data-ttu-id="d3105-117">Это свойство применяется только для элемента календаря Организатор собрания.</span><span class="sxs-lookup"><span data-stu-id="d3105-117">This property is only relevant to a meeting organizer's calendar item.</span></span>  <br/> |
|[<span data-ttu-id="d3105-118">LastResponseTime</span><span class="sxs-lookup"><span data-stu-id="d3105-118">LastResponseTime</span></span>](lastresponsetime.md) <br/> |<span data-ttu-id="d3105-119">Представляет дату и время последнего ответа, полученные.</span><span class="sxs-lookup"><span data-stu-id="d3105-119">Represents the date and time of the latest response that is received.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3105-120">Родительские элементы</span><span class="sxs-lookup"><span data-stu-id="d3105-120">Parent elements</span></span>

|<span data-ttu-id="d3105-121">**Элемент**</span><span class="sxs-lookup"><span data-stu-id="d3105-121">**Element**</span></span>|<span data-ttu-id="d3105-122">**Описание**</span><span class="sxs-lookup"><span data-stu-id="d3105-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3105-123">RequiredAttendees</span><span class="sxs-lookup"><span data-stu-id="d3105-123">RequiredAttendees</span></span>](requiredattendees.md) <br/> |<span data-ttu-id="d3105-124">Представляет участников, которые необходимы на участие в собрании.</span><span class="sxs-lookup"><span data-stu-id="d3105-124">Represents attendees that are required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d3105-125">OptionalAttendees</span><span class="sxs-lookup"><span data-stu-id="d3105-125">OptionalAttendees</span></span>](optionalattendees.md) <br/> |<span data-ttu-id="d3105-126">Представляет участников, которые не требуется на участие в собрании.</span><span class="sxs-lookup"><span data-stu-id="d3105-126">Represents attendees that are not required to attend a meeting.</span></span>  <br/> |
|[<span data-ttu-id="d3105-127">Ресурсы</span><span class="sxs-lookup"><span data-stu-id="d3105-127">Resources</span></span>](resources.md) <br/> |<span data-ttu-id="d3105-128">Ресурс запланированного собрания.</span><span class="sxs-lookup"><span data-stu-id="d3105-128">Represents a scheduled resource for a meeting.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d3105-129">Замечания</span><span class="sxs-lookup"><span data-stu-id="d3105-129">Remarks</span></span>

<span data-ttu-id="d3105-130">Схема, описывающая этот элемент, расположена в виртуальном каталоге EWS на компьютере с MicrosoftExchange Server 2007 и установленной ролью сервера клиентского доступа.</span><span class="sxs-lookup"><span data-stu-id="d3105-130">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3105-131">Сведения об элементе</span><span class="sxs-lookup"><span data-stu-id="d3105-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3105-132">Пространство имен</span><span class="sxs-lookup"><span data-stu-id="d3105-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3105-133">Имя схемы</span><span class="sxs-lookup"><span data-stu-id="d3105-133">Schema name</span></span>  <br/> |<span data-ttu-id="d3105-134">Схема Types</span><span class="sxs-lookup"><span data-stu-id="d3105-134">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3105-135">Файл проверки</span><span class="sxs-lookup"><span data-stu-id="d3105-135">Validation file</span></span>  <br/> |<span data-ttu-id="d3105-136">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3105-136">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3105-137">Может быть пустым</span><span class="sxs-lookup"><span data-stu-id="d3105-137">Can be empty</span></span>  <br/> |<span data-ttu-id="d3105-138">False</span><span class="sxs-lookup"><span data-stu-id="d3105-138">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3105-139">См. также</span><span class="sxs-lookup"><span data-stu-id="d3105-139">See also</span></span>

- [<span data-ttu-id="d3105-140">Элементы XML веб-служб Exchange в Exchange</span><span class="sxs-lookup"><span data-stu-id="d3105-140">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

